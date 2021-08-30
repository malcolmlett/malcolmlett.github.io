# PREPRINT DRAFT

## Title: A Characterisation of processing loops in AI and biological neural networks and its implications for understanding Consciousness

# Abstract

Shows that any sufficiently advanced processing system requires loopy processing, which requires regulation, which requires a self-model, and that this structure can lead to self-referential conclusions about an agents own mental faculties and their involvement in its own agency.

# Introduction

Any computational system is limited in the complexity that it can handle within a single computational step. For embodied agents, this appears as a limit on the environmental complexity that they can sufficiently model and respond to within a single "time step" (citation needed). For more complex problems, multiple steps of processing are required in order to determine the next physical action. Such multiple processing steps may entail, for example, further analysis of the environment in order to better model its state; or it may entail action planning over multiple iterations.

In biology, this provides scope for evolutionary pressures to trade off between a more energy hungry complex brain and a simpler less energy intensive one that takes longer to make some decisions.

The _good regulator theorem_ says that "every good regulator of a system must be a model of that system" (Conant & Ashby, 1970). A biological or artificial agent in a system must thus model that system in order to regulate its state within that system. An embodied agent with complex actions must also model its body in order to regulate its actions. This is seen in the brain as the _body schema_ (Proske & Gandevia, 2012).

Agents that incorporate multi-step processing have an additional kind of action: one that changes its internal data state without affecting its physical state. In humans, we call this _thought_. Agents with such _non-physical actions_, thus must additionally model their non-physical self.

In order for an agent to model its non-physical self, it requires direct access to the inputs, actions, and outcomes of that non-physical control. To understand this statement, consider the case of fluent aphasia, caused by damage to the Wernicke's area of the brain. Individuals with fluent aphasia can easily produce speech, but it is typically full of many meaningless words and often unnecessarily long winded. Wernicke's area is associated with language comprehension and, as such, provides a corrective mechanism during speech production in a neurotypical individual (_Wernicke's area_).


# Visceral Loop

This paper introduces the concept of a _visceral loop_ as a characterisation of processing within a looping biological or AI agent. The visceral loop is so named because it refers to an agent concluding that it experiences consciousness "in a visceral way". It identifies, at the most optimum, the three iterations of a processing loop required for an agent to make such a conclusion.

Consider the following sequence of internal mental observations:
1. "What's that red blob in the tree? Oh, it's an apple".
2. "Oh, I those thoughts just came from my mind, and not from the outside world".
3. "That's what consciousness is. I am conscious".

Those three observations are produced from (at least) three iterations of a high order processing system. However, important distinctions can be drawn between the kinds of data represented as input and result within each of those loop iterations.

The visceral loop characterises those three observations as follows.

**Iteration 1**:

We assume that the agent (biological or otherwise) has some _a priori_ knowledge of the concept of consciousness, but has never previously analysed itself in that respect.

The first step in the thought sequence above is characterised as _Iteration 1_, whereby the agent produces an inference that is non-self-referential in terms of its mind schema. In that example the agent draws an inference about the observed red blob being an apple.

As stated within the introductory section, agents with sufficiently complex self-modelling requirements must have direct observation of their own sequence of thought actions. Thus, iteration 1 inference becomes available for subsequent processing.

**Iteration 2**:

During _Iteration 2_, the agent makes an inference about a prior Iteration 1 mental action, and this inference draws reference to its mind schema. The second step in the thought sequence above is an example of this, whereby the agent realises that it is aware of its own thoughts.

The agent has multiple sense inputs, most of which observe either the physical environment in which it exists, or observe its physical body. The agent's ability to observe its own non-physical actions counts as an additional sense input. During iteration 2, the agent explores its memory of its prior non-physical action, and produces an inference about that action; specifically, i) that the action was non-physical, and ii) that it was sourced from within the agent's own processing capabilities.

The result of Iteration 2 is a relationship between a simple Iteration 1 thought and the agent's mind schema.

**Iteration 3**:
During _Iteration 3_ that relationship becomes the input data that is further processed in relation to the mind schema. The result is an inferred self-referential relationship about its own mind schema.

In the third observation in the example above, the agent draws upon its memory of its immediately prior thought, and upon its _a priori_ knowledge about the concept of consciousness. Its immediately prior thought was a relationship between a simple thought and its own mind schema. Its _a priori_ knowledge of consciousness is effectively a set of beliefs about mind schemas in general. The conclusion it draws is a statement of belief about its own mind schema.

## Formal Description of Visceral Loop

A formal definition of the visceral loop shall now be presented.

Let:
* `X` be the agent's set of beliefs about the external world
* `B` be the agent's set of beliefs about its own physical body
* `M` be the agent's set of beliefs about minds and it own mind
* `f(..)` be the function executed by the agent on the specified inputs in order to draw inferences
* `x_i` be an inference that results from the execution of `f` (it may be any output conclusion, decision, action, or intermediate logical steps)

Iteration 1:

Given `s`, some sense input or past state, iteration 1 inferences are of the following form:

* inference x_1: `f(s, X U B) -> x_1`

Iteration 2:

2. prerequisite: `x_1` is present
3. prerequisite: `x_1` is sourced from 'I' (as indicated through sense labelling)
4. prerequisite: ∃ memory of producing `x_1` in past thought
5. prerequisite: `x_1` is selected as focus of attention for processing
ie: producing: i) fact of presence of `x_1`, and ii) relationship of `x_1` to mind schema `M`

