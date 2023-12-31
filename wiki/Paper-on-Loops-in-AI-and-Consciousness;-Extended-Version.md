---
title: Paper on Loops in AI and Consciousness; Extended Version
layout: wiki
parent: Wiki
---

# PREPRINT DRAFT

## Title: A Characterisation of processing loops in AI and biological systems and its implications for understanding Consciousness - Extended Version

# Abstract

The claim is made that recurrent cycles of non-physical "mental" actions are required in agents that operate within complex environments, and that in order to maintain stability such actions require regulation through the use of a model. The _Visceral Loop_ is proposed as a novel framework for characterising three distinct kinds of processing within such a system in terms of how the system uses that model. It is shown how this can be used to characterise human thought, including about thought itself, and to explain the semiotic process when an individual concludes that they are conscious. A proof is given relating an upper bound on data available within access consciousness to the Visceral Loop characterisations of thought.

# Introduction

_tbd: should this be rephrased in terms of recurrency?_

Any computational system is limited in the complexity that it can handle within a single computational step. For embodied agents, this appears as a limit on the environmental complexity that they can sufficiently model and respond to within a single observe-infer-act cycle. For more complex problems, multiple iterations of processing are required in order to determine the next physical action. Such recurrency in processing may entail, for example, further analysis of the environment in order to better model its state; or consideration of alternative action plans.

In biology, this provides scope for evolutionary pressures to trade off between a more energy hungry complex brain and a simpler less energy intensive one that takes longer to make some decisions. Van Bergen & Kriegeskorte (2020) make the case that recurrency is indeed employed in biology for that very reason. A growing body of research in artificial intelligence is also now employing recurrency and is showing that complex results can be achieved with shallower networks when using recurrency, for example that of Kubilius _et al_ (2019) and Wen _et al_ (2018).

This paper makes the claim that an agent that employs _multi-step processing_ (ie: multiple cycles of processing without producing physical action) also must employ a model of its own processing capabilities in order to regulate its _non-physical actions_. Different agentive architectures support different abilities for the agent to introspect the internal structure of that model. In this paper the _Visceral Loop_, is offered as novel framework for characterising an agent's ability to introspect those models and then use them for drawing inferences about itself. 
The descriptive power of the Visceral Loop will be illustrated through three human-centric examples: i) how an individual may reach the conclusion that they are conscious, ii) providing an upper bound on the data content of consciousness, and iii) providing a new interpretation of neurobiological studies suggesting that reported awareness occurs after the act of decision making.

In the rest of this paper, the Regulation and Model sections elaborate further the need for regulatory models within any biological or artificial agent. The Schemas section suggests how this is manifested within humans in the form of a hypothesised _mind schema_. The Visceral Loop section presents the core thesis of this paper in the form of a mathematical formalism over the inferences that may be drawn from different kinds of model. The Consciousness section examines how the Visceral Loop can be applied to understanding aspects of consciousness through the presentation of the aforementioned humans. Final thoughts are presented in the Summary section.

# Regulation

An autonomous embodied agent, depending on its purpose, may need to control either its environment, itself, or both, towards some static or dynamically determined target. That agent can be described as a _regulator_ of its target system.

For example, an agent that regulates its environment operates within a system containing environment state `S_env` which changes with some ambient dynamics `D_env(t)`. The agent must perform an action, `A_env`, against the environment in order to regulate itself towards some target. After an action has been executed the environment state outcome `O_env` is influenced by both `D_env(t)` and `A_env`. This can be summarised as the following equation:

    S_env + D_env(t) + A_env = O_env

According to the _good regulator theorem_, if the agent is to regulate the environment state it must be a "model of the system" (Conant & Ashby, 1970). Furthermore, we can say that the efficiency of the agent to regulate its environment depends on its accuracy in modelling the system. Errors in the accuracy of the model result in errors in the regulation of the system. In learning agents, those errors are used for subsequent training of the model.

