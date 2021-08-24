# PREPRINT DRAFT

## Title: A Characterisation of processing loops in AI and biological neural networks and its implications for understanding Consciousness

# Abstract

Shows that any sufficiently advanced processing system requires loopy processing, which requires regulation, which requires a self-model, and that this structure can lead to self-referential conclusions about an agents own mental faculties and their involvement in its own agency.

# Introduction

Any computational system is limited in the complexity that it can handle within a single computational step. For embodied agents, this appears as a limit on the environmental complexity that they can sufficiently model and respond to within a single "time step" (citation needed). For more complex problems, multiple steps of processing are required in order to determine the next physical action. Such multiple processing steps may entail, for example, further analysis of the environment in order to better model its state; or it may entail action planning over multiple iterations.

In biology, this provides an option for evolutionary pressures to trade off between a more energy hungry complex brain and a simpler less energy intensive one that takes longer to make some decisions.

According to the _good regulator theorem_ (citation needed), and as the most promising AI models today are showing (citationS needed), in order for an agent to operate within a complex environment, it must model that environment (citation needed). Additionally, if an embodied agent has complex actions, it must model its body (citation needed).

Agents that incorporate multi-step processing have a second kind of action: one that changes its internal data state without affecting its physical state. In humans, we call this "thought". Agents with such _non-physical actions_, thus must additionally model their non-physical self. <<tbd: this argument is still a little weak>>.

In order for an agent to model its non-physical self, it requires direct access to the inputs, actions, and outcomes of that non-physical control. To understand this statement, consider the case of fluent aphasia, caused by damage to the Wernicke's area of the brain. Individuals with fluent aphasia can easily produce speech, but it is typically full of many meaningless words and often unnecessarily long winded. Wernicke's area is associated with language comprehension and, as such, provides a corrective mechanism during speech production in a neurotypical individual (_Wernicke's area_).


tbd: also needed for corollary discharge?

_tbd_: argue why needing a mental-schema also mandates needing direct awareness of thought.

_tbd_: introduce body schema and mind schema.

_tbd_: argue for hierarchical architecture.

# Visceral Loop

This paper introduces the concept of a _visceral loop_ as a characterisation of processing within a looping AI or biological system. The visceral loop is so named because it refers to an agent concluding that it experiences consciousness "in a visceral way". It identifies, at the most optimum, the three iterations of a processing loop required for an agent to make such a conclusion.

Consider the following sequence of internal mental observations:
1. "What's that red blob in the tree? Oh, it's an apple".
2. "Oh, those thoughts just came from my mind, and not from the outside world".
3. "That's what consciousness is. I am conscious".

We shall now break that sequence down.

**Iteration 1**:

At the beginning of the first step (or _iteration_) in the sequence above, we assume that the agent (biological or otherwise) has some _a priori_ knowledge of the concept of consciousness, but has never previously bothered to analyse itself in that respect.

During the first iteration, the agent's processing capabilities produce a non-self-referential inference. In the example above, an inference about the observed red blob being an apple.

As stated within the introductory section, agents with sufficiently complex self-modelling requirements must have direct observation of their own sequence of thought actions. Thus, the act of making the iteration 1 inference becomes available for subsequent processing.

**Iteration 2**:

During iteration 2, the agent makes a self-referential inference about its prior mental action.

The agent has multiple sense inputs, most of which observe either the physical environment in which it exists, or observe its physical body. The agent's ability to observe its own non-physical actions counts as an additional sense input. During iteration 2, the agent explores its memory of its prior action, and produces an inference about that action; specifically, that the action was non-physical and sourced from within the agent's own processing capabilities. In other words, with reference to the agent's mind schema, the action was produced by its own mind schema...

**Iteration 3**:
Iteration 3 thought takes that to the next level. The relationship itself becomes the input data that is further processed in relation to the mind schema. With sufficient thought in this category, one can conclude themselves as conscious.

_tbd_: flesh out.

# Formal Description of Visceral Loop

Iteration 1:

1. a sense input or some past state is processed, producing `t`: some output conclusion, decision, action, or intermediate logical step

Iteration 2:

2. prerequisite: `t` is present (in model)
3. prerequisite: `t` is sourced from 'I' (as indicated through sense labeling)
4. prerequisite: ∃ memory of producing `t` in past thought
5. `t` is selected as focus of attention for processing, producing: i) fact of presence of `t`, and ii) relationship of `t` to 'I'

Iteration 3:

6. prerequisite: ∃ some a priori notion about consciousness or experience
7. prerequisite: model contains i) fact of presence of `t`, and ii) relationship of `t` to 'I'
8. `t` and its relationship to `I` is selected as focus of attention for processing, producing: "I am conscious of `t`"


....


Formally, the three iterations of the visceral loop can be represented using a mathematical notation that highlights the inputs to the function, and its result:

* Iteration 1: f(inputs) -> x - some result of simple thought
* Iteration 2: f(x, mind-schema) -> relationship(x : mind-schema)
* Iteration 3: f(relationship(x : mind-schema), mind-schema) -> relationship(mind-schema : mind-schema)

# Consciousness

_tbd_

If we ascribe phenomenal experience as a feeling, and recognise that feelings are just additional data input produced through heuristic predictions, then we see that a simulation of a visceral loop, that we intuit to have no phenomenal experience, is computationally indistinguishable from a biological visceral loop that we know to be accompanied by such phenomenon.

Visceral loop explains why fRMI studies have shown that we become aware of a decision after its made. Because it takes extra processing cycles to consciously consider the fact of the decision being made. In short: we can only think about one thing at a time, so the decision itself and thought about the decision require separate steps.

The visceral loop can be used to explain how someone concludes themselves as conscious. It can also be used to classify the kinds of thought that occur within an agent, and the kinds of thought that it's possible for an agent to have. For example, it may be the case that simpler organisms only ever operate with Iteration 1 thought.


# Summary and Conclusions

_tbd_


# References

Conant, R. C., and Ashby, W. R. (1970). Every good regulator of a system must be a model of that system. Int. J. Systems Sci., vol. 1, No. 2, 89-97.

Wernicke's area. (n.d.). In _Wikepedia_. https://en.wikipedia.org/wiki/Wernicke%27s_area. 


----
# Discarded content

For example, many current artificial _reinforcement learning_ (RL) agents continually choose actions at a fixed rate of one (discrete or continuous) action per time step.
