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
    
The agent's actions are performed in order to regulate it towards some target, which is dynamically inferred based on its requirement for body homeostasis and for environment action `A_env`. Like for regulation of the environment, the agent requires a tuple `<S_body, A_body, O_body>` in order to train its model. Neuroscience has identified such a model in mammals, known as the _body schema_ (Proske & Gandevia, 2012).

Agents that incorporate multi-step processing have a third kind of action: one that changes its internal data state without affecting its physical state. Importantly, as such _non-physical_ actions may not elicit any change to `S_body` or `S_env`, this system also requires regulation. Thus the agent has non-physical state `S_mind` with ambient dynamics `D_mind(t)`, and performs action `A_mind` producing outcome `O_mind`, summarised as follows:

    S_mind + D_mind(t) + A_mind = O_mind
    
The agent's non-physical actions are performed in order to regulate towards some target, which is dynamically inferred based on its requirement for environment action `A_env`, body action `A_body`, and possibly for some form of non-physical homeostasis. Like for both the environment and body, the agent must train its model for regulation from a tuple `<S_mind, A_mind, O_mind>`.

By way of example, consider the case of fluent aphasia, caused by damage to the Wernicke's area of the brain. Individuals with fluent aphasia can easily produce speech, but it is typically full of many meaningless words and often unnecessarily long winded. Wernicke's area is associated with language comprehension and, as such, provides a corrective mechanism during speech production in a neurotypical individual (_Wernicke's area_).

The need for a mind-regulating agent to model the behaviour of its mind suggests that it must incorporate a functional equivalent of the body schema, which this paper refers to as the _mind schema_. Other research has drawn similar conclusions (Graziano, 2017).

# Visceral Loop

This paper introduces the concept of a _visceral loop_ as a characterisation of processing within a looping biological or AI agent. The visceral loop is so named because it refers to an agent concluding that it experiences consciousness "in a visceral way". It identifies that a processing loop with sufficient representational capabilities can, at the most optimum, conclude itself as conscious within three iterations of the loop. Each of those iterations have specific characteristics, and the visceral loop characterises thought as falling into one of those three iterations.

Let:
* `E` be the agent's set of beliefs about the external world
* `B` be the agent's set of beliefs about its own physical body (drawn from the body schema) and of bodies in general, and if it has a concept of "I" then this set includes a belief that relates other body beliefs to "I"
* `M` be the agent's set of beliefs about its own mind (drawn from the mind schema) and of minds in general, and if it has a concept of "I" then this set includes a belief that relates other mind beliefs to "I"
* `f(..)` be the function executed by the agent on the specified inputs in order to draw inferences

`M` can be thought of as an agent's "theory of mind", because it relates to not such itself but also its ability to predict the hidden mental state of others.

**Iteration 1:**

Let `x` be an inference produced as the result of a processing step, such that it does not draw any reference to `M` (ie: if `x` is a value then `x ∉ M`, or if `x` is a relation of two values then `x = relation{a:b}` such that `a ∉ M` and `b ∉ M`, or if `x` is a relation involving a set then `x = relation{a:B}` such that `a ∉ M` and `B ⊄ M`). Given some sense input or past state `s`, a processing step is characterised as visceral loop _Iteration 1_ if it is of the following form:

* `f(s, E ∪ B ∪ M) -> x`

**Iteration 2:**

Iteration 2 requires an agent to have sufficient representational capabilities to draw inferences that represent relations involving `M`. Given some prior inference `y`, a processing step is characterised as visceral loop _Iteration 2_ if it is of the following form, and the relation with respect to `M` is non-empty, and it can not be characterised as _Iteration 3_:

* `f(y, E ∪ B ∪ M) -> relation{y:M}`


**Iteration 3:**

Iteration 3 likewise requires the agent can represent relations involving `M`. Given some prior inference `relation{z, M}`, and some belief `m ∈ M`, a processing step is characterised as visceral loop _Iteration 3_ if it is of the following form and the relation with respect to `M` is non-empty:

* `f(relation{z:M}, E ∪ B ∪ M) -> relation{m:M}`


Iteration 1 represents the most common kind of data processing, such as spending multiple processing cycles to refine the identification of something within the visual field. While an agent's mind schema may be used to control the thought process, the result of Iteration 1 never makes any reference to the agent's own mind schema.

Iteration 2 processing steps draw conclusions that relate past conclusions to the agent's theory of mind. 

..tbd.. examples...

# Consciousness

The visceral loop can be applied to understand the thought processes whereby an individual concludes themselves as conscious. Consider the following sequence of internal mental observations:
1. "What's that red blob in the tree? Oh, it's an apple".
2. "Oh, those thoughts just came from my mind, and not from the outside world".
3. "That's what consciousness is. I am conscious".

The first observation is a straightforward example of Iteration 1 that does not make any self-reference to the agent's theory of mind (of their own mind or of others).

The second observation is an example of Iteration 2. However it is of specific form, whereby the individual produces an inference that identifies the source of the past thought in relation to their own mind schema (recall that this is a subset of `M`).

The third observation is additionally a specific form of Iteration 3, whereby the individual produces an inference based on the prior specialisation of Iteration 2, and produces an inference as a statement of fact about their own mind-schema. In this observation, the resultant inference is in relation to some _a priori_ conception about consciousness in general.

The concept of the visceral loop may appear simple, but it has important implications for understanding consciousness. By way of example of its descriptive power, two theorems of consciousness are offered in the text that follows.

Let's first establish a baseline. I am unable to think of any rationale way in which I may consciously experience something and yet be unable to subsequently knowingly think about that experience. Thus, it would seem that being able to knowingly think about our conscious experiences is a fundamental component of consciousness. The following claims are derived from this statement, without further proof:

Claim 1:
* All conscious experience is subsequently available for further thought.

Claim 2:
* For all thought about conscious experience, the individual can identify that thought as being their own.

Claim 3:
* All thought about conscious experience is itself a conscious experience.

Note that these claims do not assume that all conscious experience is thought about; only that it is available for such thought.

Theorem 1:
* what data is possible to enter visceral loop iteration 2 as input defines an upper boundary on the content of conscious experience.

Proof:
* In order for an individual to identify thought as being their own, they must have some beliefs about thought and how it relates to themselves as an individual entity. This is the mind schema of which iteration 2 is focused upon.
* As per claims 1 and 2, all of conscious experience must be available for further thought and the individual must be able to identify that thought as their own. This requires the ability to process that thought in relation to one's own mind, which is characterised as visceral loop iteration 2.
* Any supposed experience that is not available for input to iteration 2, is thus not a conscious experience.
* For any given experience, one of three possibilities is true:
    a) it is used as input to an iteration 2 processing step.
    b) it is _possible_ for it to be used as input to iteration 2, but current attentional focus avoids that in favour of other processing.
    c) it is not possible for it to be used as input to iteration 2, eg: due to some incompatibility of structure or a lack of data path to iteration 2.