An embodied agent with complex actions may require an additional level of regulation. For example, an animal must not only regulate its external environment, but also regulate its own physical state. This includes both maintaining homeostasis and controlling the efficiency and effectiveness of its actions against the environment. The agent performs action `A_body` against its body with the intent to regulate the body towards efficiently achieving environment action `A_env` while satisfying its requirement for body homeostasis. Such an agent thus operates in a system that additionally has body state `S_body` with ambient dynamics `D_body(t)`. The agent performs action `A_body` against its body, producing outcome `O_body`, summarised as follows:

    S_body + D_body(t) + A_body = O_body
    
Agents that incorporate multi-step processing have a third kind of action: one that changes its internal data state without affecting its physical state. This system requires regulation for the same reasons as for environment and body, but such _non-physical_ actions do not elicit any change to `S_body` or `S_env`. Thus the agent must regulate its non-physical state `S_mind`, having ambient dynamics `D_mind(t)`. The target state in this case is dynamically inferred based on its requirement for environment action `A_env`, body action `A_body`, and possibly for some form of non-physical homeostasis of `S_mind`. In order to regulate towards that target it performs action `A_mind` producing outcome `O_mind`, summarised as follows:

    S_mind + D_mind(t) + A_mind = O_mind
    
By way of example of the importance of such mind regulation, consider the case of fluent aphasia caused by damage to the Wernicke's area of the brain (_Wernicke's area_). Individuals with fluent aphasia can easily produce speech, but it is typically full of many meaningless words and often unnecessarily long winded. Wernicke's area is associated with language comprehension. In a neurotypical individual, the comprehension of their own vocalizations provides a corrective mechanism. This illustrates the importance of feedback in the regulation of one's own actions, and by way of analogy extends to the regulation of non-physical actions.


# Models

All of the systems described above are of the form `S + D(t) + A = O`. The production of the optimal action `A` for a given situation can be computed by a function, `f`, such that `A = f(S,O,t) = O - S - D(t)`. In this way, function `f` becomes a _model_ of the system in exactly the way meant by Conant and Ashbey. There are many different ways of constructing such a function, with implications on how much its inherent model can be introspected for purposes other than merely computing the next action.

Consider the following function. This function is, for example, effective at predicting the action required to regulate towards a target state of `3` by doubling the input signal and comparing to that target state. However, an agent that merely uses this function to calculate actions cannot inspect anything about the function other than the actions it calculates for different inputs.

    f(x) = 3 - 2x
    
Alternatively, consider the following diagram, which shows an _abstract syntax tree_ (AST) of the function above, of the sort used in computer science to parse an expression within a software compiler (_Abstract syntax tree_). Instead of using the above function, a regulating agent could use this AST to calculate its next action and achieve the same outcome. However, the AST is a more explicit model of the dynamics being regulated. The components of the original function are represented individually and thus they can be individually queried. So here the AST can be introspected and much more can be derived from it that may apply either to the system being modelled or to how the AST models that system. 

![ast](files/Paper-on-Loops-in-AI-and-Consciousness-ast.png)

To examine the introspective opportunities further, consider the task of constructing a set, `F`, that contains all beliefs that may be drawn from the model. In the case of the function, pairs of input and output action values are all that can be drawn from the model, ie: `<0,3>, <2,-1>, <-3,9>, <-1,5>`, etc. The AST supports the ability to draw those same pairs of input and action values. However the AST also supports that many other beliefs may be drawn from the model and added to `F`. For example that i) the target is `3`, ii) input signal `x` is significant to the calculation, while `y` and `z` are not, and iii) the execution of the function depends on the operations of _subtraction_ and _multiplication_.

So, it is clear that different architectures enable different levels of _introspection_ of the underlying models. What about the case for neural networks? In the modern use of artificial neural networks (ANNs), it is commonplace to refer to ANNs as a _function approximator_ (Goodfellow et al., 2016), and indeed many networks fall into the category of a function. For example, in _model-free_ deep reinforcement learning (RL) an ANN is used to calculate either the next action or the expected value of all possible actions given the current state (Lazaridis, Fachantidis & Vlahavas, 2020). The architecture of the RL algorithm treats the ANN as a function without any introspective capabilities. There is also _model-based_ RL. One variant of _model-based_ RL uses ANNs to predict the expected outcome of executing an action. The introspective ability here is the same as for _model-free_ deep RL -  the ANN is treated as a function. For the RL models mentioned so far, the set `F` of beliefs is of similar content: `F` is the set of `<state,action>` or `<state,action,outcome>` tuples. There do exist forms of model-based RL that use something more akin to the AST, usually where there is a known physics model that is represented mathematically, and which could potentially be used to introspect for more than just `<state,action,outcome>` tuples. However, a significant point to note here is that ANNs, and neural networks in general, may not lend themselves naturally to introspection on their own.

