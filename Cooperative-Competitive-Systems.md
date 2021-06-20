This page forms part of the [[Proto AGI v1]] series.


# Introduction

## Principles

* Distributed working memory
* Distributed control via mutual competition and cooperation, and shared learning.
* Reusable templates


# Templates

## Gated Output Selection

This template uses an active selection gate to enable the output to be chosen between two or more competing "processor" components. For example, selecting between the output from a habitual NN planner, and a bayesian model-based planner. The gate NN learns to choose which component produces the best output for different situations, and the competing components learn from each event regardless of whether they were involved.

![gated output selection](files/Cooperative-competitive-systems.png)

### Processors
All processors must output same representation, but they can have different implementations. Eg: NN, bayesian inference engine, bayesian planning engine, decision tree.

### Selection
The Selector is a NN that outputs a vector of size `n` floats.

The Gate forwards the output via one of the following mechanisms:
* `argmax` across the selector output and using just that processor's output, or
* `softmax` across the selector output and using for weighted sum of processor outputs, or
* `log prob` frequency with probabalistic selection of processor output.

### Training
For NN processors, gradient descent against the gate's output will apply training pressure to the individual processor (or processors) that was used for the particular output at the time; however other processors will not receive training pressure (or have proportionately negligeable pressure). Thus, it is preferable to apply training pressure to each processor individually, regardless of whether it was used for the output.

Training pressure must also be applied to the final output, in order to train the Selector. 

### Variations
* Selection context: supply processor inputs to Selector too, to provide extra context to enable output selection.
* Certainty-based selection: processors updated to output certainty measure an addition to other data. Selector becomes a hard-wired primitive transformer from certainties into log prob category selection.
* NN-based Gate: combine Selector into Gate as a single NN. More flexible, but significantly adds to training dimensions because Gate now dynamically produces final output, rather than applying a simple deterministic selection.

If all processors are NNs and have no additional training pressure, then this subsystem can be replaced with a single NN.


## Vetoing Reflex

This template models a reflex processor with right of veto. It draws inspiration from biology to enable processors to indicate a level of _activation_ in their output, and then combines an always-active main processor whose output is usually used, with a usually-inactive veto processor that can take over when needed.

A _strength_, `y_i`, is determined from a processor output vector by taking the mean of vector component amplitudes (ie: `ave(|.|)`). The veto processor is given a boost in the form of a `β` multiplier against its strength. And then the final output is chosen as the soft-arg-max of the processor outputs (`o0`, `o1`), based on the weights `y0` and `β*y1`.

![vetoing reflex](files/Cooperative-competitive-systems-vetoing-reflex.png)

Some form of regularization will likely be needed to keep both processor outputs on the same scale.

### Learning
There are two pressures that need to be hard-wired for this architecture to work:
* The veto processor should be inactive most of the time so that it can specialise to reflex situations where it is needed. This can be achieved through pre-training.
* The main processor needs to be conservative with its signal strength, so that the veto processor has the strength to override it when needed. This can be achieved through regularization, and also through treating signal strength as equating to effort and penalising agent behaviours that employ more effort than needed.

### Variations
* `β` could be either hard-wired or a learnable parameter. Higher values mean that executive control cannot override the reflex.
* The veto processor is probably pre-trained and then not learnable during main agent learning. However, there may be ways for the veto processor to learn too.

### Mimicking biological neuronal signal strength
Biological neurons have both signal _value_ and _strength_, encoded in the form of spike trains with different frequencies, amplitudes, and inactive periods. In contrast, the typical usage of an AI neuron is that its output is interpreted as _value_ only. Another difference is that AI neurons output a value in range -ve to +ve, whereas biological neurons only output values in range zero through +ve values but may be interpreted as excitatory or inhibitory, depending on the physical structure.

AI neural networks can take inspiration from biological neuronal signal strength by treating a positive output as excitatory, a negative output as inhibitory, and a value close to zero as inactive.

### Mimicking biological veto mechanisms
In biology, a reflex machinism can be primarily inactive, but when needed it can emit a signal with high strength that supercedes any other signals. Additionally, a person can often consciously choose to override their reflex; the success of this depending on the specific reflex being overridden, and on training.

## Amplitude-based Selection

This template is a generalisation of the Vetoing Reflex solution. It uses relative signal strength from two or more processors, without any implied precedence. It would typically be used where multiple processors compete that have different architectures, different inputs, or different behavioural purposes. The later case requires that the processors are independently trained.

If all processors are the same, and differ only in random initialization values, then this simplifies to an ensemble model.

![amplitude-based selection](files/Cooperative-competitive-systems-amplitude-based-selection.png)

For each `i`-th processor, it's output `o_i` is a vector of length `m`, and the amplitude `a_i` of that output is calculated as `L1(o_i)/m` (ie: the average of absolute value of each component of the vector). Soft arg-max (typically referred to as just 'softmax') is applied to the amplitudes `a_0` ... `a_n`, producing weights `w_0` ... `w_1`: `w_i = e^a_i / Σ(e^a_j)`.

The softmax function provides a smooth way of switching between selecting just one processor output and combining the output of multiple processors. So, finally, the output is produced as: `Σ(w_i * o_i)`.

### Training
The softmax function allows some backpropagation from output to all processors. However that backpropagation is heavily attenuated for processors that produced low amplitude values. Best results will likely be achieved where some training pressure can be directly applied to each processor output.

## State
This template simply adds internal state to components, such as through the use of RNN components.

This can be used for useful behaviours such as:
* Priming - eg: where a Reviewer component is "primed" in past time steps to be biased towards a particular outcome.
* Distributed Working Memory - eg: inputs from other components is stored into the components local state, for use in subsequent time steps.

### Training
It is naively assumed that RL processes are sufficient to produce meaningful results. However, this remains to be seen. It is unlikely to be as affective as RNN in simple sequential data processing, where the RNN is trained against a high frequency of data.

## Evaluation Loop