* Both possibilities (a) and (b) satisfy the theorem. Possibility (c) fails on claim 2, and thus must not be a conscious experience.
* Possibility (c) fails on claim 2 because the individual
* 
* As conscious experience is characterised by the ability to think about that experience, and there is no experience that we cannot subsequently consciously think about, all of conscious experience must enter iteration 2 or otherwise it cannot be consciously experienced.


Theorem 2:
* Inferences produced by visceral loop iteration 2 processing define wholly the content of conscious experience.

Proof:
* Theorem 2 can only be weakly proven under a further assumption: that there is no meta-physical processing or processing of other sorts via physics or algorithmic capabilities not currently known to modern science.
* An experience must either be thought about in relation to one's own mind, in which case it enters iteration 2 as input and an outcome is produced relating the experience to one's own mind, or it must avoid being thought about in relation to one's own mind, in which case the individual is not aware of having had that experience.
* ...tbd better: the ability to think about something, and to know that you think about something requires a recursive ability to process that thing, and the knowledge of that thing, and the knowledge of knowing about that thing, and so forth. Thus data must exit iteration 2 and also exit iteration 3 in order for it to be knowingly consciously experienced. And, as a slight extension of claim 1, it is only consciously experienced if it is knowingly consciously experienced.

Theorem 2 summarises the recursive nature of conscious experience.


An example of Theorem 2 is where an event occurs that is potentially available for conscious experience, but it does not become an iteration 2 inference at the time. The individual may still have a memory of that past event, and upon recalling that past event may draw an iteration 2 inference about it, at which time it becomes a conscious experience.

If we ascribe phenomenal experience as a feeling, and recognise that feelings are just additional data input produced through heuristic predictions, then we see that a simulation of a visceral loop, that we intuit to have no phenomenal experience, is computationally indistinguishable from a biological visceral loop that we know to be accompanied by such phenomenon.

# Summary and Conclusions

Visceral loop explains why fRMI studies have shown that we become aware of a decision after its made. Because it takes extra processing cycles to consciously consider the fact of the decision being made. In short: we can only think about one thing at a time, so the decision itself and thought about the decision require separate steps.

The visceral loop can be used to explain how someone concludes themselves as conscious. It can also be used to classify the kinds of thought that occur within an agent, and the kinds of thought that it's possible for an agent to have. For example, it may be the case that simpler organisms only ever operate with Iteration 1 thought.



# References

Conant, R. C., and Ashby, W. R. (1970). Every good regulator of a system must be a model of that system. Int. J. Systems Sci., vol. 1, No. 2, pp 89-97. https://doi.org/10.1080/00207727008920220. \[[Full Text](http://pespmc1.vub.ac.be/books/Conant_Ashby.pdf)\]

Graziano, M. S. A. (2017). The Attention Schema Theory: A Foundation for Engineering Artificial Consciousnes. Front. Robot. AI. https://doi.org/10.3389/frobt.2017.00060.

Proske, U., and Gandevia, S. C. (2012). The Proprioceptive Senses: Their Roles in Signaling Body Shape, Body Position and Movement, and Muscle Force. Physiological Reviews 2012 92:4, pp 1651-1697. https://doi.org/10.1152/physrev.00048.2011.

Wernicke's area. (n.d.). In _Wikepedia_. https://en.wikipedia.org/wiki/Wernicke%27s_area. 