For that reason, a third form of model exists, whereby a secondary model predicts the behaviours of the former. The secondary model may, for example, be a second ANN that captures aspects of the same underlying system but at a more macro level, and it may be more suitable for integration with other data. This macro representation is at the core of the theory of Higher Order Thought (Rosenthal, 1997 & 2006), and of recent theories based on it such as Hierarchical Active Inference (Giovanni _et al_, 2018) and Integrated World Modeling Theory (IWMT) (Safron, 2020).

## Schemas

The lack of introspective ability of a simple function contrasts with the introspective ability of a human. Psychology has long identified in humans the existence of a model of the individual's body - known as the _body schema_. A good definition is given by Morasso _et al_: "In summary, we view the body schema as a set of fronto-parietal networks that integrate information originating from regions of the body and external space in a way, which is functionally relevant to specific actions performed by different body parts. As such, the body schema is a representation of the body’s spatial properties, including the length of limbs and limb segments, their arrangement, the configuration of the segments in space, and the shape of the body surface" (2015). So the body schema is a model used in production of action control by integrating information from our main physical senses and the proprioceptive senses (Proske & Gandevia, 2012). That model can also be introspected - for example, we can know where our hands and feet are without seeing them - and those introspections can become the topic of subsequent thought. But there are aspects of the model that cannot be introspected - for example, we have no observability of the arrangement of the sense nerves used to infer the hand and feet positions, or of the effector nerves used to actuate their muscles.

This paper hypothesises the existence of a second kind of schema, the _mind schema_, that performs an analogous role for the regulation of the mind and non-physical actions. Anecdotally, this seems highly plausible within humans given our introspective ability towards our own mind's capabilities. For example, we can know that we are good at focussing, but struggle with maths, that we are more creative when background music is present, and that we need the support of tools to help remember people's names (eg: a notebook). The underlying notion here is that the mind schema helps us to control, monitor, predict, and rationalise about our mental structure and actions in the same way that our body schema does that for our physical structure and actions. It is the regulatory model for our non-physical actions. Additionally, just as for the body schema, there is a distinct delineation between what can be introspected and subsequently thought about, and what cannot.

The suggestion of a mind schema has also been made in the form of the _Attention Schema Theory_ (Graziano & Kastner, 2011; Webb & Graziano, 2015; Graziano, 2017), although the meaning there is perhaps narrower than what is proposed in this paper.

# Visceral Loop

This paper introduces the _Visceral Loop_ as a novel framework for the characterisation of inferences drawn by a processing loop within a biological or AI agent. The Visceral Loop is so named because it refers to an agent concluding that it experiences consciousness in a visceral way. It identifies that an agent with sufficient representational capabilities can, at the most optimum, conclude itself as conscious within three iterations of the processing loop. Each of those iterations have specific characteristics, and the Visceral Loop can be used to characterise any thought as falling into one of those three iterations.

Let:
* `E` be the agent's set of beliefs about the external world
* `B` be the agent's set of beliefs about its own physical body (drawn from the body schema) and of bodies in general, and if it has a concept of its identity then this set includes a belief that relates other body beliefs to its identity
* `M` be the agent's set of beliefs about its own mind (drawn from the mind schema) and of minds in general, and if it has a concept of its identity then this set includes a belief that relates other mind beliefs to its identity
* `f(..)` be the function executed by the agent on the specified inputs in order to draw inferences

`M` can be thought of as an agent's "theory of mind", because it relates not only to itself but also to its ability to predict the hidden mental state of others.

**Iteration 1:**

_Iteration 1_ represents the most common kind of data processing, such as spending multiple processing cycles to refine the identification of something within the visual field. While an agent's mind schema may be used to regulate the thought process, the result of Iteration 1 never makes any reference to it.

