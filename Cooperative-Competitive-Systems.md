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


## Amplitude-based Selection
This template uses relative signal strength from processor outputs to select selection gate to enable the output to be chosen between two or more competing "processor" components.

### Variations
* When two processors are arranged such that one is an always-active primary processor and the other is a usually-inactive processor, this models a reflex mechanism with right of veto.

## Evaluation Loop