* inference x_2: `f(x_1, M) -> relationship(x_1 -> M)`

Iteration 3:

6. prerequisite: ∃ some _a priori_ belief about consciousness or experience
7. prerequisite: model contains i) fact of presence of `x_1`, and ii) relationship of `x_1` to `M`
8. `x_1` and its relationship to `M` is selected as focus of attention for processing, producing: "I am conscious of `t`"

* inference x_3: `f(x_2, M) = f(relationship(x_1 -> M), M) -> relationship(M -> M)`


....


Formally, the three iterations of the visceral loop can be represented using a mathematical notation that highlights the inputs to the function, and its result:

* Iteration 1: f(inputs) -> x - some result of simple thought
* Iteration 2: f(x, mind-schema) -> relationship(x : mind-schema)
* Iteration 3: f(relationship(x : mind-schema), mind-schema) -> relationship(mind-schema : mind-schema)

# Consciousness

_tbd_: argue for hierarchical architecture.

_tbd_: argue why needing a mental-schema also mandates needing direct awareness of thought.

_tbd_

If we ascribe phenomenal experience as a feeling, and recognise that feelings are just additional data input produced through heuristic predictions, then we see that a simulation of a visceral loop, that we intuit to have no phenomenal experience, is computationally indistinguishable from a biological visceral loop that we know to be accompanied by such phenomenon.

Visceral loop explains why fRMI studies have shown that we become aware of a decision after its made. Because it takes extra processing cycles to consciously consider the fact of the decision being made. In short: we can only think about one thing at a time, so the decision itself and thought about the decision require separate steps.

The visceral loop can be used to explain how someone concludes themselves as conscious. It can also be used to classify the kinds of thought that occur within an agent, and the kinds of thought that it's possible for an agent to have. For example, it may be the case that simpler organisms only ever operate with Iteration 1 thought.


# Summary and Conclusions

_tbd_


# References

Conant, R. C., and Ashby, W. R. (1970). Every good regulator of a system must be a model of that system. Int. J. Systems Sci., vol. 1, No. 2, pp 89-97. https://doi.org/10.1080/00207727008920220. \[[Full Text](http://pespmc1.vub.ac.be/books/Conant_Ashby.pdf)\]

Proske, U., and Gandevia, S. C. (2012). The Proprioceptive Senses: Their Roles in Signaling Body Shape, Body Position and Movement, and Muscle Force. Physiological Reviews 2012 92:4, pp 1651-1697. https://doi.org/10.1152/physrev.00048.2011.

Wernicke's area. (n.d.). In _Wikepedia_. https://en.wikipedia.org/wiki/Wernicke%27s_area. 


----
# Discarded content

tbd: also needed for corollary discharge?

For example, many current artificial _reinforcement learning_ (RL) agents continually choose actions at a fixed rate of one (discrete or continuous) action per time step.