Let `x` be an inference produced as the result of a processing step, such that it does not draw any reference to `M` (ie: `x ∉ M`, and if `x` is a relation then `x = relation(α,β)` such that `α ∉ M` and `β ∉ M` and `α ⊄ M` and `β ⊄ M`). Given some sense input or past state `s`, a processing step is characterised as Visceral Loop Iteration 1 if it is of the following form:

* `f(s, E ∪ B ∪ M) -> x`

**Iteration 2:**

_Iteration 2_ processing steps draw conclusions that relate past non-physical actions and conclusions to the agent's theory of mind and to the agent's concept of its identity. For example, concluding that a past data state or non-physical action is classified as "thought", concluding whether the primary source of a past data state was external or internal, or relating the fact of an internal source to the agent's concept of its identity.

Iteration 2 requires an agent to have sufficient representational capabilities to produce inferences that represent relations involving `M`. Given some prior inference `y`, a processing step is characterised as Visceral Loop Iteration 2 if it is of the following form, and the relation with respect to `M` is non-empty, and it can not be characterised as Iteration 3:

* `f(y, E ∪ B ∪ M) -> relation(y, M)`

**Iteration 3:**

_Iteration 3_ is a special case of what would otherwise be Iteration 2, but it implies stricter requirements on the agent's introspective and representational capabilities. Iteration 3 covers the ability for the agent to develop a summary of its own mental capabilities (ie: some subset `m ⊂ M`), and to consider that in relation to its conception of mental capabilities in general or to its identity (ie: `M`). Iteration 3 is involved in an agent concluding itself as conscious, as will be seen in the section below.

Given some prior inference `relation(z, M)`, and some subset of beliefs `m ⊂ M`, a processing step is characterised as Visceral Loop _Iteration 3_ if it is of the following form and the relation with respect to `M` is non-empty:

* `f(relation(z, M), E ∪ B ∪ M) -> relation(m, M)`

# Consciousness

In the consideration of conscious experience, two closely incident but distinct forms have been identified:

* _Access consciousness_ (A-Cs) refers to state representations that are "(1) inferentially
promiscuous, that is, poised for use as a premise in reasoning, (2) poised for rational control of action, and (3) poised for rational control of speech." (Block, 1995). In other words, A-Cs is the data content that has a direct influence on subsequent thought. For example, generally the data content of access consciousness can be directly consciously thought about and reported on via speech or other actions; although research suggests that some information can influence our subsequent thought without us being aware of it, such as in the example of blindsight (Block, 1995).

* _Phenomenal consciousness_ (P-Cs) refers to the question of why a physical bundle of matter should have a subjective experience anything at all. It is often described as "what it is like" (Nagel, 1974) to be a conscious organism. In approximate terms, P-Cs is the phenomenal aspect of having experience of access consciousness. Some authors believe that there is not an exact one-to-one relation between A-Cs and P-Cs; that, while they largely correlate, one can have P-Cs without A-Cs, and vice versa. That remains an open question, for which this paper does not attempt to address.

_tbd: need to revise following section if don't manage to split A-Cs and P-Cs in theory section._

The Visceral Loop has implications for understanding consciousness, particularly in terms of A-Cs. As will be seen, based on the Visceral Loop, one can make a strong argument that associates the behaviours of the underlying modelling mechanism to limits on the ability for self-reference and to the ability for an individual to recognise their own consciousness. In a weaker form that can be related to the content of P-Cs.

To avoid confusion in the sections that follow, this paper uses the term "data content" when talking about both A-Cs and P-Cs. In that context, it is used to draw a distinction between what is present or included within A-Cs or P-Cs, respectively, and what is not. For example whether or not someone can see and report on something within their visual field refers to the data content of A-Cs, and whether or not someone phenomenally experiences pain refers to the data content of P-Cs.

What follows are three examples of the descriptive power of the Visceral Loop applied to consciousness.

## Concluding oneself as conscious

In this first example, the Visceral Loop is applied to understand the thought processes whereby an individual concludes themselves as conscious. Consider the following sequence of internal mental observations:
1. "What's that red blob in the tree? Oh, it's an apple".
2. "Those thoughts just came from my mind, and not from the outside world".
3. "That's what consciousness is. I am conscious".

