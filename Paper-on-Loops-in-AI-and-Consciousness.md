# PREPRINT DRAFT

## Title: A Characterisation of processing loops in AI and biological neural networks and its implications for understanding Consciousness

# Abstract

Shows that any sufficiently advanced processing system requires loopy processing, which requires regulation, which requires a self-model, and that this structure can lead to self-referential conclusions about an agents own mental faculties and their involvement in its own agency.

# Introduction

Any computational system is limited in the complexity that it can handle within a single computational step. For embodied agents, this appears as a limit on the environmental complexity that they can sufficiently model and respond to within a single "time step" (citation needed). For more complex problems, multiple steps of processing are required in order to determine the next physical action. Such multiple processing steps may entail, for example, further analysis of the environment in order to better model its state; or it may entail action planning over multiple iterations.

In biology, this provides scope for evolutionary pressures to trade off between a more energy hungry complex brain and a simpler less energy intensive one that takes longer to make some decisions.

An agent that regulates its environment operates within a system described in Fig 1. The environment state `S_env` changes with some ambient dynamics `env dynamics`, and the agent performs action `A_env` against the environment in order to regulate it towards some target. The environment state outcome `O_env` is influenced by both `D_env(t)` and `A_env`. 
    Fig 1:    
    {diagram}
    S_env + D_env(t) + A_env = O_env
    {diagram}

According to the _good regulator theorem_, if the agent is to regulate the environment state it must be a model of the system (Conant & Ashby, 1970). Furthermore, we can say that the efficiency of the agent to regulate its environment depends on its accuracy in modelling the system. Errors in the accuracy of the model result in errors in the regulation of the system. For learning agents, those errors must be used to adjust the model. An agent that must regulate its external environment requires the tuple `<S_env, A, O_env>` in order to adjust its model.

An embodied agent with complex actions requires an additional level of regulation. Not only must it regulate its external environment, it must also regulate its own physical state. This includes both maintaining homeostasis and controlling action. Such an agent thus operates in a system that additionally has body state `S_body` with ambient dynamics `D_body(t)`. The agent performs action `A_body` against its body, producing outcome `O_body`. Summarised as follows:

    S_body + D_body(t) + A_body = O_body
    
The agent's actions are performed in order to regulate it towards some target, which is dynamically inferred based on its requirement for body homeostasis and for environment action `A_env`. Like for regulation of the environment, the agent requires a tuple `<S_body, A_body, O_body>` in order to train its model.

Agents that incorporate multi-step processing have an additional kind of action: one that changes its internal data state without affecting its physical state. Importantly, as such _non-physical_ actions may not elicit any change to `S_body` or `S_env`, this system also requires regulation. Thus the agent has non-physical state `S_mind` with ambient dynamics `D_mind(t)`, and performs action `A_mind` producing outcome `O_mind`, summarised as follows:

    S_mind + D_mind(t) + A_mind = O_mind
    
The agent's non-physical actions are performed in order to regulate towards some target, which is dynamically inferred based on its requirement for environment action `A_env`, body action `A_body`, and possibly for some form of non-physical homeostasis. Like for both the environment and body, the agent must train its model for regulation from a tuple `<S_mind, A_mind, O_mind>`.

By way of example, consider the case of fluent aphasia, caused by damage to the Wernicke's area of the brain. Individuals with fluent aphasia can easily produce speech, but it is typically full of many meaningless words and often unnecessarily long winded. Wernicke's area is associated with language comprehension and, as such, provides a corrective mechanism during speech production in a neurotypical individual (_Wernicke's area_).

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

...

Let's first establish a baseline. I am unable to think of any rationale way in which I may consciously experience something and yet be unable to subsequently think about that experience. I would seem that being able to think about our conscious experiences is a fundamental component of consciousness. The following claims are derived from this statement, without further proof:

Claim 1:
* All conscious experience is subsequently available for further thought.

Claim 2:
* All conscious experience can be knowingly thought about.

Note that claim 1 does not require that all conscious experience is thought about; only that it is available for such thought. Claim 2 extends claim 1 in an important way that depends on the distinction indicated by the keyword _knowingly_. A processing system may process some data and produce a result from it, without being able to subsequently introspect any fact about that operation. Here, _knowingly_ is used to refer to a processor being able to subsequently introspect both the input and output, to know the causal relationship between, and to perform additional processing about the fact that it had performed that operation. Additionally, the act of performing that additional processing must itself be _knowable_.

Theorem 1:
* ...tbd better: what data is possible to enter visceral loop iteration 2 as inputs defines the maximum set of the content of conscious experience.

Proof:
* As per claim 1, all of conscious experience must be available for further thought. The ability to process that thought in relation to one's own mind, is characterised as visceral loop iteration 2.
* For any given experience, one of three possibilities is true:
    a) it is used as input to iteration 2 and thus becomes thought about.
    b) it is possible for it to be used as input to iteration 2, but current attentional focus avoids that in favour of other processing.
    c) it is not possible for it to be used as input to iteration 2 (eg: due to some incompatibility of structure or a lack of data path to iteration 2).
* Both possibilities (a) and (b) satisfy the theorem. Possibility (c) fails on claim 1, and thus must not be a conscious experience.
* 

So an experience must either be thought about in relation to one's own mind, in which case it enters iteration 2 as input, or it must avoid being thought about in relation to one's own mind, in which case the individual is not aware of having had that experience.
*
* As conscious experience is characterised by the ability to think about that experience, and there is no experience that we cannot subsequently consciously think about, all of conscious experience must enter iteration 2 or otherwise it cannot be consciously experienced.



Theorem 2:
* ...tbd better: what data is possible to exit visceral loop iteration 2 as output defines wholly the content of conscious experience.

Proof:
* Theorem 2 can only be weakly proven under a further assumption: that there is no meta-physical processing or processing of other sorts via physics or algorithmic capabilities not currently known to modern science.
* ...tbd better: the ability to think about something, and to know that you think about something requires a recursive ability to process that thing, and the knowledge of that thing, and the knowledge of knowing about that thing, and so forth. Thus data must exit iteration 2 and also exit iteration 3 in order for it to be knowingly consciously experienced. And, as a slight extension of claim 1, it is only consciously experienced if it is knowlingly consciously experienced.





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