The first observation is a straightforward example of Iteration 1 that does not make any reference to the agent's theory of mind (of their own mind or of others). The concepts of "red", "blob", "tree" and "apple" are all contained within the set `E`, and thus the inference in relation to the visual field sense input `s` is of the form `x_1 = relation(s, E)`.

The second observation contains two examples of Iteration 2 inferences. In the first, the individual's processing capabilities have selected attentional focus upon the prior Iteration 1 inference, and have drawn a subsequent inference about it as being data that can be classified as a "thought". As beliefs about "thought" are contained within `M`, this is an inference of the form `x_2 = relation(x_1, M)`. In the second, the individual draws a subsequent inference about the source of the Iteration 1 inference as being their own mind. The individual's ability to classify inferences in relation to themselves also depends upon `M`, and the inference is of the form `x_3 = relation(x_1, M)`.

The third observation draws upon the individual having an _a priori_ conception about consciousness in general, denoted here by `m_c ⊂ M`. The individual compares its prior Iteration 2 inferences `x_2` and `x_3` to `m_c`, and produces an inference that `x_2` and `x_3` together satisfy the requirements for consciousness. This is another iteration 2 inference of the form `x_4 = relation(x_2 & x_3, m_c)`. Finally, the individual relates `m_c`, the belief of consciousness in general, to itself, which again depends on `M`. That final inference is thus an Iteration 3 inference in the form `x_5 = relation(m_c, M)`.

## Content of conscious thought

As a second example of the descriptive power of the Visceral Loop, a set of theorems is now presented that makes the claim that the Visceral Loop explains the data content of conscious experience. Later analysis discusses some shortcomings with the theory.

_TBD: try focussing on A-Cs only first, and then later do another theory for P-Cs. Otherwise will have to revise this section anyway to be more honest about the axiomatic baseline not being sufficiently inline with current research and theories_.


First an axiomatic baseline must be established. The author is unable to think of any rational way in which they may consciously experience something and yet be unable to subsequently think about that experience and to know that they are thinking about that experience. Indeed, this is consistent with the _transitivity principle_ of Rosenthal (1997). Thus, it would seem that being able to knowingly think about our conscious experiences is a fundamental component of consciousness. The following claims are derived from this statement without further proof:

Claim 1:
* All conscious experience is subsequently available for further thought.

Claim 2:
* For all thought about conscious experience, the individual can identify that thought as being their own.

Note that these claims do not assume that all conscious experience is actually thought about; only that it is in principle available for such thought.

Theorem 1:
* the content of conscious experience is upper bounded by the data about which Visceral Loop iteration 2 inferences can be produced.

Proof:
* The _content of conscious experience_ here refers to the set of data represented and/or processed within the brain which is consciously experienced by that individual, in distinction to other data represented and/or processed in the brain which is not consciously experienced.
* Thought is a computational process, and thus is a series of inferences.
* As per claim 1, all of conscious experience must be available for producing subsequent inferences about those conscious experiences.
* As per claim 2, the individual must be able to identify that they produced those inferences.
* In order for an individual to identify an inference as being their own, they must have some beliefs about their inference capabilities and how they relate to themselves as an individual entity. This is included in the set `M`, which iteration 2 produces inferences in relation to, and which is not directly accessible for inferences within iteration 1.
* Imagine some supposed experience, and an inference `i` produced about that experience. Additionally imagine that an iteration 2 inference cannot be produced about `i`, for example, due to some incompatibility of structure, lack of data path to iteration 2 processing capabilities, or inherent limitation in iteration 2 processing capabilities. The inference `i` cannot be identified in relation to the individual. As such, the supposed experience fails on Claim 2 and `i` must be in actual fact an inference about some sort of non-conscious experience.
* Thus, an experience is not a conscious experience if it can only lead to inferences which cannot be included in an iteration 2 inference.

## Delayed awareness of decisions

The Visceral Loop can be used to understand other aspects of thought. For example, fRMI and EEG studies have suggested that we become aware of a decision after it is made (Soon _et al_, 2008; Libet _et al_, 1983). At first glance this might seem to suggest that our conscious thought is just some sort of after-the-fact passive summarisation.

The framework of the Visceral Loop provides a different interpretation. It explains that the act of making a decision and the conscious consideration of having made that decision occur in different processing cycles. First one or more processing cycles are used to reach the decision, and subsequently the individual may use one or more additional processing cycles to examine their most recent inference in relation to themselves. So it is entirely predictable that the individual would activate brain regions for reporting the decision after a measurable delay from the decision itself being made and a resultant action initiated. Importantly, the same underlying system can produce both sets of processing cycles, and thus there is no reason to conclude that consciousness has no causal effect in the actions initiated.

In short, we can only think about one thing at a time, so the decision itself and thought about the decision require separate processing steps.

# Analysis

The examples above show that it is possible to mathematically reason about thought processes, their sequencing, and what can/cannot be thought about depending on the capabilities of the underlying thought processing system. This section examines the Visceral Loop (VL) against some existing theory.

The VL views thought as a _biosemiotic process_. Semiotics is the study of signs and their interpretations, and biosemiotics looks at how semiotics plays out within biology, including neural cognition. A semiotic process has three components: a _referent_, the object for which a sign or representation will be made; a _representamen_, which is a representation of the _referent_, a.k.a. a "sign"; and a _interpretant_, the interpretation made from the _representamen_.  The _intepretant_ may or may not accurately reflect the original _referent_, depending on the quality of _representamen_ and on the ability of the system to infer information about the _referent_ from the _representamen_. From an external point of view, the brain acts as a semiotic process against the environment. The environment is the _referent_, with a concrete and actual state that the brain does not have direct awareness of. Instead, the brain uses the physical senses as a _representamen_ of that environment, and from that representation produces an _interpretant_. The VL is interested in a more internal semiotic process within the brain. The _interpretant_ from before must itself be encoded in a representation that is subject to the constraints imposed by the specific characteristics of the underlying biological substrate. In order for the brain to subsequently use that representation, it must decode its meaning. Thus an inner semiotic process is activated, where the prior inference becomes the _referent_, which is encoded as a _representamen_, and subsequently decoded as a new _interpretant_, possibly after combining with additional information from other sources.

The semiotic interpretation of cognition is important for a number of reasons. Firstly, it explains that a data state is meaningless without a process that interprets that data state - even if the process generated the data state in the first place, that data state is still meaningless to the process without re-interpreting it. Thus, while the brain must include considerable machinery for the interpretation of external stimuli, it must also include considerable machinery for the interpretation of its own outputs. The VL builds on this by describing the kinds of interpretations that may be generated depending on the what information is available within the _representamen_ and on the capabilities of the process.
	- citation: https://en.wikipedia.org/wiki/Semiotics, Pearce.

Thus, the biosemiotic process of the VL within an individual (with the specific representations that are possible within that process) form the individual's _Umwelt_ (citation, Uexküll plus correction paper) - the aggregate representation of the individual's external and internal world, constructed within their mind, and available to the individual's consciousness.

The VL and the biosemiotic process that it operates upon examine thought at a high-level, but the VL does not presuppose a particular physical or computational structure. In that sense it is applicable to many theories of cognition and brain function. However, it is most consistent with other theories that also examine thought at a high-level or provide theories about the underlying mechanims of such high-level thought. For example, those of Higher-Order Thought Theory, and Global Workspace Theory.

Higher-Order Thought Theory (HOTT) describes mental processes as hierarchical. In HOTT, consciousness forms the highest layer of the hierarchy, and has access to the output from the immediate layer below, but not of further lower layers. Thus the information available for conscious thought is a unified high level abstract representation of many sub-processes. The VL does not require a HOTT architecture, but it explains how a HOTT architecture results in the specific nature of human experience in terms of what internal processes are and are not directly observable.

_tbd: The Visceral Loop is consistent with Global Workspace Theory (citation), and Higher-Order Thought Theory of Rosenthal (1997, 2006)._

_tbd: predictive coding, active inference, and world modelling?_

# Summary

As bemoaned by Colograsso & Mozer (2004), in the fields attempting to understand consciousness, solid computational models are rare. The work presented here has implications for understanding consciousness, for the design of AI systems, and perhaps forms one of the necessary building blocks towards artificial general intelligence (AGI).

_tbd: above needs work._

This paper makes the claim that agents operating within complex environments and with complex bodies require a trade-off between the inferential computing power of a single processing step versus the use of multiple iterations of a recurrent processing loop. In order to be a "good regulator" of its own non-physical actions, the agent must model its non-physical behaviours. Various different forms of such modelling are possible, and the characterisations offered by the Visceral Loop provide an insight into what kinds of self-referential thought are possible depending on the kind of model in use.


_tbd: Further work would be to phrase the Visceral Loop in the terms of predictive coding (Seth, Suzuki, & Critchley, 2012; Millidge, Seth, Buckley, 2021)_

_tbd: The Visceral Loop has been shown to offer significant insight into consciousness. More work is possible here. It should be noted that there are aspects of consciousness that the Visceral Loop makes no claim over. In particular, it offers no explanation for the so called "hard problem" of phenomenal consciousness (Chalmers, 1995) - the "what it feels like" aspect of consciousness. However, the author believes that stronger claims about the natures of both access consciousness and phenomenal consciousness can yet be made, based on the framework of the Visceral Loop._

# References

Abstract syntax tree (n.d.). In _Wikepedia_. In https://en.wikipedia.org/wiki/Abstract_syntax_tree

Block, N. (1995). On a confusion about a function of consciousness. Brain and Behavioral Sciences, 18(2), pp 227–247. https://doi.org/10.1017/S0140525X00038188. \[[Full Text](https://www.nyu.edu/gsas/dept/philo/faculty/block/papers/1995_Function.pdf)\]

Chalmers, D. J. (1995). Facing up to the problem of consciousness. Journal of Consciousness Studies 2(3): pp 200-19. http://dx.doi.org/10.1093/acprof:oso/9780195311105.003.0001. \[[Full Text](http://consc.net/papers/facing.pdf)\]

Colagrosso, M. D., and Mozer, M. C. (2004). Theories Of Access Consciousness. NIPS 2004. \[[Full Text](https://proceedings.neurips.cc/paper/2004/file/ff2cc3b8c7caeaa068f2abbc234583f5-Paper.pdf)\]

Conant, R. C., and Ashby, W. R. (1970). Every good regulator of a system must be a model of that system. Int. J. Systems Sci., vol. 1, No. 2, pp 89-97. https://doi.org/10.1080/00207727008920220. \[[Full Text](http://pespmc1.vub.ac.be/books/Conant_Ashby.pdf)\]

Giovanni, P., Rigoli, F., Friston, K. J. (2018). Hierarchical Active Inference: A Theory of Motivated Control. Trends in Cognitive Sciences, Volume 22, Issue 4, 294 - 306. https://doi.org/10.1016/j.tics.2018.01.009

Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep learning. MIT Press.

Graziano, M. S. A., and Kastner, S. (2011). Human consciousness and its relationship to social neuroscience: a novel hypothesis. Cogn. Neurosci. 2, 98–113. doi:10.1080/17588928.2011.565121

Graziano, M. S. A. (2017). The Attention Schema Theory: A Foundation for Engineering Artificial Consciousnes. Front. Robot. AI. https://doi.org/10.3389/frobt.2017.00060.

Kubilius, J., Schrimpf, M., Kar, K., Rajalingham, R., Hong, H., Majaj, N., Issa, E., Bashivan, P., Prescott-Roy, J., Schmidt, K., Nayebi, A., Bear, D., Yamins, D. L., DiCarlo, J.J. (2019). Brain-like object recognition with high-performing shallow recurrent anns. Advances in Neural Information Processing Systems, pp. 12805-12816. https://papers.nips.cc/paper/2019/hash/7813d1590d28a7dd372ad54b5d29d033-Abstract.html.

Lazaridis, A., Fachantidis, A., & Vlahavas, I. (2020). Deep Reinforcement Learning: A State-of-the-Art Walkthrough. J. Artif. Intell. Res., 69, 1421-1471. https://doi.org/10.1613/jair.1.12412. \[[Full Text](https://jair.org/index.php/jair/article/view/12412/26638)\]

Libet, B., Gleason, C. A., Wright, E. W., & Pearl, D. K. (1983). Time of conscious intention to act in relation to onset of cerebral activity (readiness-potential). The unconscious initiation of a freely voluntary act. Brain : a journal of neurology, 106 (Pt 3), 623–642. https://doi.org/10.1093/brain/106.3.623. \[[Full Text](https://www.researchgate.net/publication/16556603_Time_of_Conscious_Intention_to_Act_in_Relation_to_Onset_of_Cerebral_Activity_Readiness-Potential_The_Unconscious_Initiation_of_a_Freely_Voluntary_Act)\]

Millidge, B., Seth, A., Buckley, C. L. Predictive Coding: a Theoretical and Experimental Review. https://arxiv.org/abs/2107.12979

Morasso, P., Casadio, M., Mohan, V., Rea, F., and Zenzeri, J. (2015). Revisiting the body-schema concept in the context of whole-body postural-focal dynamics. Front. Hum. Neurosci. 9:83. https://doi.org/10.3389/fnhum.2015.00083

Nagel, T. (1974). What Is It Like to Be a Bat?. The Philosophical Review, 83(4), 435–450. https://doi.org/10.2307/2183914. \[[Full Text](https://warwick.ac.uk/fac/cross_fac/iatl/study/ugmodules/humananimalstudies/lectures/32/nagel_bat.pdf)\]

Proske, U., and Gandevia, S. C. (2012). The Proprioceptive Senses: Their Roles in Signaling Body Shape, Body Position and Movement, and Muscle Force. Physiological Reviews 2012 92:4, pp 1651-1697. https://doi.org/10.1152/physrev.00048.2011.

Rosenthal, D. M. (1997). A Theory of Consciousness. In N. Block, O. Flanagan, & G. Güzeldere (Eds.), _The Nature of Consciousness: Philosophical Debates_ (pp. 729-753). Cambridge, Massachusetts: MIT Press/Bradford Books. \[[Full Text](https://www.davidrosenthal.org/DR-A-Theory.pdf)\]

Rosenthal, D. (2006). Consciousness and Higher‐Order Thought. https://doi.org/10.1002/0470018860.s00149.

Safron A. (2020). An Integrated World Modeling Theory (IWMT) of Consciousness: Combining Integrated Information and Global Neuronal Workspace Theories With the Free Energy Principle and Active Inference Framework; Toward Solving the Hard Problem and Characterizing Agentic Causation. Frontiers in artificial intelligence, 3, 30. https://doi.org/10.3389/frai.2020.00030

Seth AK, Suzuki K and Critchley HD (2012) An interoceptive predictive coding model of conscious presence. Front. Psychology 2:395. doi: 10.3389/fpsyg.2011.00395

Soon, C. S., Brass, M., Heinze, H. J., & Haynes, J. D. (2008). Unconscious determinants of free decisions in the human brain. Nature neuroscience, 11(5), 543–545. https://doi.org/10.1038/nn.2112. \[[Full Text](https://www.researchgate.net/publication/5443390_Unconscious_determinants_of_free_decisions_in_the_human_brain)/]

van Bergen, R. S., Kriegeskorte, N. (2020). Going in circles is the way forward: the role of recurrence in visual inference, Current Opinion in Neurobiology, Volume 65, Pages 176-193, ISSN 0959-4388, https://doi.org/10.1016/j.conb.2020.11.009

Webb, T. W., and Graziano, M. S. A. (2015). The attention schema theory: a mechanistic account of subjective awareness. Front. Psychol. 6:500. doi:10.3389/fpsyg.2015.00500

Wen, H., Han, K., Shi, J., Zhang, Y., Culurciello, E., Liu, Z. (2018). Deep predictive coding network for object recognition. https://arxiv.org/abs/1802.04762. https://proceedings.mlr.press/v80/wen18a.html

Wernicke's area. (n.d.). In _Wikepedia_. https://en.wikipedia.org/wiki/Wernicke%27s_area
