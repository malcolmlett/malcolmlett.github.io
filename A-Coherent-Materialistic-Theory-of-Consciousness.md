_This is a work in progress._

_Please come back later._

Abstract:
- Consciousness is produced by a semiotic multi-step planner state machine with meta management. 

Contents:

* [Part I - Introduction](#part-i--introduction)
* [I.1 A Question of Consciousness](#i1-a-question-of-consciousness)
* [I.2 Summary of Thesis](#i2-summary-of-thesis)
* [I.3 Background - Theories of Consciousness](#i3-background--theories-of-consciousness)
  * [A point of Central Unification?](#a-point-of-central-unification)
* [I.4 Background - Biology and Neuroscience ](#i4-background--biology-and-neuroscience-)
* [Part II - Problems in Simple Synthetic Control Processes](#part-ii--problems-in-simple-synthetic-control-processes)
* [II.1 Interlude: Environment, Body, and Control Processes (first part)](#ii1-interlude-environment-body-and-control-processes-first-part)
* [II.2 Complexity and the need for Processing Loops](#ii2-complexity-and-the-need-for-processing-loops)
* [II.3 State Trajectories in a Multi-iteration Processor](#ii3-state-trajectories-in-a-multiiteration-processor)
* [Part III - Problems in Complex Synthetic Control Processes](#part-iii--problems-in-complex-synthetic-control-processes)
* [III.1 Meta-management in Deliberative Systems](#iii1-metamanagement-in-deliberative-systems)
  * [State Trajectory Control during Body Action](#state-trajectory-control-during-body-action)
  * [State Trajectory Control during Multi-iteration Processing](#state-trajectory-control-during-multiiteration-processing)
  * [State Trajectory Control during Iterative Inference](#state-trajectory-control-during-iterative-inference)
  * [State trajectory control in summary](#state-trajectory-control-in-summary)
  * [Objective learning](#objective-learning)
  * [Mode control](#mode-control)
  * [Mode identification](#mode-identification)
  * [Distributed cooperation](#distributed-cooperation)
  * [Certainty measurement / reaction](#certainty-measurement--reaction)
* [III.2 Interlude: Mechanisms of Standard Control Processes](#iii2-interlude-mechanisms-of-standard-control-processes)
  * [Stateless reactive control process](#stateless-reactive-control-process)
  * [Stateful reactive control process](#stateful-reactive-control-process)
  * [Planning control process](#planning-control-process)
  * [Expectation-Maximisation / Iterative Convergent Control Processes](#expectationmaximisation--iterative-convergent-control-processes)
  * [Hand-written Control Processes in AI vs Biologically Plausible Control](#handwritten-control-processes-in-ai-vs-biologically-plausible-control)
  * [A Biologically Plausible Planning Control Process](#a-biologically-plausible-planning-control-process)
* [III.3 Meta-control Options in Meta-management](#iii3-metacontrol-options-in-metamanagement)
* [III.4 Meta-observation Options in Meta-Management](#iii4-metaobservation-options-in-metamanagement)
* [III.5 Architectural Options for Meta-management](#iii5-architectural-options-for-metamanagement)
  * [Implicit Meta-management](#implicit-metamanagement)
  * [Independent Meta-management](#independent-metamanagement)
  * [Inline Meta-management](#inline-metamanagement)
  * [Chapter Summary](#chapter-summary)
* [Part IV - Problems in Biological Control Processes](#part-iv--problems-in-biological-control-processes)
* [IV.1 Interlude: Environment, Body, and Cognitive Processes](#iv1-interlude-environment-body-and-cognitive-processes)
  * [Classification](#classification)
  * [System Interactions](#system-interactions)
  * [Markov Process Modelling](#markov-process-modelling)
  * [Identification of Source](#identification-of-source)
  * [Schema](#schema)
  * [The Ego in "I"](#the-ego-in-i)
  * [Emotions](#emotions)
  * [Meaning Attachment](#meaning-attachment)
* [IV.3 Deeper Dive into Control Process Learning](#iv3-deeper-dive-into-control-process-learning)
  * [Innate Control](#innate-control)
  * [Habitual Standard Control](#habitual-standard-control)
  * [Rational Standard Control Management](#rational-standard-control-management)
  * [Habitual and Rational Control operating together](#habitual-and-rational-control-operating-together)
* [IV.4 Deeper Dive into Meta-management](#iv4-deeper-dive-into-metamanagement)
  * [Components of Habitual and Rational Meta-management](#components-of-habitual-and-rational-metamanagement)
  * [Reusable Domain Knowledge](#reusable-domain-knowledge)
  * [Summary of Meta-management Architecture](#summary-of-metamanagement-architecture)
* [IV.4 Distinguishing Meta-management from Standard Control](#iv4-distinguishing-metamanagement-from-standard-control)
  * [State Representation](#state-representation)
  * [Pathways](#pathways)
  * [Learning](#learning)
* [IV.5 Semiotics](#iv5-semiotics)
  * [Objects, Representations, and Interpretations](#objects-representations-and-interpretations)
  * [Infinite semiosis](#infinite-semiosis)
  * [Semiotic Analysis of Control Processes](#semiotic-analysis-of-control-processes)
    * [Body action control](#body-action-control)
    * [Meta-management of CP state trajectory](#metamanagement-of-cp-state-trajectory)
    * [Meta-learning](#metalearning)
    * [Summary](#summary)
  * [Trains of Thought](#trains-of-thought)
* [Part V - Solution](#part-v--solution)
* [V.1 The Architecture of Subjective Experience](#v1-the-architecture-of-subjective-experience)
* [V.2 Subjective Experience State](#v2-subjective-experience-state)
* [V.3 Interpretation of Subjective Experience States](#v3-interpretation-of-subjective-experience-states)
* [V.4 The Properties of Subjective Experience](#v4-the-properties-of-subjective-experience)
  * [Homonculous](#homonculous)
  * [Conscious and Unconscious Thought](#conscious-and-unconscious-thought)
  * [Subjective experience is "always on"](#subjective-experience-is-always-on)
* [V.5 Sufficient Conditions of Subjective Experience](#v5-sufficient-conditions-of-subjective-experience)
  * [MM feedback loop](#mm-feedback-loop)
  * [inline mm architecture](#inline-mm-architecture)
  * [iterative processing](#iterative-processing)
  * [representational and processing capacity](#representational-and-processing-capacity)
  * [topic attenuation avoidance](#topic-attenuation-avoidance)
  * [attention](#attention)
  * [modelling](#modelling)
  * [meaning attachment](#meaning-attachment)
  * [Conditions for evolution of Subject Experience](#conditions-for-evolution-of-subject-experience)
* [V.6 Necessary and Sufficient Conditions of Subjective Experience](#v6-necessary-and-sufficient-conditions-of-subjective-experience)
* [Part VI - The Intuitional Gap](#part-vi--the-intuitional-gap)
* [Part VII - Predictions](#part-vii--predictions)
  * [Convergence of Meta-Management](#convergence-of-metamanagement)
  * [Does it exist?](#does-it-exist)
* [Part VII - Next Steps](#part-vii--next-steps)
* [References](#references)

---

# Part I - Introduction

# I.1 A Question of Consciousness

It has been said that the field of neuroscience is data rich, and theory poor. While vast quantities of data are available from the nature of individual neurons to the activity of the brain as a whole, we lack functional theories of cognitive function in order to make sense of that data. While theories exist, they are just not detailed enough [citation, and fleshing out].

That problem is no less poignant for the question of consciousness. What is the basis of consciousness? It's underlying mechanisms? What makes one thing conscious, while another is not? What is this ethereal "something other" that seems to be associated with conscious experience - the "what it feels like" to be conscious [citation, nagal]? We have ample information about so called _correlates of consciousness_ - neurological data about high level brain activity at the time of conscious experience. But we lack an effective functional theory to compare that activity against. While many _theories of consciousness_ (TOC) exist, they lack the details needed to sufficiently explain the neurological data ..._todo: needs some more precise wording_.

One particular attribute of interest is best explained through contrast. When we look at a rock rolling down a hill, many of us would imagine that the rock has no experience of itself or of its current activity in rolling. The rock has nothing in its physical makeup that could behave like neurons, and thus no capability for computational or cognitive processing of any sort in order to capture its state and activity, nor to consider that state and activity. Many who have belief in some kind of spiritual reality also do not imagine the rock to have a form of spirit that could comprehend or somehow sense its existence. In the short, the rock is both not alive and not aware.

A plant is alive. Furthermore, a plant can react to its environment. But again many of us would imagine that the plant produces its reactions without any real "awareness" of what happens to it and what it does in response. Instead, we imagine that the plant is an entirely (bio-chemical) mechanical process that just operates its mechanics as is.

Contrast that to humans. We have some sort of internal experience of the things that happen to us, of the things we do in response, and of and the thoughts that swim around our brain while all of that is happening. That internal experience is variously referred to as _phenomenal consciousness_ [citations] and _subjective experience_ [citations]..._todo: any other terms?_. I shall use the term _subjective experience_ in a hope to avoid some of the debate associated with other terms. What is peculiar about subjective experience is that despite hundreds of years of theorising [citation], we cannot explain a) what the underlying processes are that produce subjective experience, nor b) why we might have subjective experience in the first place.

Chalmers makes the claim that no physical property, mechanical or computational process known to us today can explain subjective experience [citation], and the issue has become known as the _Hard Problem of Consciousness_. This problem is so "hard", that it has led many, Chalmers included, to pose non-materialistic theories: theories that incorporate some form of reality outside of what we can measure through physical means.

This article is interested in resolving that most perplexing question of consciousness. I present the case that subjective experience can be fully explained through materialistic means. Not only that, I present a theory that explains _why_ and _how_ subjective experience occurs - the underlying mechanisms of subjective experience.

The theory presented here provides an opportunity for testing against empirical evidence. .....


The theory presented is compatible with ...._todo: HOT, IIT, competition theories....._ In fact, many of the ideas presented here are not new. But I believe this to be the most comprehensive attempt to combine ideas together at the most detailed level. I suspect that in many respects, a key skill of anyone doing research in this area is to sieve through the many partial stories and see how they can be linked together.

# I.2 Summary of Thesis

I believe that three things go hand-in-hand: general intelligence, meta-management, and consciousness. Further, understanding these systems must proceed in that order. Thus, in order to understand why we have subjective experience, we need to begin to develop a theory of general intelligence and of the processes that restrain it from cascading into chaos. This article presents an end-to-end argument following that thread.

To save the impatient reader from the tedium of waiting till the end, the entire argument is first presented here in brief. Background explanations and some definitions are omitted for the sake of brevity. The rest of the article is devoted to detailed explanations of each of the logical steps in the argument thread here.

Any computational system is limited in the complexity that it can handle within a single execution of its computational process. For embodied agents, this appears as a limit on the environmental complexity that they can sufficiently model and respond to within a single executional iteration. For more complex problems, multiple iterations of processing are required in order to determine the next physical action. Such recurrency in processing may for example entail further analysis of the environment in order to better model its state; or consideration of alternative action plans. In biology, this provides scope for evolutionary pressures to trade off between a more energy hungry complex brain and a simpler less energy intensive one that takes longer to make some decisions. Van Bergen & Kriegeskorte (2020) make the case that recurrency is indeed employed in biology for that very reason.

During the execution of a _multi-iteration_ controller within an embodied agent, its control process (CP) passes through an internal state trajectory that is only occasionally associated with interaction with the physical environment. That internal state trajectory can become increasingly disassociated with the physical environment the more complex the problem space and the longer time required for deliberation. If the multi-iteration processor must also learn through reinforcement then it is likely to exhibit chaotic and unproductive behaviour, particularly so during the earliest stages of learning. Reinforcement from the environment may be too sparse for efficient learning to take place, and simple rules that penalise longer deliberation time may be insufficiently advanced to cater for the complexity of problem domains that the agent may be faced with. Explicit meta-management processes are required to observe the control process, to model its behaviours, to track its success rate, to act upon it to prevent chaotic behaviours that could harm the agent, and to participate in providing rewards and penalties with more advanced problem-domain aware knowledge than just a simple penalty for deliberation time.

In a complex biological brain that can operate its body effectively within the real world, including all the complexity of modern human life, the systems and processes required to model and understand the environment and to interact with them are immense. It turns out that the systems required to effectively carry out meta-management are similarly complex. More importantly, the systems required for meta-management are similar to those required for primary control: observing, modelling, inference, planning, sequencing, controlling. Additionally, the domain knowledge required by the meta-management process in order to effectively meta-manage the control process is often strongly associated with the domain knowledge employed by the primary control process at the time. The level of overlap between primary control and meta-management implies a radical solution: that the control process meta-manages itself.

In order to meta-manage itself, the control process needs to observe itself. This can be achieved through a _meta-management feedback loop_ that observes the state of the control process, observes the recent trajectory of the control process, distils that into a high-order representation with lower dimensionality, and makes it available to the control process as a sensory input signal. Thus, the fact that we have awareness of some aspect of our own mental state is a direct result of the need for meta-management. And that meta-management feedback loop is a 6th sense.

The existence of the meta-management feedback loop does not alone explain subjective experience. Two more ingredients are required: interpretation and meaning. In a complex organism such as a human being, the brain maintains _schema_ that represent and track the characteristics of different aspects of the individual. This includes the body schema, which models and tracks the location and orientation of the limbs, their abilities, and whether any injuries have been acquired. This includes schema about regularly encountered external things, such as is required to mentally track the location and orientation of the wheels while driving a car over potholes. With the introduction of the meta-management feedback loop, this also includes schema for tracking the state and capabilities of the mind. And, importantly, it includes a strongly developed sense of self vs other. All external and internal sensory inputs (including the meta-management feedback loop), all schema states, are labelled as to their source. Different source labels imply significantly different meaning in terms of, for example, the level to which the agent can affect that state.

External sensory inputs, meaning association, and feedback loop together are interpreted by the brain and a decision made about the next action. Information about that action and/or the mental state that produced it is available via the feedback loop in the next iteration of processing. This creates a continuous cyclic stream of ever changing inputs, states and actions. As the control process decides to perform some body action, knowledge of that chosen action is immediately available as a sensory input before the action is even started. As the control process chooses to deliberate further on a problem at hand, knowledge of that deliberation and is immediately available. At every moment in time, the control process can choose to attend to external matters, to continuation of the current deliberation problem at hand, or to the very feedback sense that it receives continuously while it is usually distracted doing other things. If the control process stops to consider its own feedback sense, compares that to memory of recent deliberations, compares that to its schema of self vs other, it necessarily concludes that it has its own "stream of thought". That stream of thought is subjective experience.

The metaphor of a _philosophical zombie_ was introduced to hypothesise a human-like individual that has all the behavioural characteristics of a human, including voicing that it is conscious, without actually experiencing subjective experience. A philosophical zombie is _behaviourally indistinguishable_ from a human with consciousness. I argue that, if the zombie employs the mechanisms given in the explanation above (and outlined in more detail in the chapters that follow), then it is also _computationally indistinguishable_ from a human with consciousness. In other words, if we were to assume an ability to tap into all of the inner state and workings of a brain, and if we were to compare the philosophical zombie from the conscious human, we would find no difference. At that point I argue that the zombie is not a zombie after all, but instead is a fully conscious human being having subjective experience.

Finally, I argue that our disgruntlement with such an explanation is not an _explanatory gap_ [citation], but an _intuitional gap_. Nagal famously pointed out that we have no conception of and no way of developing a conception of what it is like to be anything other than ourselves [citation]  [is the 'no way of developing a conception' reference due to 'The Harder Problem of Consciousness'?]. But that does not stop us making assumptions about what should and should not experience subjective experience. It took us a very long time to accept that animals could have any form of consciousness and subjective experience, and likely many still deny that outcome [details, citations]. If we have no way to conceive of the experience held by an animal, why should we be so adamant about its properties? The answer simply is our deluded intuition. Our brains excel at finding patterns and extrapolating from them. This works well when the physical environment around us is there to provide an error signal. But when no error signal is available, we are prone to delusion. Our minds create such a strong sense of self vs other by keying that information into every sensory signal that we ever receive, so that our senses seem to take on an extra quality of realness, of subjectiveness, of _qualia_ [citation]. That seeming extra quality is further processed by the same system that produced it, reinforcing the delusion that the qualia is something extra, beyond mere sensory information. And thus we are deluded into the intuition that subjective experience is somehow more than can be produced by mere computational processing.


# I.3 Background - Theories of Consciousness
Many theories exist about the nature of consciousness. A summary of such theories will be given here.

_todo later: extend out as suitable intro for someone totally new to the question._


To provide some uniformity, the explanatory framework of a stack of theoretical layers is used, illustrated in the following diagram. Here, the physical biology of the brain is viewed as a substrate that might potentially be replaced or emulated via some other substrate (eg: silicon neurons). Built upon that substrate are many non-conscious processes. Either directly from the underlying substrate, or as a result of the non-conscious processes, some mental states are associated with subjective experience. The blue boxes represent potential layers involved in that subjective experience. For example, some non-conscious processes may produce representations that are associated with subjective experience. Such representations may or may not require specific functional structures in order to lead to subjective experience. Additionally, even with appropriate functional structures, something extra special may or may not be needed in order for those representations to be associated with subjective experience.

![theory layers](files/A-coherent-theory-v1-theory-layers.drawio.png)

* _**Layers common to many theories of consciousness.** Theories of consciousness can be discussed in terms of which of these stacked layers that they focus on. Many theories focus on just one of these layers_

**Substrate:** Everything is constructed within a physical substrate such as biological neurons. Identity Theory posits that there may be something special about biological neurons that give rise to subjective experience; or in other words, that functional isomorphisms of biological neurons such as silicon neurons or computer simulated neurons will never produce subjective experience. Inspired by the peculiar behaviour of quantum mechanics, some have suggested that the physical substrate produces quantum entanglement and that this quantum entanglement may be the underlying mechanism behind subjective experience, such as  ...{insert name of Microtubules theory}.... Such theories are quiet on which of the other layers are required. Those theories bare some similarity to that of Pan-Psychism, the theory that consciousness is fundamental in the same way that physical forces and energies are fundamental. Under Pan-psychism, some non-conscious processes lead directly to subjective experience with pan-psychist properties providing the "something special" without necessarily requiring specific representations or functional structures. However, pan-psychism is unable to explain why only certain processes are associated with subjective experience while others are not. An obvious explanation would be to require that only certain representations and associated functional structures are sufficient to "combine" the conscious properties of independent neurons / molecules / atoms, but this still leads many open questions about what those representations and/or functional structures might be that have such a power over this underlying fundamental consciousness.

**Non-conscious processes:** Many processes operate that neither directly nor indirectly lead to any kind of conscious subjective experience. While earlier work assumed that most brain processes are conscious, there is increasingly strong evidence that almost all mental processes are non-conscious, even for mental processes that are associated with attentive subjective experience. The furthest logical extension is that of epi-phenomenalism which posits that no functional mental processes are associated with subjective experience. Rather, subjective experience is posited as being some sort of non-causal summary of internal and external events. A significant problem with epi-phenomenalism is why subjective experience, and indeed consciousness at all, would have evolved if it can provide no functional / causal benefit to the individual. In that sense, epi-phenomenalism only makes any sense if viewed in conjunction with pas-psychism or with metaphysical dualistic theories where some "spirit" that exists on another plane of reality are perceiving the experiences for some grander purpose outside of the context of the corporeal reality.
- References: https://www.britannica.com/topic/philosophy-of-mind/Qualitative-states

**Representation:** Under Computational Representation Theories of Consciousness, some of those non-conscious processes produce representations that are associated with subjective experience. Debates within this area are about the kinds of these representations. For example, the intransitive vs transitive debate questions whether it is sufficient that a representation is simply held in attention or whether the representation must be in relation to the individual.......{needs work and better tie-back to actual theories}....
- References: https://www.britannica.com/topic/philosophy-of-mind/The-computational-representational-theory-of-thought-CRTT
- Reference: https://www.britannica.com/topic/philosophy-of-mind/Qualitative-states#ref283994

**Functional Structures:** The next question arises about why certain representations would have subjective experience and others would not. Is it sufficient that a particular kind of representation exists for it to be associated with subjective experience, or does that representation need to occur in conjunction with particular functional structures? For example, imagine that all aspects of the brain were understood to the point that we could identify exactly which representations are associated with subjective experience. Now imagine that an exact replica of a particular representation was encoded within the gates of a silicon memory chip within a computer. Most would argue that the silicon memory chip does not subsequently have subjective experience of that representation, because a representational state alone is insufficient for subjective experience. Some kind of functional structure presumably must be required to observe that representation. But if functional structures are indeed required, what are those functional structures? And what distinguishes those functional structures that are associated with subjective experience and those that are not? Once again here it can be hard to avoid the pitfall of infinite regress: if a representation must be interpreted in order to be perceived, and a functional structure is required in order to interpret that representation, what is the output of that interpretation if it is not just another representation needing to be further interpreted?

**Something Special:** A deeper philosophical debate rages about whether representation and functional structures alone are sufficient to produce subjective experience, or whether something else is required. In the example below, if all the representational and functional structures are in place for an individual to have both the external behaviours and internal mental behaviours of an individual in intense pain, can we even conceive it to be possible that they would not have the typical associated subjective experience of the pain?

> Suppose that, in order to avoid the risks to his patient of anaesthesia, a resourceful surgeon finds a way of temporarily depriving the patient of whatever nonfunctional condition the critic of functionalism insists on, while keeping the functional organization of the patient’s brain intact. As the surgeon proceeds with, say, a massive abdominal operation, the patient’s functional organization might lead him to think that he is in acute pain and to very much prefer that he not be, even though the surgeon assures him that he could not be in pain because he has been deprived of precisely “what it takes.” It is hard to believe that even the most ardent qualiaphile would be satisfied by such assurances.
>
> Reference: https://www.britannica.com/topic/philosophy-of-mind/Qualitative-states#ref283995

## A point of Central Unification?
One particular area of debate falls variously under the terms "Cartesian theatre" or "homunculus problem". The Cartesian Theatre ..introduced by ....describes the interactions between supposedly two parts of the mind: the part that has subjective experience (the audience in the theatre), and the part that produces the contents of subjective experience (the actors in the theatre). This has also been described as a "homunculus" or "little man" inside the brain that has the experiences. Both descriptions pose a problem: that the audience/homonculus requires a significant level of intelligence in order to interpret and understand the show being put on; but that same intelligence is required to produce the show in the first place. In the case of homunculus, we can provide two descriptions w.r.t. to the layers described above. In the first description, the non-conscious processes produce a representation that is perceived by the homunculus. Here the problem becomes what mechanisms the homunculus uses to do that perceiving? In the second description, the representation is sufficiently processed by functional structures so that no further processing is required, and that final result is simply perceived-without-processing. In practice this raises more questions than it seeks to address. What kind of thing is it that can perceive-without-processing? In response, the theory of semiotics (discussed in a section below) claims that it is impossible for such a thing to exist, because there is no perception without interpretation, and interpretation necessarily involves processing.

_todo: references and more details from:_
- https://www.lesswrong.com/posts/GBXKZujXSZe84aAL9/the-homunculus-problem
- https://en.wikipedia.org/wiki/Homunculus
- http://pespmc1.vub.ac.be/HOMUNCUL.html
- https://www.consciousentities.com/deadends.htm
- For later: semiotics explains this as being one and the same system.

Ned Block and various other's variations propose that consciousness is divided into access consciousness and phenomenal consciousness, and that access-consciousness variously stops somewhere below the "something special" layer, with various arguments about where it stops. Such arguments down to differences in opinion about the relation between access and phenomenal consciousness: i) are they one-to-one: all access conscious events have phenomenal consciousness, ii) can some access conscious events lead to external behaviour without the individual having subjective experience?, or iii) can some phenomenal conscious events occur that have no access consciousness: for example that the individual experiences in the moment but cannot have any memory of it and cannot report on it.

Others offer alternative ideas focused on how multiple streams of processing become "unified":
* Winkielman P, Ziembowicz M and Nowak A (2015) The coherent and fluent mind: how unified consciousness is constructed from cross-modal inputs via integrated processing experiences. Front. Psychol. 6:83. doi: 10.3389/fpsyg.2015.00083
* von der Malsburg, C. (1997). The coherence definition of consciousness. In M. Ito, Y. Miyashita, & E. T. Rolls (Eds.), Cognition, computation, and consciousness (pp. 193–204). Oxford University Press. https://doi.org/10.1037/10247-013
* von der Malsburg, Christoph (1997) The Coherence Definition of Consciousness. [Book Chapter]
* keywords: coherent theory of consciousness, coherence theory

# I.4 Background - Biology and Neuroscience 

Todo - brain parts etc

![forward and backward connections](files/forward-and-backward-connections-in-brain-marino-2021.png)


---


# Part II - Problems in Simple Synthetic Control Processes

# II.1 Interlude: Environment, Body, and Control Processes (first part)

_...todo..._


# II.2 Complexity and the need for Processing Loops

In most artificial neural network (ANN) based reinforcement learning (RL) agents today, each input is associated with an immediately produced output. This means that in an embodied agent the choice of the next physical action is made by a single pass through its ANN(s): input nodes are populated with current sensory signals, matrix operations are carried out that permute and transform those input node values through the multi-layer network of weights, and the values produced by the output nodes are immediately taken as the chosen next action. This is true even for Recurrent Neural Networks (RNN). RNNs are _recurrent_ in the sense that state from a previous pass is made available to influence the output on the next pass with the next input value. In this way, when a time-bound signal stream is fed into the RNN, it produces an output stream where each value in the output stream is influenced not just by the current input but by all inputs received up until that point. However, the RNN still produces exactly one output for every input, and each output is produced by a single pass through its network.

![single iteration anns](files/A-coherent-theory-v1-single-iteration-anns.drawio.png)

* _**Single-iteration Artificial Neural Networks (ANN).** Each of these networks produce one output for each input, via a single pass pass through the network. In the context of an embodied agent, this means that the agent has no option for further deliberation of the same input._

Another form of recurrency is to execute multiple passes through the same network before producing an output. This form is common in hand-rolled algorithms, where it is usually referred to as processing _loops_. When an algorithm employs a processing loop, a single output may be produced for each input, but only after a variable length delay. Some inputs may lead to updates of internal algorithm state only, without producing an output. Or a single input may produce multiple outputs. Examples abound, but one familiar to those in the AI research community is the Expectation Maximisation algorithm. It takes as input a set of data points, produces as output a set of parameters that describes the input data set, and employs multiple iterations of alternating calculation of log-likelihood expectations and parameter optimisation. The alternating expectation and parameter optimisation loop is stopped according to a _halting rule_ that is either based on detecting diminishing returns in the improvement of log likelihoods or on completing a fixed number of iterations.

Some have begun to experiment with loops in ANNs. Complex results can be achieved with shallower networks when using a loop-style of recurrency [Kubilius et al (2019); Wen et al (2018)]. Loop architectures have been used to adaptively vary the amount of computation time allocated to problems, as Adaptive Computation Time [Graves, 2016], which has been suggested as an important component of next generation language decoder-encoders known as Universal Translators [Dehghani et al, 2018].

There is a practical limit to the complexity that a single-iteration processing architecture can achieve. The network can be made broader (more nodes in each layer) and deeper (more layers), but that increases the number of parameters that need to be optimised during learning. In earlier versions of ANNs, where smooth non-linearity functions such as sigmoid were used within hidden layers, the vanishing gradient problem [citation] meant that practical networks could not be more than a few layers in depth. Current state of the art ANNs obtain non-linearity through piecewise linear functions and enable many more layers before the vanishing gradient problem becomes an issue. However an upper bound on the number of layers is still recommended [details, and citation]. Even GPT 3 only uses 96 layers [citation].

_..todo: any estimate on number of layers in human brain?_

![mountcastle](files/Striate-cortex-modules-mountcastle-1997.png)

Another problem with a single-iteration processing architecture is that its fixed depth implies a tradeoff between the maximum complexity that the architecture can handle and the cost of training in order to cater for the average complexity of situations that the agent must cope with. Additionally, if we consider that such processing may entail multiple stages of processing, the order in which those stages is executed is fixed.

An architecture that employs multiple passes through its network can be conceptualised by unrolling its iterations into a much deeper single-iteration network. But it has a number of advantages. Its depth varies dynamically as needed, for example that it is deeper for more complex problems. If processing is made up of multiple separable stages, the order in which those stages are executed can now be dynamically varied. It is additionally quite natural to imagine that for certain problems, some stages will be simply omitted entirely.

![multi-iteration ann](files/A-coherent-theory-v1-multi-iteration-ann.drawio.png)

* **Multi-iteration network.** Panel A: a multi-iteration network with the result from its output layer fed back as input. Panel B: an equivalent single pass network by unrolling the iterations into a deeper network assuming 3 iterations. Notice that in the depth-unrolled network, weights are shared between sections.

So, it can be said that there is a limit on the complexity that can be handled by a single pass through any computational process. While that computational process can be extended with more parameters, there are practical limitations to how much it can be extended. For embodied agents, this appears as a limit on the complexity of the environmental and of their own body that they can sufficiently model and respond to within a single processing iteration. In biological terms, this practical limit is manifested in terms of both the energy costs of larger brains and in terms of the time required to reach maturity of brain function.

To adapt to more complex environments, an embodied agent must employ multiple iterations of processing. This enables, for example, further analysis of the environment in order to better model its state; or further deliberation alternative action plans before proceeding. In biology, this provides scope for evolutionary pressures to trade off between a more energy hungry complex brain and a simpler less energy intensive one that might take longer to reach a decision for more complex problems. Van Bergen & Kriegeskorte (2020) make the case that recurrency is indeed employed in biology for that very reason.

_todo: Estimate of layer depth in brain?_

_todo: I use the term multi-step processing to clarify that I am referring to a particular form of recurrency where, for some materially significant portion of the process, the majority of its outcome is fed back as input.... yeesh, this is hard to quantify. _

_Todo: To avoid confusion with micro-level recurrency, this article uses the term "multi-step processing". 
or should I use multi-iteration processing everywhere instead?_


# II.3 State Trajectories in a Multi-iteration Processor

The course taken by an agent to get from a past state to its current state is its _state trajectory_. Analogous to the path taken by an agent while walking through a maze, the state trajectory describes the path of the agent through state space. Here the state space can refer to its possible locations in physical space, such as in the maze example, or to more abstract possible states, such as an encapsulation of all measurable aspects of the agent's body parts.

Not all state trajectories are good ones. The figure below illustrates a number of possible state trajectories from start state A to goal state G, while avoiding obstacle X. Each trajectory successfully reaches the goal, but they vary in other ways that may have significant impact to the agent. They length of the trajectory may indicate energy efficiency, which is important for an agent with limited energy reserves. The length may also indicate the time taken, which impacts whether or not the goal is reached "in time". The smoothness of the trajectory can be important. A jagged trajectory might indicate that the agent's physical body is moved in a chaotic way with abrupt stops and starts, causing damage to delicate moving parts from the stresses of that chaotic movement. A smoother trajectory may be easier for the agent to subsequently learn from and reason about in order to improve its later attempts; whereas a more chaotic path may add so much noise to the observations of the trajectory that the agent is unable to detect the most important patterns for such learning.


![good and bad state trajectories](files/A-coherent-theory-v1-good-and-bad-trajectories.drawio.png)

* _**Good and bad state trajectories.** Examples of some possible state trajectories from start state A, to goal state G, while avoiding obstacle X. The shortest and smoothest trajectory is assumed to be the best: the most energy-efficient, the quickest, the least stresses applied to the mechanics of the agent._

In a multi-step control process, the controller traverses a state space independent of the state of the body that it controls, as illustrated below. It needs to incorporate mechanisms to control its own state. Those mechanisms are referred to as _meta-management_, because they relate to management of the controller's own processes, rather than to management of the primary thing that the controller acts against (the agent's body in this case).

![control process trajectories](files/A-coherent-theory-v1-cp-trajectory.drawio.png)

<ul>
<li style="list-style-type: none;"><i><b>Control process trajectories.</b> With multi-step processing, the control process (`CP`) has its own state trajectory (`S_cp`), influenced by its actions (`A_cp`). Control process actions only occasionally produce changes to body state (`S_bdy`).</i></li>
</ul>

Within a learning setting, the control processes must learn to manage the state of the agent's body. Typically this is influenced by feedback received in association with the outcome of some sequence of actions. That feedback must be interpreted and used to infer the best way to optimise the parameters of the control process. In a synthetic RL setting, that feedback and parameter optimisation is performed via hand-coded learning algorithms, often incorporating back-propagation and gradient descent. In a biological organism, the corresponding learning processes may be somewhat more complex and are certainly much less understood, but their effect is the same: that parameters of the control process are optimised such that future attempts would be more successful or efficient. This is a first concrete example of meta-management.

The learning processes involved with a multi-step processor may be very similar to those involved with multi-step bodily actions. Each body action plays out over time, with complex dynamics affecting the speed and trajectory taken. The body actions required to reach a particular target body state may involve the sequencing and coordination of multiple actuators or muscles. Feedback about the relative success or failure may be sparse - only received as certain points in time, with no specific details about the relative effectiveness of steps in between, and even then the meaning of the information and how it relates to the state trajectory may be ambiguous. Any learning algorithm resolves that by assuming some distribution of the affects of the feedback over the length of the state trajectory and by averaging over multiple attempts. Some of the feedback received by an agent can be more frequent and detailed, such as those produced by evolved low-level processes that encourage smooth and efficient movements.

![cp state with meta-management](files/A-coherent-theory-v1-cp-state-with-mm.drawio.png)

* _**Control Process with state.** A control process (CP) that has state needs to act to manage its own state as well as the actions and state of the body that it controls. In some cases, this may require an additional _meta-management_ process. Some interactions omitted from the diagram for simplicity._

For simple control processes, those same mechanisms can be applied to parameter optimisation affecting the control process state trajectories. For example, the same low-level evolved processes can encourage efficient CP state trajectories by attempting to minimise the number of CP actions that don't produce body actions, without degrading the quality of the body state trajectories. Likewise, they may encourage "smooth" CP state trajectories in order to avoid disorganised chaotic processing.

But the simplicity of these suggested low-level CP state controls limits the capacity of the control process. Some computational problem spaces will require much more extended computational time, with much more divergent state space trajectories, than could be accompanied by these simplistic parameter optimisation rules. If a real physical world includes not just straight lines, but obstacles, walls, mazes, and other complex environmental constructions involving complex sequences of actions, then so too might a "computational world" that an advanced control process might have some need to operate within.

A good example is that of a path planner.........todo.....describe one particular planning algorithm in simple terms... Also mention that there are multiple approaches. 

![complex state trajectories](files/A-coherent-theory-v1-complex-state-trajectories.drawio.png)

* _**Complex state trajectories**. A) An example of agent position state trajectory as the agent navigates a maze environment. B) A hypothetical 2D representation of the trajectory of the internal state of a planner as it considers different possible paths for navigation within the maze environment. Here, pairs of upward and downward sub-trajectories represent the forward and backward pass of each considered path, and the general motion from lower-left to upper-right signifies the planner progressing as it finds increasingly better solutions._

The sequence of CP actions required to execute a planner are complex and, although an overall strategy is known, the exact sequence is unknown a priori. Additionally, there are multiple strategies for solving the planning problem and different domains may be better aligned to different strategies. 

So meta-management may be more than just parameter optimisation at learning time. It may involve processes for monitoring, modelling, and actively affecting the state of the control process while the control process performs its control of the body.

A detailed discussion for all the possible reasons for meta management will be carried out in a later chapter after introducing more elaborate forms of deliberative control process. For now, in the context of the control processes discussed so far, some example forms of meta management include:
- parameter optimisation at time of learning based on past action sequences and feedback 
- generation of low-level feedback signals such as to indicate efficiency and "smoothness" of state trajectories
- generation of feedback signals based on higher order understanding of the problem domain (eg: that the path planner considered paths in the wrong order)
- monitoring of control process
- active tuning of control process during execution
- strategy selection

In conclusion, a multi-step processor requires meta-management. For the most simple multi-step processors, meta-management can be in the form of simple parameter optimisation algorithms applied during a learning phase post execution. For more advanced multi-step processors, a much more advanced and active form of meta-management is required, one which might even have comparable complexity to the primary control process itself.


---


# Part III - Problems in Complex Synthetic Control Processes

We now turn our attention to deliberative artificial embodied agents that might operate within the real world.

# III.1 Meta-management in Deliberative Systems

_todo: needs a clear strategy for referring to "main/standard/first-order control process"_


Why might we need to add meta-management processes to connectionist architectures? Deep AI techniques have had many successes of late [citation]. However, these networks still lack some of the most basic adaptive capabilities that we see in many biological organisms (citations, eg: sloman). A key feature lacking from AI today is _deliberation_. Deliberation can be thought of as an extension of multi-iteration processing to more human-like thought that incorporates modelling of multiple problem domains, selection of goals, the ability to break problems into smaller sub-goals, and the ability to select between multiple strategies for problem solving.

A number of potential control problems have been identified in systems with such deliberative capabilities (Beaudoin, 1994):
- **Oscillation between decisions.** Wasteful re-assessments of decision points, leading to a meta-stable (oscillating) but stagnant state (ultimately achieving nothing useful).
- **Insistent goal disruption.** Repeatedly getting distracted by competing goals that have been previously disregarded.
- **High busyness.** Attempting to multi-task between too many goals, leading to poor outcomes.
- **Digressions.** Choosing to deliberate over some sub-goal, and then loosing track of the "big picture" by forgetting to return to the overarching goal.
- **Maundering.** Getting stuck deliberating over the details of a goal without making a decision.

Here some specific meta-management features are discussed in the context of how they might improve connectionist computational systems with deliberative capabilities. This "design stance" is useful as a means for teasing out the lower level mechanisms that may underlie much higher-order behaviours such as meta-cognition.

## State Trajectory Control during Body Action
Actions by an embodied agent occur over time. During the time it takes for an agent to move its arm through space from the arm's initial position to target position, the agent will make many observations about the environment and body states. The agent's goal and action plan must be relatively persistent during that time. Otherwise the agent's behaviour will be chaotic, with rapid goal and action changes.

Thus, while the agent manages (controls) the trajectory of its body state through the use of its computational state (eg: the given goal and action-plan at the time), it must also meta-manage the trajectory of that computational state. In this case, the agent's computational state must to some extent resist change influenced by new observations.

## State Trajectory Control during Multi-iteration Processing
During multi-iteration processing the control process navigates through computational state space, without performing body actions.

This state trajectory needs to be managed just the same as for the body state trajectory. In order to maintain stability the agent needs to i) observe the state trajectory, ii) apply some objective measure to decide upon the relative effectiveness of the trajectory, and iii) act to change the trajectory if a better one is available.

## State Trajectory Control during Iterative Inference
A special case of multi-iteration processing is that of _iterative inference_, where the control process takes multiple iterations to interpret some input signal. Here a representation of the input signal may need to be held persistent for the duration of the inference, even if the original input signal has ceased. For example in an animal context where a fleeting glimpse of a potential predator has been observed but that observation needs re-review before being certain.

In that case, some portion of the state must be held stable, while the rest is free to change significantly. Something needs to manage

## State trajectory control in summary
_todo: do I really need this summary?_

As discussed in detail in an earlier chapter, there is a strong case for the need to actively manage the trajectory of the agent's computational state. Three contexts have been highlighted for this need:
- during iterative prediction (micro-scale recurrency)
- during looping multi-step execution (macro-scale recurrency)
- while waiting for actions to play out.

Mechanisms underlying state trajectory control can include:
- Observing performance over time
- Predicting future outcomes from current trajectory
- Predicting expected future utility of current trajectory, and comparing against that of other predicted possible trajectories.
- Applying tuning control where current trajectory is sub-optimal.

## Objective learning
How does a continuously learning embodied agent know which actions are better than others? This decision is tied to the agent's objective: it's ultimate goal that influences all other goals. For example, to eat and stay healthy in order to survive. Or to produce as many staples as possible in as little time as possible (citation). If the agent is not pre-configured with its objective, then it must learn that objective.

An agent in the human world requires the use of inedible metal tokens (coins), which are used in complex ways for the purpose of life preservation. The involvement of such an inedible metal token as part of some process (eg: doing a job and being payed) does not necessarily immediately result in a life sustaining outcome. Thus, without any other information, it is hard for the agent to learn the relationship between that inedible metal token, the processes that it must be involved in, and the life sustaining result. This is known in the AI community as _sparse feedback_, and it poses a particularly difficult problem for continuously learning agents (citation needed).

Another problem for a continuously learning agent is known as the "exploration-exploitation dilemma" (citation needed). The agent gains knowledge about its world and itself by exploring places and things, and by experimenting with novel behaviours. When the agent needs to achieve a goal, it may know that it can achieve the goal via its existing knowledge (exploitation), but it may be able to achieve that goal in some better way if it were to explore more first; it also may not. The dilemma concerns how the agent chooses between exploration and exploitation at any given moment.

Sparse feedback and the exploration-exploitation dilemma make objective learning difficult. One solution is for the agent to build simplified models of its environment, itself, the behaviours it can perform, and how those behaviours influence different outcomes. Simplified models have fewer degrees of freedom than found in the raw first-order signals. This means that the models can be built up from fewer examples, and they are easier to change as learning progresses. These models become the agent's "knowledge", and somewhere within that knowledge a continuously learning agent builds a structure that ultimately governs its behaviours and goals – that is, an objective that it infers over time.

_todo: remove....Importantly, those models can have different forms, and their forms influence what kinds of inferences the agent can draw from the knowledge, and consequently how they can be used for other management and meta-management purposes. A discussion of different models is presented in a later section._

_todo: needs revising....Objective learning becomes a meta-management concern for two reasons. Firstly, the objective governs all lower level concerns, including meta-management. Secondly, as will be seen later, meta-management necessarily operates at a higher-order representation, and is thus an appropriate framework upon which to build objective learning._

## Mode control
A number of seemingly distinctly different behavioural outcomes share a single principle, referred to here as _mode control_. Mode control involves a decision being made between multiple alternatives and that decision influencing the way in which a subsequent process or decision is carried out.

Examples of mode control include:
- **Strategy selection.** Choosing between multiple previously learned strategies (ie: sequences of processing) that may be useful for solving the particular problem at hand. The selected strategy may affect goal selection and/or it may bias the outcomes of certain processes.
- **Goal selection.** Choosing the next target state, for example based on an interpretation of external signals, or from weighed up options in an ambiguous situation. The chosen target state thus becomes the reference point for generation of actions.
- **Context.** Context plays a huge part in the interpretation of sparse signals. A visual patch of yellow with dark spots, when seen in the Savannah, may indicate a leopard, but the same patch on the beach may simply indicate sea shells. Context is not always available from direct sense of the external environment. Most perceptual interpretation also receives context from short-term and/or long-term term memory. Thus meta-management plays a role in inferring that context from a mixture of current sensory signals plus memory.
- **Attention.** As suggested in the chapter on embodied state machines, the bandwidth of any computational system is limited, and the complexity of the environment may exceed the agent's computational bandwidth. One solution is to focus on only the most salient features of the environment, ignoring the rest. What the agent considers salient differs depending on things in the environment, the context in which the agent is operating, and on the agent's knowledge. Attention has a significant impact on the processes executed by the main control process – a change in attention changes the input to the control process, and thus to its output.
- **Exploration vs exploitation.** Already introduced in an earlier discussion on objective learning, the choice between exploration and exploitation affects sub-goal selection and the actions taken by the agent. Where an agent chooses its actions based on certainty of expected outcome, an exploration mode may for example bias the agent towards preferring expected outcomes with less certainty.

## Mode identification
For mode selection to be possible, the agent must identify the modes that can be selected from, whether they be discrete or a range of continuous values. This requires two important features of the meta-management system: i) that it has sufficient access to observe the things that it needs to control, the outcomes of the control, and the values used in control; and ii) that it can model those observations and later use that model to choose the control mode.

In some cases this may involve modelling the relationships between different components of the first-order control process. Timmermans et al (2012) give the example of meta-cognitive processes learning cause-effect relationships between the supplementary motor cortex and the primary motor cortex and using this to infer what signals to send from higher order areas.

## Distributed cooperation
Some theories of brain function describe the brain as having multiple independent processes that are in constant competition. For example the biased-competition theory of attention (citations) assumes multiple processors, each interpreting their own local sub-scene out of a larger visual scene. It pits those different sub-scene interpretations against each other, until a single unified scene interpretation wins out. Global Workspace Theory adds the option for groups of otherwise competing processes to cooperate (citation), with the outcome being that a group of processes can collectively win the competition for attention when each process individually would loose.

This seems like an obvious situation in which meta-management has a part to play – in managing the competition and cooperation between those processes. One possible mechanism is the same as discussed in the section above on Mode selection – by adjusting priors.

Curiously, as observed by Baars (citation, pp ref), humans don't appear to have experiential awareness of this competition / cooperation process. Rather, we observe only a sort of stabilized outcome. So perhaps this is a first-order concern, at least in humans. But in principle it could also be a meta-management concern.

## Certainty measurement / reaction
todo: Eg: low level simulations linking certainty encoding to attention. Not sure how used for meta mgtmt, but has a plausible low level mechanism.

# III.2 Interlude: Mechanisms of Standard Control Processes

What form might meta-management take. In order to answer that question I shall first present a review of different architectures for standard control (ie: non meta-management). 

_..todo...maybe now diagram all the component parts of an AI RL learning algorithm, so we can see what meta-management is already incorporated._

In AI, a common scenario is to train a simulated robot to navigate within a virtual environment. It is common to incorporate a Neural Network (NN) as part of the control system and to use Reinforcement Learning (RL) to train that neural network. Several broad options exist for the architecture of the control algorithm. These can be framed as a progression of improvements, that lead to increasingly better adaptability. The progress is illustrated in the diagram below, and outlined as follows. 

_...todo...update wording below to use "policy" instead of "function"._

![standard control algorithms](files/A-coherent-theory-v1-std-control-algs.drawio.png)

* _**Control algorithms.** A graduation of increasingly adaptive control algorithms in an embodied controller. Training algorithm connectivities simplified or it is entirely omitted for the sake of simplicity. A) A so called "model-free" parameterised function that produces action without awareness of its own state. B) Model-free parameterised function that is aware of its own state. C) A so called "model-based" planner that predicts entire trajectories in order to choose the best action, with or without awareness of its own state. D) a hybrid that employs model-free control with a planner to observe and protect against major errors._


_..todo.. for all of the sections that follow:_
- _need to describe the algorithms better, and more formally._
- _look at industry explanations_

## Stateless reactive control process
In the most simple case, a _policy_ NN simply predicts the best action given a sensory input about the environment. A typical example is a robot car with very simple choices of actions: stop/go, left/right/forwards. The robot observes its surroundings using, for example, vision, sonar, or laser. The dynamics of the robot itself are ignored. The robot is assumed to produce the required action immediately; for example that no time is taken while the robots changes its steering angle.

This kind of agent is known as _model-free_, because it lacks an explicit model of the state-space in which it operates. For example, it has no possibility to predict expected outcomes of actions and to detect when actual outcomes diverge from expectation.

The RL algorithm is really the thing with the smarts here. It has access to much information that the agent does not. For example, it knows what the training goal is (eg: to navigate a race course), it knows the ground truth position and orientation of the robot at all times, and it knows how "costly" each robot action was relative to the goal. From that information it computes a _loss function_ as the time-devalued sum of those action costs [citation, and details]. That loss function is then used via back propagation to update the weights within the NN.

In the earlier days of neural network research, including deep learning, many of the problems addressed were of this very simple form.

## Stateful reactive control process
A small improvement enables the agent to cope with its own dynamics.

Here the agent has information about its own state. For example, information about the current steering angle and speed of the robot car's wheels. ....[citation needed].... how does that actually improve things?

A particular scalability problem afflicts reactive control processes for more realistic real-world scenarios. In the real world, the best trajectory is a function not just of the initial state, but also of the goal at the time. Here the policy NN learns a probability distribution `P(a|s,g)`. The potential range of goals could be large, and thus the dimensionality of the distribution is exponentially larger than `P(a|s)` alone. And this solution only generalises to new goals that are similar to ones seen at training time.

## Planning control process
A significant improvement to adaptability and reduction in training time is seen in AI research by incorporating a planner into the control process. Here, a model is incorporated that predicts the effect of an action on the state of the environment and on the agent's own state. Rather than predicting a single best action, the agent simulates a trajectory from its current state via a sequence of actions to see where it may end up. It does that multiple times with multiple trajectories. It completes each step by picking the best trajectory tried, and the first action from that trajectory. Then it repeats the whole process again for the next timestep.

Compared to reactive control processes. Such a solution has a significant advantage in the real world where the most appropriate action depends on the goal at the time. The planner learns a model P(s'|s,a). The model is not parameterised by goal, as the goal needs only be considered at the time of planning. Additionally, the same model parameters can be updated from experience regardless of the goal that was being followed at the time. So the model generalises well to totally unseen goals.

A key feature of this control algorithm is the use of _simulation_ when considering different possible trajectories. A simulated sequence of actions can often be run orders of magnitude faster than actually carrying out the same sequence of actions. Negative outcomes in a simulation have no impact on the agent except for the time spent running the simulation. And simulations can even be used to train other systems.......todo: [citation] example of EM where problem space is split into multiple models.

Unfortunately, this planning approach can also be computationally inefficient. In a naive implementation an extensive amount of computations are performed that are completely discarded and repeated again. It also doesn't scale well into long trajectories of high-resolution. Various optimisations exist. One particularly relevant optimisation is to use a planner to produce a course-grained high-level trajectory, and to use a reactive control process for the fine-grained motion control. In such a setup, the next point in the high-level trajectory sets a dynamic goal that is fed into the reactive control process as an additional input. [citations]

Note that the structure and algorithm of the planner is far from given. It too has many parameters. In AI research the planning algorithm is typically chosen beforehand. In a biological setting, the planning algorithm itself may be learned from experimentation and instruction.

_...todo....this needs better phrasing. I think I should accept that the planner is multi-step, and that meta-management is incorporated into the hard-coded planner implementation, but that it's all totally different for a biological setting:_
_- In most AI research today, a planning control process is still a single-step control process: each env + body state inference is associated with a single pass through its control process and an immediate choice of action. Any apparent multi-step processing, such as within the planner, are typically hard-coded by AI engineers. The planning process is not controlled by a learned NN. In biology, such a hard-coded static planner does not exist. The biological organism needs to learn how to do and control such a process itself._

_...todo...use this to introduce the idea of a biologically plausible NN-based planner._

## Expectation-Maximisation / Iterative Convergent Control Processes
...todo..


## Hand-written Control Processes in AI vs Biologically Plausible Control
_todo_:
* I need to make regular reference to the idea that AI today uses a lot of "hand-written" processes, many of which are imperative in style rather than connectionist. So there are many aspects of AI today that are a) not biologically plausible, and b) conveniently skip some of the problems that I'm trying to identify and propose solutions for.
* Then draw some specific comparisons and a framework for understanding the biologically plausible equivalents: dynamic layers bootstrapping on top of relatively static layers.

In the above I have taken substantial inspiration from contemporary AI research into artificial connectionist computational paradigms. I shall continue to use AI research for to take inspiration and to draw comparisons. For that comparison to be legitimate, I need to address a major difference between contemporary AI's use of connectionist architectures and that of biology.

In contemporary AI...... It could be argued that even the primary control process itself is more imperative than it is connectionist. The connectionist architecture is just a "model" - not the real thing, but a data structure that represents some key properties of the real thing. As it is just a data structure, something else must _execute_ it. And the thing that executes is hand-written imperative code.

In its most significant example, and applicable to most implementations today, the main cyclic processing loop - the thing that takes the current sensory input, processes it, and then actions the output - is governed entirely by imperative code. The decision whether or not to feed the output into actuators is governed by hand-written imperative code. The decision whether to start the loop in the first place is governed by hand-written code. The decision of _when_ to stop the loop is governed by hand-written code. That last, most important decision, is not based on anything related to the connectionist model, nor the outputs of the connectionist model, nor even of any sense of "lifespan" of the agent. Rather, it is typically related to either a training "epoch" (an entirely arbitrary time period, usually of only a few seconds) or to a "buffer size" (ie: of how long before some data buffer becomes full and where those hand-coded meta-management processes must kick in).

...

![hard-coded CP and MM in AI](files/A-coherent-theory-v1-hard-coded-cp-and-mm.drawio.png)

* _**Control and meta-management processes in contemporary AI.** A mixture of imperative code hand-written by AI researchers plus connectionist models implement the control and meta-management processes of the agent._

...that is not entirely dissimilar from biology. Biology employs aspects that are "hard-coded" by an individual's genetics. But the key point here is that significantly more of the control and meta-management processes use connectionist solutions that learn. In that way, contemporary AI today avoids some of the difficulties faced by biology. But it also misses out on the opportunities provided by that flexibility.

![biologically plausible CP and MM](files/A-coherent-theory-v1-bio-plaus-cp-and-mm.drawio.png)

* _**Control and meta-management processes in biology.** Layers of increasingly flexible and learning connectionist networks run on top of more static connectionist networks, plus on top of a "hard-coded" body._

_todo: improve diagram by making it just one vertically connected network, with fussy boundaries rather than strict boundaries, and describe the vertical sections as layers._


## A Biologically Plausible Planning Control Process

_...todo...But first, to help motivate the discussion, let's first specify a useful example to have in mind...._

The control algorithms considered were taken directly from AI research, but not all of the implementations are biologically plausible in the same form as used within AI research. It is reasonable to consider that an ability to do planning is very important for biological agents just as much as it is for artificial agents. But biological agents are unlikely to be imbued with a fully-formed pre-built planning engine. And even if such a thing was partially or fully formed, it is more likely to built using the same kind of neural network structures found throughout the rest of the brain.

![biologically plausible planner](files/A-coherent-theory-v1-bio-planner.drawio.png)

* _**A biologically plausible planner.**_ _A NN-based policy executes as a multi-step control process (`CP`). CP state_ (`s_cp`) _represents everything that a planner may need to hold onto, including the partially complete trajectory being considered at the time and information about other trajectories already attempted. The policy predicts control process actions_ (`a_cp`) _that change the control process state_ (`s_cp`). CP actions sometimes also cause body actions_ (`a_bdy`) _that lead to new body state_ (`s'_bdy`) _and environment state_ (`s'_env`). One or more separately trained models could feed into the policy, or the policy itself could effectively represent those models. The training algorithm optimises policy parameters in order to achieve the right body state trajectories while meeting CP state constraints_ (`c_cp`) _and body state constraints_ (`c_bdy`). _Parameter optimisation of models not shown._

The above diagram presents a rough structure of a biologically plausible planner. The pre-built planner is replaced by a policy network that controls the behaviour of the planner in exactly the same way that a policy network could control the outwardly visible behaviour of an embodied agent. Actions produced by the planner (`a_cp`) are for the most part hidden - they modify the state of the control process (`s_cp`) without producing any outwardly visible behaviour. Depending on certain properties, some CP actions additionally produce body actions (`a_bdy`), this being the key goal of the planner.

The policy network is trained through reinforcement learning to produce suitable CP actions and body actions. On average the right body actions should be generated that produce suitable body state trajectories from current state to goal. And the number of CP actions that don't produce body actions should be minimised in such a way that the appropriateness of body actions are not significantly reduced. In a biological setting, suitable low-level constraints would be optimised through evolution in order to achieve those outcomes.

A traditional AI planner incorporates one or more models in order to predict the effect of actions. The policy network described here incorporates an inverted version of that model, and so it does not require a separate model as input. However, as mentioned in the planning control algorithm introduction above, having a separate model of state space and the effects of actions against that state space gains some efficiencies and improved generalisations. Thus a biologically plausible NN-based planner likely incorporates models too. The specifics of how that might be achieved are outside of the scope of this article.

The structure described here can produce the behaviour of a planner in the traditional AI sense. But it is more generic than that as its behaviour is driven by whatever reinforcement learning is applied against it. It could also produce other kinds of behaviour, including iteratively refined interpretation of observed state, other AI algorithms such as Expectation Maximisation (EM), or more human-like behaviours like problem solving. The same policy network could even exhibit multiple behaviours, depending on the need at the time.

But how stable would it be? Would it need a meta-management process to help it converge more rapidly?

_...todo...Also present argument that meta-management only makes sense in the context of a planner such as this, because it has multiple steps where it doesn't produce actions, whereas all the variations of reactive function always produce body actions.  That motivates why the next section considers meta-management in the context of a planner._

# III.3 Meta-control Options in Meta-management

What options are available for a control process to be meta-managed? We have already mentioned parameter optimisation. Here we shall look at some other options. The goal is not to provide an exhaustive list, but to build up a case for the need to observe the control process and to draw out what kinds of observation might be needed.

![meta-management control options](files/A-coherent-theory-v1-mm-cntrl-options.drawio.png)

* _**How meta-management can influence the control process.** Identification of some ways in which a control process may be meta-managed._

Let's examine some options:

- **Parameter optimisation.** Our first example of meta-management was "after the fact" parameter optimisation. This occurs as a training process guided by feedback following execution of the control process against some problem. Through processes such as gradient descent and back-propagation the parameters of the control process can be optimised so that future attempts are improved.
- **Strategy selection.** The control process may develop multiple strategies for solving different kinds of problems. For example there are multiple ways to do path planning. Selection of the most appropriate strategy for a given problem at hand is an example of meta-management. 
- **Goal selection.** Real world agents don't have hard-coded goals. They change goals according to situation.
- **Bias control.** The biological brain is believed to incorporate a predictive coding architecture....[citations, and elaboration]. Inferences incorporate biases. Those biases can be manipulated by some explicit meta-management process. An example can be seen in mammals with interactions between the sympathetic and parasympathetic nervous systems influencing thought processes.
- **Direct state control.** Perhaps it is possible to directly influence the state of the control process.
- **Input manipulation.** It is possible to change the input in order to change the behaviour of the control process. This could be, for example, through attention. A more elaborate example is to infer what input manipulations are necessary in order to produce a desired CP behaviour, which would require more advanced modelling of CP behaviours and how various inputs affect those behaviours.
- **Output manipulation.** Another possibility is to directly manipulate the output from the control process before it takes effect on other systems. One example is to use this to entirely replace the control process in some situations. Another, perhaps more realistic example, is to attenuate the strength of signals from the control process while the control process is in its earliest stages of training. When the control process is untrained, it is likely to produce chaotic behaviours that might be detrimental to the survival of the agent. Some measurement of its level of stability could be used to gradually increase the strength of its output signals over time.
- **Feedback manipulation.** The outcome of the control process causes feedback. Meta-management can be involved in the interpretation and even manipulation of that feedback. A simple example is to infer what parameter optimisations are required based on the feedback. This may include mechanisms for handling sparse feedback by somehow averaging and distributing the feedback over the sequence of actions that were carried out. Another example is to produce the feedback itself. In AI this is known as learning the reward model...[citation, and elaboration]. A further extension is possible if the meta-management processes are actually more advanced than the reactive control process, and that the meta-management processes can independently devise measures of success.
- **Controller selection.** Similar to the case of strategy selection. If multiple different control processes are available, a meta-management task is to choose which control process takes effect, or perhaps to choose a relative weighting of effect.

A few general notes can be said about the above. Firstly, parameter optimisation is the only example of an "after the fact" meta-management process. The rest all take effect during online execution of the control process against a current problem. This is significant because it suggests that a) meta-management processes need to be actively involved during execution of control processes, and b) meta-management processes need immediate live observation of the behaviour of the control process as it executes.

Many meta-management processes can be implicit or explicit. Implicit meta-management occurs as a side-effect of the reactive mechanisms of the control process. Explicit meta-management is driven by a separate process that somehow influences the control process. For example, in AI, parameter optimisation is typically carried out as an "offline" process by a learning algorithm that is entirely separate from the processes used when executing the control process. In contrast, within biological brains, it is believed that _hebbian learning_ occurs as the primary learning mechanism and that it primarily occurs as "online" learning ....[citation, and further elaboration].

# III.4 Meta-observation Options in Meta-Management

In order to carry out any of the meta-control mechanisms described in the section above, any explicit meta-management processes need to observe the behaviour of the main control process. We look now at a brief review of some of those meta-observation options.

![meta-management observation options](files/A-coherent-theory-v1-mm-observation-options.drawio.png)

* _**How meta-management can observe the control process.** Illustration of the sorts of things that explicit meta-management may need to observe, and the processes that might be involved to draw inferences from that information._

Mechanisms for meta-management processes to observe the control process include:
- **Inputs.** Including any goal selection supplied from systems outside of the scope of discussion. Needed in order to associate CP behaviour with certain kinds of input.
- **Outputs.** Needed in order to observe CP behaviour.
- **State.** For multi-step control processes, their internal hidden state may be the only thing that changes from step to step. It is the trajectory of the CP state that we first called out above as needing meta-management.
- **Whether outputs lead to body action or not.* Useful in order to measure the "efficiency" of the multi-step process for producing useful body actions.
- **Feedback.**
- **Trajectory caches.** Unlike the control process itself, meta-management may need to track the trajectory of CP behaviours over time. Likely across multiple timeframes. This will involve some mechanism to represent those trajectories. For example, the trajectory in the context of the current problem at hand in order to monitor whether it is leading towards a solution. And for example tracking of the control process's overall abilities and over time, and whether it tends to produce useful results or tends to be "wrong" (for some definition of "wrong").
- **Modelling.** Modelling of CP behaviour and how meta-control signals affect them, in order to infer the most appropriate meta-control signals.
- **Predicting.** For example predicting whether the current CP state trajectory is likely to lead towards a beneficial outcome or not.
- **Associative memory.** Used to recognise frequent and infrequent CP behaviours that need specific meta-management. For example, situations in which the multi-step CP tends to get "stuck in a loop", where it would repeat a particular cyclic sequence of steps ad-infinitum without any intervention.
- **Measuring error rate.** Recording and tracking how beneficial the CP behaviours are, such as would be needed to attenuate CP output strength in early stages of CP training.

Of particular note is the fact that many of these mechanisms described are the same kinds of systems that would be used in an advanced agent for the observation, inference, and manipulation of interactions between the agents limbs, and between the agent and the environment.

# III.5 Architectural Options for Meta-management

..todo: intro..

![meta-management architecture options](files/A-coherent-theory-v1-mm-architectures.drawio.png)

* _**Meta-management Architectures.** Three broad architectures for meta-management. A) Implicit - the control process converges towards stable behaviour without any explicit meta-management processes acting upon it. B) Independent - explicit meta-management processes acting upon the main control process. C) Inline - control process acting upon itself to self meta-manage._

## Implicit Meta-management
This is the null-hypothesis of meta-management strategies. The control process somehow produces stable behaviour without any explicit meta-management processes acting upon it. Or whatever meta-management processes are required are inherent within the primary mechanisms of the control process.

Only the simplest of control processes could fit this category of meta-management. One example is a simple mechanical thermostat that uses temperature feedback to control a heater. No meta-management is required as the system's control strategy is static - it does not learn.

Perhaps it could be argued that an Expectation Maximisation style of iterative inference incorporates its own implicit meta-management. This could be true provided that no additional process is required to act upon it in order to adjust its behaviour. Once again, no real learning takes place.

## Independent Meta-management
A training process that records positive and negative feedback, derives a loss function, computes the gradients, and optimises the parameters of the control process is a simple example of an independent meta-management process. It is the most common example within AI research today.

In AI research the training process is typically hand-rolled, but research has begun to look at how some parts of that process can be replaced with ANNs. This includes using ANNs to estimate gradients (Bengio, Léonard, Aaron Courville, 2013) and using ANNs to calculate parameter updates (Andrychowicz et al, 2016).

So, one can consider the possibility of a neural network that calculates and executes all of the meta-management needs against a target control process. This could include all of the meta-control options discussed in a section above.

## Inline Meta-management
A somewhat radical suggestion is that perhaps the control process can meta-manage itself, given the right conditions. This suggestion stems from the observation that the processes involved to observe, infer, and act as part of meta-management seem very similar to those processes that we would assume make up the main control process in terms of interactions with its own body and the environment. In a complex environment we would expect those processes to be very complex. In a biological brain, due to the complexities and difference between the different sub-processes (modelling vs memory, for example) we expect some degree of brain region specialisation. Correspondingly, if two different problem domains need the same kind of processing capability, perhaps the same brain region might handle that processing capability for both problem domains.

What conditions might make this possible? Firstly, the control process needs to observe its own behaviours. 
This could be achieved via a feedback loop that captures that behaviour and feeds it back as input. That feedback may capture the control process' current state, its recent trajectory, and its inputs and outputs.

In some architectures, the overall state of the control process may be held as state within each network node. Any attempt to capture the whole of that state leads to an infinite regress on the size of the control process. Thus, necessarily, the feedback loop would provide a higher-order, dimensionality reduced, summary of that state and behaviour.

Importantly, the output of the feedback loop needs to frame observations about the control process not from the perspective of the control process's current state on its immediate current task, "from the inside" as it were. Rather, it must carry the perspective of the control process as part of a larger system, and as it interacts over a larger period of time. In other words, framed with a perspective as "from the outside".

Lastly, training of the whole system needs to be bootstrapped. Initially the self meta-management capabilities of the control process will be as chaotic as its primary control behaviours. This could be achieved through a separation of meta-management concerns into a non-learning primitive (or "innate") independent process that applies simple domain agnostic constraints against the learning, adaptive, and complex processes of the self meta-managing control process.

## Chapter Summary
All of the meta-management architectures described above may be valid. In fact, biological brains probably incorporate a mixture of all of them, and perhaps with other mechanisms not listed above. But we are interested in the most significant form of meta-management that might be at play in the context of subjective experience. Subjective experience seems to be tightly correlated with higher order executive control, and so we are interested in the most significant form of meta-management as it pertains to that higher-order executive control.

When looking at generic control problems, there is no architecture that is clearly more effective or more realistic than the others. Perhaps the answer depends too much on how the control process itself functions. The devil is in the details, as they say. The functioning of the control process depends also on what kinds of control are required, and the more interesting kinds of control process occur in more complex agents.

Another sobering issue is that the distinction between these three architectures is somewhat poorly defined. If inline meta-management is a valid architecture, what distinguishes it from an implicit architecture? What distinguishes the "Summarisation" component in panel C from the independent meta-management process component in panel B?

For those reasons, the next part drills deeper into more complex control process requirements and mechanisms. After that we will be in a better position to circle back to re-address the question of meta-management architecture.

In the interim, however, there is some anecdotal evidence to suggest that the inline meta-management architecture is at play within humans. It is said that humans have 5 senses of touch, taste, smell, sight, and hearing. That list has since grown with the recognition of proprioception, balance, and other internal senses ..[citation, and use of accurate terminology]. While it is not often classified as such, our awareness of our own mental state behaves like any other sense. The extent to which we can attend to any sense varies by modality (eg: while we have proprioceptive sense, it doesn't seem to carry the same ability to flood our consciousness than, say, our vision), but they are clearly all available for observation, integration, differentiation, correlation, modelling, and reaction-to within that higher-order executive control process that seems to be associated with subjective experience. This applies equally to the sense of mental state. That suggests the feedback loop described within the inline meta-management architecture.

_todo: either here or somewhere else, I need to draw correlation between the inline meta-management architecture and human phenomena, eg: higher-order thought, awareness of only certain processes_

---


# Part IV - Problems in Biological Control Processes

The focus of this article now shifts from generic "agents" of any form to biological organisms with complex brains. I shall start by reviewing some human concerns that relate to meta-management and for which suggestions have been made about their connection to human consciousness. This will be followed by an examination of potential meta-management processes within human brains.

Like many others, I focus on humans in order to avoid the ambiguity and uncertainty inherent with topics such as intelligence and subjective experience within the larger animal kingdom. This should not be taken to imply any statement about that larger animal kingdom. In fact I do make a few points in relation to other animals in a later part.

Now that this article is focused on biology, and humans in particular, the reader will also notice that some of the terminology shifts to be more human-centric. One such shift, with a happy coincidence, is that the abbreviation CP will now be used interchangeably to stand for both _Control Process_ and _Cognitive Process_ - because a cognitive process is just a computational-style of control process, implemented upon a substrate of wet biological neurons.


# IV.1 Interlude: Environment, Body, and Cognitive Processes

Before continuing, it'll be useful to do a deep dive into the interactions between the three key systems of: external environment, body, and the cognitive processes. This is key because it explains the importance of independent modelling of env, body and CP, and thus why "I" becomes so prominent in the computation that produces subjective experience.

With respect to an embodied individual, three interacting systems are typically assumed: external environment, body, and mind. In an attempt to be a little more precise, this article uses the term _"cognitive processes"_ (CPs) instead of _"mind"_. In any case, while these systems provide a useful basis for discussion, their exact distinction can become blurred. So some effort is first required to define them more clearly.

## Classification

_todo: most of this chapter is potentially interesting but a waste of time w.r.t. to the thesis. If I leave this in, it needs to be introduced as such. A key message could be to make the reader aware that the kinds of interactions between env/body/cp are far more nuanced and varied than are discussed in this article generally, but that the article ignores them for the sake of simplicity._

In attempting to define the delineation between these three systems, it is important to take a particular perspective: that of evolution. The most simple organisms lack a nervous system but nevertheless have evolved to react sufficiently well in order for their species to continue. We can say with some certainty that they lack cognitive processes of any sort, but they do have a clear delineation between their body and the environment around them - that delineation usually being a semi-permeable membrane. Evolutionary forces have produced such an organism to act in a way that it mostly protects itself from danger long enough to produce offspring. With some organisms, such as jelly fish, a nervous system has evolved that improves the ability of that organism to meet its homeostatic needs (eg: feeding), to protect itself from danger, and to procreate. The nervous system is entirely there to meet the needs of the body as a whole - those same same needs that applied to simple organisms lacking a nervous system. In mammals that nervous system is largely centralised into the brain as a discrete organ and in some cases that brain acts to look after its own homeostatic needs independent of the direct needs of the rest of the body.

So the nervous system is just a part of the body in the same way that a limb is. There is no need to be confused about body vs mind, as in truth the mind is just a physical brain, which is a subset of the body.

It is useful however to treat the processes and states of the brain/main as separate from the rest of the body, so they we can analyse the interactions between the subsystem of the brain/mind against the other subsystems of the rest of the body. This article draws such a distinction.

Thus we have:

||Environment|Body|Cognitive Processes (CPs)|
|--|--|--|--|
|Description|All people and things external to the physical body of the individual.|The physical form of the individual in its entirety, including head and brain.|A part of the Body. Computational processes that operate within the nervous system of the body.|
|State|Environment State|Body State|Variously referred to as Cognitive State or CP State.|
|Actions||_Body Actions_ include: any externally observable actions, hormone released from anywhere except the brain. Body Actions exclude: actions performed directly by the Cognitive Processes.|_Cognitive Actions_ include: sending nerve signals to control body actions, changing cognitive state, hormone release from the brain.|

During discussions that follow it will often be necessary to place cognitive processes and their underlying neural basis in juxtaposition with the rest of the body. In general I try to use the phrase "rest of the body" to make that clear, but in some cases that becomes too cumbersome and the term _Body_ implicitly assumes the meaning "rest of the body". This is particularly the case for the term _Body Actions_, which are always assumed to exclude those actions which are better categorised as _Cognitive Actions_.

With that said, let's examine what these three systems can do:

![env, body, and CP high level](files/A-coherent-theory-v1-env-body-cp-why.drawio.png)

* _**Some pathways of how the environment, body, and cognitive processes are leveraged to support the needs of the body.** Solid arrows indicate the most significant relationships, with dotted arrows indicating supporting processes._

**Environment:**
- The environment is a source of nourishment, of pleasure, and of danger. Some components of the environment (eg: family members) have a vested interest in helping the individual. While others (eg: predators and bacteria) have a vested interest in using the body of the individual in ways that would be detrimental to the survival of the individual.
- For most interactions the size and stability of the environment outweighs any ability for the individual to manipulate it. Thus the individual may manipulate the environment in a small localised way in order to meet the needs of the individual. The individually generally does not need to also consider the homeostatic needs of the environment itself. But in some situations the individual will need to consider the environment's homeostatic needs and act accordingly; for example to water the food crops before they die, or to act nicely to other individuals in order to keep them as friends.
- In the discussions that follow, we assume a simplified model whereby the individual acts in relation to the environment only in terms of their own immediate needs. But that is not intended to imply that those other important interactions do not exist.

**Body:**
- The body's most obvious actions are those that can be externally observed, such as those it performs via its limbs. The individual performs actions using these devices and in so doing changes the state of its body, eg: the left arm was hanging down but is now held upright. In some cases the action also changes the state of the environment, eg: by pulling a fruit from a tree branch.
- The body also performs more subtle actions, including using the eye and neck muscles to change where it is looking. In that sense, body actions can be performed due to some need that is more directly related to cognitive processes than to the immediate state of the rest of the body. These range from the innocuous (eg: idly looking around while day-dreaming) to the urgent (eg: looking to see whether the unexpected sound signifies danger). Thus, the body can perform actions that influence the cognitive processes. 
- Another kind of body action is the release of hormones by endocrine glands distributed around the body. These include the thyroid, parathyroid, thymus, adrenal glands, kidneys, pancreas, ovaries and uterus (females) or testes (males). As discussed earlier, for the purposes of the discussions in this article, hormones released from the brain are arbitrarily attributed to CP rather than to the body.
- Body actions are performed for a number of broad reasons:
  - to meet immediate homeostatic needs of the body excluding cognitive processes, eg:
    - the need to maintain body temperature near an ideal level
    - the need to maintain energy levels
    - the need to sleep when the body requires it
  - to meet immediate homeostatic needs of the cognitive processes (more on this later),
  - goals that the individual has decided upon, eg:
    - to seek a partner for procreation
    - to explore the far mountain
    - to build a hut

**Cognitive Processes:**
- Arguably the most important role of CP is to take all of the raw information obtained from sensory nerves distributed throughout the body, to infer the state of the body and the state of the environment, to infer the necessary body actions to take, and to coordinate the many body muscles and organs in the execution of those body actions.
- The brain also contains endocrine glands that produce hormones and which have direct impacts on both the body and the cognitive processes. These include the hypothalamus, the pituitary gland, and the pineal gland.
- But CP is now sufficiently complex that it has its own homeostatic needs. Eg: to stop unnecessary processing in order to minimise energy usage, to avoid chaotic processing for it's negative effects on learning, to stabilise attention control. In addition, the mind is complex enough that it can execute goals that don't directly involve the body - eg: solving maths problems for the sake of learning. 
- Jobs:
  - monitor and infer body state
  - coordination of body actions
  - release of brain-based hormones
  - infer and control mind actions to meet homeostatic and goal needs of body
    - monitor and infer cognitive state
    - infer and control cognitive actions to meet homeostatic and goal needs of body
    - infer and control cognitive actions to meet the homeostatic and goal needs of the mind
- So cognitive actions are performed for a number of broad reasons:
  - to meet immediate homeostatic needs of the body excluding cognitive processes
  - to meet immediate homeostatic needs of the cognitive processes
  - goals that the individual has decided upon

## System Interactions
![env, body, and CP interactions](files/A-coherent-theory-v1-env-body-cp.drawio.png)

* _**Environment, body, and CP interactions.** todo - description._

[Braindump] Points on above diagram:
- Body and CPs have their own homeostatic needs and in many cases this requires CPs to coordinate the necessary actions and other processes to meet those homeostatic needs.
- Individual's goals may relate specifically to something in the body sense (eg: "I want to move into the shade to cool down"), to something specifically in the CP sense (eg: "I want to be better at problem solving"), or have elements of both (eg: "I want to go to a cafe to study").
- The state of the environment is inferred by CPs based on information obtained via the 5 senses and from past learnings. Such inference has low certainty because the 5 senses provide only minimal information about the environment, and thus there are many hidden (unobserved) variables.
- The state of the body is inferred by CPs based on information obtained via the 5 senses, via internal senses such as proprioception and hunger, and from past learnings about the body. Such inference has a moderate certainty. The individual can act with high confidence regarding the broad high-level location and orientation of its limbs, for example. But the individual has very limited information about the internal workings of the body across its many scales. For example, often only a trained physician can identify the cause when an individual experiences pain within the area of the abdomen. There is significant room for variation on the amount of information that could be obtained about body processes, but not without cost. For example, any increase in information acquisition carries costs of a) extra energy expenditure, b) extra space taken up by additional nerves, c) extra processing capacity required in order to accurately infer based on the larger informational dimensionality. Thus the amount of information known about the body is a trade-off that is balanced through evolutionary pressures.
- The state of CPs are inferred through the meta-management feedback loop and from past learnings and modelling of the individual's own CPs. Like for the body, there is a trade-off associated with variations in the amount of information acquired about cognitive state. This is especially obvious for the case of CPs gaining information about themselves. The more CPs state that is acquired, the larger the brain must be to infer based on that acquired information. The larger and more complex the brain, the greater the amount of CPs state that might need to be acquired. Thus, necessarily, the amount of information obtained by CPs about their own processes is minimal, and the associated inference of that state carries only moderate certainty at best - something akin to knowing the broad high-level location and orientation of a limb, without knowing anything of the individual muscles, nerves, ligaments involved with holding the limb in that state.
- The level of control that the individual has over the environment is minimal, and tends to carry a high energy and time expense. Additionally, the certainty that an individual has that they will be able to obtain the desired environment state is low, eg: that a branch over their head will prevent rain from falling on them.
- The individual has full control over the state of their body, disregarding low-level molecular breakdown processes and quantum uncertainty. Most of that control is carried out automatically by the body without CPs, through localised biological processes controlled by DNA. A small selection of high order body actions are controlled by CPs. The level of energy and time expenditure associated with body control varies significantly, with most localised biological processes operating very efficiently, while some large scale outwardly observable actions requiring significant energy and time expenditure (eg: running). Those automatic biological processes probably have a fairly high accuracy in their ability to effect the desired outcome. On the other hand, the ability for CPs to control body state carries some uncertainty. Every action initiated via nerve signals from the brain occurs over a period of time and is affected by many dynamic factors, including: i) whether the individual is experiencing normal, above normal, or below normal levels of energy at the time, ii) whether some unexpected resistance is affecting movement of limbs (eg: tight fitting clothes), iii) uncertainty in the inference of body state, and iv) uncertainty in inference in the environment state that might affect body action (eg: an unseen stick that trips the individual while walking).
- The individual also has full control over the state of its CPs. Similarly for the body, many of those CPs are controlled in a localised manner. For example, there is evidence that raw optical nerve signals are initially normalised via an entirely localised process .......[citation and details]............ While the brain uses about 20% of oxygen availability within the body [citation], in general we can say that CPs are relatively effortless in comparison to large-scale body actions. Thus, it is usually more energy and time efficient to imagine many possible actions and their outcomes before choosing the appropriate body action, than it is to physically act out all of those possible actions. But CP effort is not negligeable. The level of certainty associated with a CP action is harder to quantify, but is probably relatively high.
- Environment, body, and CP state affect each other, leading to additional indirect pathways for the individual to control state of those systems. Body actions against the environment change the environment state, which can indirectly change the body state; eg: building a house to keep warm. CP actions against the body change the body state, which can indirectly change CP state, eg: turning away from a disturbing sight in order to direct attention away from it.

## Markov Process Modelling
With such significant differences between the behaviours, predictability, and level of control over each environment, body, and CP, a key feature of any models regarding them will be to distinguish between those three systems. For any given sense and associated inferred hidden state, whether that state is primarily associated with the environment, the body, or with CP has a significant impact on how certain the individual can be about the accuracy of the inference, and about the likelihood that the individual will be able to change the hidden state to a more favourable one.

That information is of particular relevance to meta-management processes. In order for meta-management processes to operate efficiently, they need to operate against a higher-order approximation. Some investigation into how those processes may operate illustrates this point.

An agent observing and interacting with an environment can model that environment with a markov process such as illustrated below in panel A: a set of `n` actions are possible, and many combinations are possible. Those actions influence `j` hidden states in complex ways. The agent make makes an observation containing `q` features. Each of those components have very large cardinality. Each individual effector nerve in the individual can lead to a range of actions in continuous space, depending on the frequency and strength of its spike train. The observations are made up of thousands of individual nerve signals. And the hidden state space is potentially enormous. For training of fine-controlled muscle movement, with actions inferred from high precision visual, tactile, and audial sensory information, that scale of modelled markov process is appropriate. However, for higher-order monitoring, rationalisation, and inference of required adjustments, that level of granularity would overwhelm any process that needs to simulate outcomes and consider alternatives. More importantly, that fine-grained level of granularity is unnecessary.

Thus, it is more efficient to apply a high-order re-modelling. In a slight simplification, that can be conceived of as grouping the low-level parts of the modelled markov process as indicated in panel B. That results in a much simpler higher-order model, represented in panel C. For example, our touch sense is really millions of independent nerve endings, but within our conscious perception we think about touch as a single state space with location, texture, amplitude and valence being parameters instead of low-level individual points.

![markov modules](files/A-coherent-theory-v1-markov-modules.drawio.png)

<ul>
<li style="list-style-type: none;"><i><b>Markov process modelling.</b> Actions `a`, hidden state `h`, and observations `o`. Lower-case letters refer to low-level fine-granularity, while upper-case letters refer to higher-order abstractions. `m << n`, `k << j`, and `p << q`.</i></li>
</ul>

As an aside: its worth noting that it is likely not just meta-management processes but higher-order planning as a whole that operates at this higher-order level. So while precise control of limb movement, for example, may require the more detailed modelling; overall coordination of actions across the body and CP probably operate a higher-order level.

## Identification of Source
So, meta-management operates against a higher-order representation of action, observation, and hidden state spaces. It is also needs to partition those spaces by their mutual level of interaction (aka mutual information).

Actions in the CP space have no impact on the environment. Actions in the body space influence the environment and the body, and have varying levels of influence over the CP space. Thus, when inferring the best action to take to apply a correction against a non-ideal state, the individual needs to model which modalities of actions are effective against different modalities of state.

Thus the higher-order representations have a strong segmentation between environment, body, and CP in both state and action spaces. Effectively, any sensory information that reaches the attention of higher-order executive and meta-management processes will have a sort of labelling associated with it to identify its source. Events that occur in the environment are labelled as occurring external to the body. Events that occur within the body are labelled as such. Events that occur within CPs are correspondingly labelled.

## Schema
_todo: flesh out:_
- body schema
- cognitive schema

## The Ego in "I"
_todo_

In combination with body schema and cognitive schema, labelling of events leads to a strong association between an event and the schema of its source. So, when I think a thought and subsequently think about having that thought, I know that "I" had that thought.
    
_Identity_ is better thought of here as an identification of _independence_. The "I" that refers to me as a whole individual, enables my cognitive models and processes to apply different strategies and belief models to my own state and actions than they would apply to the environment around me. More internally, there are distinctive differences in what can/cannot be observed and changed about my body vs my cognitive state. Thus there is a lot of value in creating an _identity_ for the cognitive state - overlaying a virtual boundary around that cognitive system. Stuff within that boundary can be modelled and changed independently of other things.

## Emotions
_..todo..may need to cover off emotions too, because it turns out that they're a form of MM too_

## Meaning Attachment
_todo:_
* Summarise all of above with the term "meaning attachment" so I can use it later on to refer to all of:
    * labelling
    * emotions
    * relationship to schema

# IV.3 Deeper Dive into Control Process Learning

By the end of Part III it was clear that complex multi-iteration control processes require meta-management, and we were able to identify some possible architectures that capture the interaction between control processes and meta-management, but we are left with an outstanding question: how do we identify which meta-management architecture is more likely in humans? The question is important to our end goal because, as will be seen, the answer impacts our ability to explain subjective experience.

To my knowledge, there is no research investigating the relative merits of the proposed possible meta-management architectures within the context of connectionist computational architectures. At this stage, drawing any conclusions from the empirical evidence of neuroscientific data is fraught [citations for general problems of conclusions from fRMI data, or the history of mistakes?]. Thus we are left to postulate based on theoretical analysis._

So, in order to answer that question, we shall now look at learning in humans.

The controversies surrounding meta-cognition research stems from one problem: that it's not just one system that controls meta-cognitive processes. The meta-cognitive research discussed above generally acknowledge two systems: first-order non-conscious processes and high-order conscious processes. Debates about whether a behaviour is meta-cognitive or not hangs on an assumption that only conscious processes can be classified as meta-cognitive. We can avoid getting caught up in such debates when we acknowledge that all behaviour is an outcome of interactions between all systems. What we need to investigate is what those systems are, their underlying mechanisms, and how they interact to produce that behaviour.

_..todo..introduce concept of layered architecture with: i) innate, ii) habitual, iii) rational systems._
_...todo : there must be lots of research on this already.....review that and then write this section._
_...can also introduce Daniel Kahneman's System I and II Thought._

![three systems of control](files/A-coherent-theory-v1-bio-3-systems.drawio.png)

* _**Three Systems of Control.** Innate control and innate feedback interpretation bootstrap learning of habitual and rational systems. Habitual and rational systems interact in order to produce learned behaviour._

Experience informs us that any attempt to classify biological processes into discrete categories is fraught with ambiguity because biological systems do not subscribe to such simple classifications. Nevertheless, the classifications will help our current endeavour, so beware in taking the distinctions between these classifications too literally.

## Innate Control
The _innate control system_ is driven by genetics and is in place at the time of birth. It varies throughout the life of an individual due to biochemical developmental processes, but does not incorporate learning. The innate control system incorporates only the most primitive control mechanisms necessary for sustaining life, for example: reflexes, thermo-regulation, heart-rate, hormone release. It also incorporates primitive sensory interpretation, for example: pain is to be avoided, pleasure is to be sought out, hunger necessitates action, and satiation permits relaxation.

The innate control system bootstraps development of more advanced systems such as habitual and rational control. It does this in three key ways. Firstly, it prevents untrained habitual and rational systems from causing the individual harm through incorrect action or through inaction. For example, the reflex to flinch and withdraw from pain is so powerful that to counteract that reflex requires an individual to carefully coordinate calming effects against the parasympathetic nervous system and tensing of counteracting muscles. Likewise, young children are often unable to prevent themselves from taking food when they have been told to wait. Habitual and rational systems can counteract innate control, but  only once they have reached sufficient maturity.

Secondly, the innate control system participates within the training of those more advanced systems through its interpretation of primitive feedback signals such as pain, pleasure, hunger, and satiation. The more advanced systems learn through reinforcement learning by seeking to maximise the integral of positive valence interpreted by the innate control system.

Thirdly, it likely provides additional primitive feedback in the form of indications of energy and time cost that should minimised by reinforcement learning. Any action should be carried out in the most energy conserving way - don't use more muscles than necessary; don't tense counteracting muscles so that motion is difficult and more effort required than necessary. Mental processes should produce effective outcomes quickly.

## Habitual Standard Control
The _habitual control system_ simply replays common behaviour that it has learned through repeated experience. Notice that now this article is focused on biology, and humans in particular, I use the term "habitual". But I am clearly referring to the same thing that I called "reactive control" when being agnostic to the kind of agent involved.

_todo: following diagrams is too concrete and implies an unrealistic architecture_

![Habitual standard management](files/A-coherent-theory-v1-habitual-std-mgmt.drawio.png)

* _**Habitual System.** ...todo...._

Initially, learning is driven by environmental and body feedback that is interpreted by the innate system. Pain signals are interpreted by the innate system as negative feedback, and used to effect neuronal weight changes that reduce the likelihood of that same behaviour in the future. Satiation following hunger is interpreted as positive feedback and likewise used to effect neuronal weight changes, but in order to increase the likelihood of that behaviour.

For more complex situations, the rational system influences behaviour. As those more complex situations are repeatedly encountered, the habitual system learns the new behaviours, freeing up the rational system for other things. In that way, habitual system learning is driven by a combination of bottom-up pressure from the innate system, and from top-down pressure from the rational system.

Significantly, habitual learning is slow. A habitual system alone would be unable to produce the kinds of rapid adaptation that we see in humans.

## Rational Standard Control Management
The _rational control system_ is significantly more elaborate than the habitual system. It's purpose is to enable rapid adaptation through high-level modelling and reasoning.

Our knowledge of rational processes in humans is still in its infancy, and as such we can only guess at the underlying mechanisms. In order to motivate some of the discussion that follows I shall hazard a guess at some of its features, illustrated in the diagram below. As discussed above already, control processes must utilise multi-iteration processing, and I believe that is a key part of the rational system. As part of that multi-iteration processing, I suspect it also learns a repertoire of strategies for navigating CP state space given different problem domains. It incorporates short term and long term memories. It incorporates modelling of other systems, in a way that it can somehow incorporate new information from few or even a single example. And it includes the ability simulate and examine environmental, body, and mental behaviours without actioning them.

The product of the rational system may be a goal selection that is then applied against habitual processes in order to actually produce the desired behaviour.

![Rational standard management](files/A-coherent-theory-v1-rational-std-mgmt.drawio.png)

* _**Rational System.** Some of the features that might underlie rational thought._

The learning processes within the rational system may be very complex. While for any given problem domain the models that it operates against are likely very high-level and efficient, and thus require only a few neurons, the brain mass required to operate such an elaborate and adaptive system is likely very large. ......_todo: details of suggested parts of brain involved and percentage of brain neuronal mass_... Correspondingly, while in a well developed brain the training required for any given problem domain may be small, the training required to reach a point where the rational system is effective may require a very long time due its overall complexity. In early infancy, the rational system is likely extremely chaotic. I expect that developmental processes attenuate the rational system during the infant period of a baby's life.

In that way, the rational system may be "held to account" by i) the innate system, which prevents the rational system from sending the individual outside of a safe operating range, ii) developmental processes, that only let the rational system take control once it is ready to do so, and iii) the habitual system, that actually carries out most actions and which is itself constrained by innate feedback mechanisms.

## Habitual and Rational Control operating together
Daniel Kahneman describes thought as operating within two "systems" or as two modes, namely _System I_ thinking and _System II_ thinking [citation]. System I is rapid and occurs without conscious involvement: a conclusion merely becomes available, apparently without any deliberation. In contrast, System II is explicitly deliberative: with subjective experience of individual steps as thought progresses from problem to solution. System II thought is significantly slower than System I thought. It is no surprise, I think, that the ideas of System I and II thought map conveniently onto the ideas of habitual and rational control, respectively.

One key point of Kahneman's work is that each system has different strengths and weaknesses, and that we benefit by the aggregate of the two. System I decisions are great for quickly choosing which toothbrush to buy in the supermarket - there's way too many options available now, and at the end of the day they all do the same job almost to the same degree of effectiveness, so there's no point stressing oneself out choosing the "best" toothbrush. But System I decisions cause us to repeat our past behaviour even when those behaviours have been proven to be "bad habits". System II thought enables us to cope with novel situations that our System I thought is not sufficiently trained to cope with. It also enables us to counteract our bad habits by considering the same problem from multiple angles and by only making a decision when we are confident that we have deliberated sufficiently. Conversely, System II thought is too slow when danger looms and a quick decision is needed between flee or fight, or of where to flee to. Additionally, System II thought is resource intensive - it consumes a lot of energy, it involves many brain regions (potentially preventing those involved brain regions from serving the needs of multiple parallelised System I activities), and it is slow. Thus System II thought carries a significant _opportunity cost_ - for any deliberation that we are currently involved in, there are countless alternative uses for the brain's resources that might have provided greater benefit to the individual.

There are two takeaways from that analysis:
1. System II thought is expensive, so use System I thought as much as possible.
2. System I thought makes mistakes, and the job of System II thought is to take over when (or before) that happens.

Where you have two independent systems, with one (or even both) producing errors at times, and you want to maximise the likelihood of "valid" behaviour, a productive technique is to make these two systems compete. This is used very effectively in AI research, where it is known as an _adversarial network_, or in its more common specific use case as a _Generative Adversarial Network_ (GAN) [citation]. Here, you have have two ANNs: the _generator_ network and the _descrimator_ network. The generator network attempts to generate novel output in some particular format (eg: an image) that mimics the characteristics of real world data as closely as possible. The descriminator network is supplied some data that either came from the real world, or was generated by the generator network. It's task is to determine which. The two networks are trained in tandem via so-called "loss functions" that guide the generative network to improve at mimicking real world data and that guide the descriminator network to improve at telling the difference between real world and generated data. Thus, in the framing of the original design for GANs within AI research, the two networks compete in the following way: the generator tries to trick the descriminator network that it's producing real world data, while the descriminator tries to catch the generator out.

There is a different way of looking at this design that is more instructive for our purposes. The generator network is tasked with producing useful output. It operates in a _reactive_/_habitual_ way, blindly producing output according to behaviour that has been trained into it through many repeated trials with associated feedback. It makes mistakes sometimes. The descriminator network is tasked with identifying those mistakes. When the generator network produces an output and the descriminator network identifies no significant error then the generator output is "good" and can be applied to whatever end it is intended. In contrast, when the descriminator network identifies a significant enough error, some intervention is required. The elegance of this solution comes not just _despite_ the fact that both networks will produce errors, but rather _because_ both networks will produce errors. The key is that while the overall problem space is the same, the exact tasks that the networks are trained against are different. So the networks themselves are different, and thus they will produce different errors at different times.

This is beautifully compatible with the description of habitual and rational control so far. The habitual system learns to repeat behaviour. It does this efficiently, requiring minimal cognitive resources to operate. In familiar situations the product of habitual control is effective - ie: it has positive utility for the individual. But in order to identify the need for intervention, a descriminator system continuously judges the output of habitual control, looking for any behaviours or outcomes that are not effective. As the operation of the descriminator system is different to the primary habitual control system, it will not produce errors in the same situation, and so it will be effective at detecting non-effective habitual control outcomes. When errors are detected, the rational control system takes over - through some unknown means that we won't attempt to discuss here.

The descriminator system itself is not necessarily a reference to the rational system. Indeed, it may operate in an entirely habitual/reactive way just like for primary habitual control. If we're trying to apply dumb categorisation, then it falls quite squarely into the camp of meta-management. But rather than an overly simplistic categorisation, this descriminator system has a number of key qualities that we have seen in meta-management before. This form of error-detection is not just applicable to external behaviour, but is equally necessary against the internal state trajectory of the control process. Thus it needs to _observe_ the behaviour of the primary habitual control system, including its CP state and state trajectory. But if that internal state is held as micro-recurrency within each neuron, then in order to process that state while avoiding an infinite regress on network size it needs a dimensionally reduced summary. In other words, a descriminator network needs a meta-management feedback loop.


# IV.4 Deeper Dive into Meta-management
points:
* domain knowledge, complex, lots of neural mass
* domain knowledge at time of meta-management same as domain knowledge in effect within CP at that time, so if there is any mechanism that "loads" domain knowledge in order to hold it is context during execution, then that same domain knowledge may be at play in both systems.
* rational system can model outside world concerns; can also model internal concerns, such as needed for meta-mgmt
* some components of rational system are probably implemented through habitual mechanisms
* conclusion: inline meta-management with meta-management feedback loop
* what exactly does it incorporate?
    - ......have I repeated that already?

So, the brain leverages both habitual and rational mechanisms in order to strike a balance between their relative strengths. Habitual systems are slow to adapt, but efficient to execute. Rational systems are fast to adapt, but complex and slow to execute. Independent habitual systems seem to be distributed throughout the human brain, as multiple habitually controlled behaviours can be executed simultaneously, eg: talking while driving. In contrast, there appears to be only one rational system, which can only operate against one task at a time.

What differences are there in the meta-management of these two different systems? Might meta-management itself also employ both mechanisms? And does that help us identify the architecture of meta-management?

As we proceed, remember that by the definitions as they stand, standard control is related to how the individual governs actions against their body and the environment, whereas meta-management is related to how the individual governs the execution of the computational processes involved with the former. If, by the end of this section, you are beginning to suspect that this distinction is somewhat arbitrary, then you will be well towards grasping one of the key points of this article.

## Components of Habitual and Rational Meta-management
Habitual mechanisms could well help to solve meta-management needs. _Habitual mechanisms of meta-management_ (HMMM) would be an individual's learned automatic behaviours with respect to meta-management. Some examples might include:
* Higher-order production and interpretation of feedback. Providing more frequent feedback for RL algorithms. Providing better understanding of feedback with broader contexts. Influences: habitual standard control, rational standard control.
* Strategy execution within rational system -- it's meta-management, but it's implemented through habitual mechanisms.
* Strategy selection within rational system - will be a mixture of habitual and rational meta-management, depending on familiarity with problem domain.
* detecting when habitual standard control behaviour has resulted in unexpected outcomes that require rational systems to take over in order to correct the situation
* Learned meta-learning behaviours - observed by others as an individual's position on the sliding scale of "learning mindset" to "fixed mindset".
* ..others..

Rational mechanisms are equally important for meta-management. _Rational mechanisms of meta-management_ (RMMM) would leverage all of the higher-order modelling and deliberative capabilities discussed above. Some examples might include:
* modelling the behaviours of the standard control processes, including tracking of their abilities (in other words, effectiveness) against different problem domains.
* deliberative selection of problem solving strategy based on above modelling
* domain knowledge, complex, lots of neural mass
* domain knowledge at time of meta-management same as domain knowledge in effect within CP at that time, so if there is any mechanism that "loads" domain knowledge in order to hold it is context during execution, then that same domain knowledge may be at play in both systems.
* In short, this is all the most advanced meta-learning, meta-cognitive thought processes that we can think of. This is the magic sauce that enables abstract thought.
* other examples (but be careful to avoid just replicating what's already in other lists:
    - noticing repeated states/sequences of states that indicate _stuck thought_.
    - associative memory to shortcut via memo-isation.
    - modelling and observing CP strategies: if CP is currently using a weaker strategy and it is floundering, then MM can detect that and encourage to use an alternative strategy.
    - modelling and improving CP strategies: choosing to use a weaker strategy in order to improve it.
    - modelling and selecting CP strategies: choosing to use the strongest strategy in CP according to a particular problem.
    - meta-mgmt is effectively a big part of the learning against CP.
    - loss-function rewards: using higher-order / domain knowledge to measure CP performance & apply as loss function -> mm acting as part of learning algorithm.

_todo: review other lists, eg from my notebook._

## Reusable Domain Knowledge

..todo..

## Summary of Meta-management Architecture
_todo: avoid temptation to relate this back to subjective experience. That'll come in the solution part._

We are now finally in a position to place our bets on the most likely architecture of meta-management, that of _inline meta-management_, incorporating both habitual and rational systems.

diagram: habitual with standard + meta-management intermingled, rational with standard + meta-management intermingled.

# IV.4 Distinguishing Meta-management from Standard Control
Things are getting blurry. At first I claimed that meta-management is something entirely different from standard control. Now I claim that there is no independent meta-management system. And to top it off, I'm also claiming that the same functions and even states associated with standard control can be re-used for meta-management. So is meta-management in any way distinct from standard control?

The answer to that question is nuanced. I believe the best answer is that some aspects of meta-management and standard control differ significantly while others have very close coincidence. Thus I consider them as separate processes that are superimposed and intermingled within the same system.

I will make this case by looking at three aspects that I believe do differ considerably between standard control and meta-management: state representation, pathways, and learning.

## State Representation
The state of the standard control process, as used as part of its computations for action decision, is considerably different to the state of the standard control process as used for meta-management. The most significant differences are in terms of context. 

Consider the biologically plausible planner introduced earlier. The state that it would hold and use in its computations would be focused on the specific problem at hand at the time, for example:
- the results of simulated real-world trajectories already attempted
- factors related to generation of new real-world trajectory simulations yet to be attempted
- factors helping to decide whether to continue to search for better real-world trajectories or to settle on the current best guess.

In contrast, the state information required for meta-management of that same planner has the planner itself as its target of representation:
- the computational state trajectory of the control process itself (ie: the three bullet points above, together, form a single point in the computational state trajectory), including how long it has been running for on the current problem
- the class of problem that the control process is currently operating against
- modelled information about how effective the control process is against that class of problem
- indication of whether the control process is currently trending towards finding an effective solution
- indication of whether the control process appears to be repeating any past observed behaviour that required intervention

Further to that. Meta-management processes can model not just past observed behaviours (of the control process), but expected future behaviours. For example, through teacher instruction and by observation of others, an individual can develop a model of how good they _should be_ at a particular task. This is clear, for example, in students comparing their results on a maths test and in a parent scolding their child for doing badly on said maths test. So the meta-management process not only observes the state of the control process, but generates additional state information in the act of comparing the current behaviour of the control process against past actual behaviours and future possible behaviours.

The distinction is best summed up in colloquial vernacular: that a standard control process represents its state "from the inside", whereas meta-management represents the state of the control process "from the outside".

## Pathways
For a standard control process, its "state" is just a concept that the scientific community apply against it as a way of understanding its operation. We know that its behaviour for the same input will be different depending on the sequence of past inputs. We explain to ourselves that the process itself must be somehow affected by that sequence of past inputs. And we summarise that as a) the process has a state, and b) the state of the process changes as processing occurs. Importantly, there is nothing said about the representation of that state, nor of the underlying mechanics of how that state is "held".

Our understanding from neuroscience is that state in brains is held in the form of recurrency: results at various layers are fed back as inputs at earlier layers [citation]. That feedback can occur with different lengths, anywhere from each individual neuron holding onto its own state to outputs at the final nodes being fed as inputs into the earliest nodes. Captured in panel A in the diagram below.

![state pathways](files/A-coherent-theory-v1-state-pathways.drawio.png)

* _**State pathways.** A) Short-path and long-path recurrency of immediate state in standard control. B) Long-path recurrency of state plus context in meta-management._

In contrast, meta-management processes require an explicit representation of the control process state. That representation is most likely constructed through a pathway that has the express purpose of generating that very representation from various sources. The sources include some kind of cache or accumulative representation generator of CP state trajectory plus information obtained through comparison with models of past and expected behaviour.

As mentioned earlier, to represent the state held by every neuron within the control process would lead to an infinite regress in the scale of the system.....todo....


## Learning
- learning pressure: standard control representations trained to accurately represent the problem state w.r.t. the mechanisms needed to solve them. Rational control representations trained to represent all of the inner workings with the minimal amount of information needed to attain sufficient stability.


# IV.5 Semiotics
The claim so far is that the meta-management feedback loop generates a (high-level, and filtered) representation of the state of the goings on within the brain. That representation is then available for processing, which may produce some computational actions as part of meta-management. Assuming an inline meta-management architecture, a logical extension is that the outcome of that meta-management processing result in]s new state that is subsequently captured by the meta-management feedback loop and fed back as a new representation.

This description begins to mimic what we'd expect of the basis for subjective experience: it provides a self-referential observation, along with a choice about simply observing or reacting to that observation. But the meta-management process only has a few basic things going on: capturing of data, generation of a representation of that data, processing of that representation, and generation of actions in response to that representation. Which of those could possibly produce subjective experience?

The answer is that it's all of those basic steps, taken together, and repeated over and over. But to explain that clearly we need the right language to talk about it. The language that will help us is that of _semiotics_: the study of signs and their interpretations.

## Objects, Representations, and Interpretations
Semiotics studies signs, meaning making, and the processes involving them. There are different formulations but the one that we shall use is through the triad of _Objects_, _Representations_, and _Interpretations_.

![components of semiotics](files/A-coherent-theory-v1-semiotics.drawio.png)

* _**Components of Semiotics.** Semiotics identifies three components to communication and meaning-making: the original object, its representation, and the interpretation of that representation. For good communication, the interpretation should closely resemble a re-construction of the original object, or at least a mental image of the original object. In that sense, the interpretation is itself just a representation._

**Representation.** Also known as a _signifier_, _representamen_, _sign-vehicle_, and just _sign_. A representation is anything that does or could communicate meaning through some aspect of its presentation. It can be of any form, eg: visual, auditory, tactile, electrical, or as some kind of virtualised information. Three forms of representation are typically identified. _Icons_ share some important quality with the object that they represent, such as by bearing a direct resemblance to that object. For example a cartoon picture of a lion represents an actual lion through nature of resembling the appearance of a lion. _Indices_ share some linkage of fact with the object, such as through a causal relation. Smoke represents fire because fire causes smoke. _Symbols_ represent their objects through conventional or cultural knowledge, and unlike the first two have no natural relation to the object that they represent. For example, in phonetic languages (and semi-phonetic languages such as English) written characters represent the sounds they make, not because there is any resemblance in the way that the characters look to the way they sound or because the shape of the characters are somehow caused by their sounds, but because we've all agreed to the convention that these characters make those sounds.

**Object.** Also known as the _referent_, the object is the underlying thing or concept being represented. For example, the lion, the fire, the sounds that written characters make. It may be some simple physical thing, or be a deep and broad concept, or a thought.

**Interpretation.** The interpretation or _interpretant_ is the meaning obtained through the act of interpreting or translating that representation. In some cases the representation exists with the intent to convey the original object as the interpretation. For example, a stop sign on the road is a representation erected with the intent to be interpreted to convey the concept of the original object: all of the traffic rules around stopping at stop signs in order to prevent accidents. In other cases the object and interpretation are different. This is particularly the case for physical objects. For example, the interpretation of smoke is that a fire is present, it does not clone the original fire within the mind of the person seeing the smoke. Likewise, the interpretation of the word "lion", elicits the recall of the hearer's conceptualisation of a lion. That conceptualisation is itself just a representation, and depending on other contextual information available, may or may not be very accurate in relation to the particular lion that the speaker was referring to.

A few points are worth drawing out.

The representation is an informational bottleneck. The object typically has far greater detail and nuance than is ever captured by a representation of it. A cartoon image of a lion captures only a superficial resemblance to the outward appearance of a real lion, omitting all of its internal biological structure, its behaviour, and the fear induced in someone who hears it roar. The varieties of intentions behind the single spoken word "happiness" far exceed  the informational qualities of the sound waves that represent it to the listener. Indeed, in many cases the purpose of a representation is that it indicates the object without consuming the same physical and informational resources as the object it represents. How short our life would be if we needed to explain to a friend that a lion is approaching by explaining in minute detail every molecular property of all the cells in the near (and approaching) vicinity.

If the object is a detailed and nuanced entity with high physical and informational bandwidth, and the representation is a bandwidth bottleneck, the interpretation can be viewed as an up-scaling of bandwidth through re-construction. This requires that information be added, where should that information come from? An example will help.

While driving, it is common to see signs that indicate that certain traffic features are ahead by some distance, such as an intersection. Often the features themselves are around a corner out of sight, and the only information one has about the approaching feature is within the sign that says "Intersection ahead, 500m" - an informational bottleneck. At the moment of observing the sign, the rest of the information comes from the observer's own knowledge - of the road rules involving intersections, of past experience with intersections, and perhaps with memory of that specific intersection. 

So the full construction of the interpretation is a little bit from the sign, and a lot from the individual doing the interpretation. In other words, interpretation requires an _interpreter_.

Moreover, the particular interpretation obtained from a representation depends on the knowledge and disposition (a.k.a. state) of the interpreter at the time. As example, consider the thumbs up hand signal illustrated in the following diagram. A thumbs up hand signal can mean several different things. When used in conversation or while interacting with social media platforms, it can mean that you appreciate or support the statement made by someone else. When used while standing on the side of the road it can mean the request for a ride. And in some cultures it makes a sexual reference intended as an insult. 

![thumbs up](files/Paper-on-Loops-in-AI-and-Consciousness-semiotics.jpg)

All of these issues with informational bottlenecks and misinterpretations arise because the object is unknown at the time, or even ultimately unknowable in a practical sense. When smoke is observed in the distance, you do not have any other information about the object itself at the time. But it is possible to move closer to investigate and learn more about the source of the smoke. Conversely, when someone speaks, they are translating (representing) the complex sequence of ideas and thoughts within their mind. While it is possible to ask questions and gain more information, it is practically impossible to know every nuance of those original ideas and thoughts within the mind of the speaker.

Semiotics provides a tool for understanding meaning-interpretation processes in different domains, regardless of whether those domains include obvious signs. Today semiotics is used in many fields, either explicitly or implicitly. It can be said that medical diagnosis is the act of interpreting a sign (the symptoms) in order to identify (diagnose) the original object (the underlying condition) (Burnum, 1993; Nessa 1996). It is used extensively in marketing to understand what meanings people are likely to add to different messaging (Borţun & Purcarea, 2013). A listing available from the Wikipedia page on [Semiotics](https://en.wikipedia.org/wiki/Semiotics) indicates specific sub-fields for biosemiotics, cognitive semiotics, computational semiotics, literary semiotics, cultural semiotics, social semiotics, and many more.

The study of Semiotics has a long history, but it's modern structure is most commonly traced to the works of Ferdinand de Saussure and Charles Sanders Peirce. Peirce was the first to introduce it via its triadic formulation. It is informative to note that in Peirce's earlier works he was focused on semiotics as the process underlying cognition (Peirce, 1982, vol 2, pg 56, 213). To that end, Peirce supported an idea of _infinite-semiosis_ within the mind: representations being interpreted, producing new representations that need to be further interpreted, and so forth. This is convenient to us, as it is an idea to which we shall now turn.

## Infinite semiosis
The examples mentioned above describe single iterations of a semiotic process: an object exists in some way, a representation of the object is presented, an interpreter constructs an interpretation based on the representation. Infinite-semiosis is the continued execution of the semiotic process, with the interpretation itself becoming an object that must be represented and further interpreted. Infinite-semiosis is not necessarily infinite in an absolute sense, and in practice never can be, but that the process is in principle capable of continuing "for a long time" before it breaks down in some way.

A fascinating and informative example comes in the form of the life sustaining processes surrounding DNA replication.....

_todo_

...Lessons:
* interpretation doesn't require a "cognitive entity"
* representation is nothing without interpretation, the interpreter is nothing without the representation.

Things get a little more nuanced when you look at computational semiotic processes in connectionist paradigms. When the entire brain is a massive multi-layered network involving many different kinds of processes, some of which talk to each other in some way, but all part of a single larger system, where are the boundaries of object, representation, and interpretation? One answer is that the brain involves many objects, representations and interpretations, layered in deep hierarchies. But more generally, the lesson is that semiotics is a tool. The concepts of object, representation and interpretation help us to understand processes as they occur, and we can apply the tool to whatever layer or part of the process that we need.

As a first example of semiotics in the brain, consider how the body gathers and interprets information about the environment, illustrated in the diagram below. The environment is the _object_, and its true state is what the individual hopes to attain knowledge of. But the individual will never gain such knowledge as they do not directly perceive the environmental state. Signals obtained from the classic five senses of sight, sound, smell, touch, taste _represent_ the environment. That collective representation captures only a narrow and shallow aspect of the true state of the environment. For example, our visual sense only reports on a small field of view at any given time, and that too only about the external surface of whatever thing is being looked at. That representation is interpreted by the network of brain neurons, producing an inference about the state of the environment. What form does this inference take? Millions of _spike trains_ [citation] in some particular pattern of activity.

![sensory semiotics](files/Paper-on-Loops-in-AI-and-Consciousness-env-semiotics.jpg)

Those millions of spike trains are not an end to themselves. Spike trains that went only to dead-end neurons would result in nothing happening. Spike trains are themselves just a representation, and thus must be interpreted.

In order to respond to the environment, the individual interprets those spike trains by applying knowledge of the environment and of the individuals own body. The resultant interpretation: an action plan that is sent as further spike trains via effector nerves to muscles. Or perhaps the individual simply chooses to think more about the environment. Thus the semiotic process forms a repeating cycle of representation and interpretation, as illustrated below. This plays out in the communication between brain regions. It also plays out at the whole system level during multi-iteration processing.

Importantly, spike train representations have the same informational bottleneck effect as discussed earlier. For example, if we consider some localised region of brain, whatever processing that occurs is through the activity of many layers involving hundreds or thousands of neurons. The activity of those neurons, and the synapses between them, is potentially impacted by dynamic static held within the neurons and synapses. In contrast, only a small subset of synapses convey messages to other regions of the brain. Whatever region receives those messages re-constructs meaning through the addition of its own knowledge - knowledge that is inherent through its structure and the learning processes that have tuned it throughout the individuals lifetime.

![cognitive semiotics](files/Paper-on-Loops-in-AI-and-Consciousness-brain-semiotics.jpg)

One question arises. Where is the object in such cyclic semiotic processes? From a computational point of view, the question is not an interesting one as the processes will continue to function regardless of how we understand them - after all, semiotics is just a tool for analysis, rather than a statement about how the world must be. But perhaps from a philosophical perspective we may gain some extra insight, or at the least another reference point for further discussion. From the outside world we have the example of a real physical lion, a cartoon image representing it, and the mental concept created in the mind of the interpreter upon seeing the cartoon image. The object, the lion, is a thing that exists and has a reality extending through time. In a multi-iteration cognitive semiotic process, the object of the next iteration is the interpretation of the current interpretation. But even the interpretation seems nebulous.

The discussion one paragraph before gives the example of a brain region producing a spike train representation that it supplies through its synaptic connection to other brain regions. That is a representation of its interpretation. Where is the interpretation? The interpretation never exists. At least, it never exists as a single whole entity with all its component parts being present at the same time. Rather, as the individual neurons fire, performing their individual proto-computations, they construct individually some small part of the whole interpretation and then immediately forget it. The immediately next neurons pick up from there and construct, individually again, other small parts of the whole interpretation. At the same time, each synaptic connection between individual neurons supplies only a spike-train representation, as part of a semiotic process at a finer level of granularity. By the time that the wave of neural activity reaches the edge of our arbitrarily chosen brain region, only the finer-grained representation of the final outgoing synaptic connections exist.

So, in computational infinite-semiosis, objects are past interpretations, but interpretations are nebulous and exist only as the sequence of activities spanning many neurons over a course of time. And representations are no better - they exist only as a sequence of electrical spikes, spanning many synapses, over a period of time. More brutally, in computational infinite-semiosis, at any given instantaneous moment in time, nothing ever exists in its complete form except the interpreters with their background (learned) knowledge ready to be applied as representations pass transiently through them.

## Semiotic Analysis of Control Processes
_todo_:
* what semiotics tells us about the architecture of standard control -> no self-interpretation loop
* what semiotics tells us about the meta-management architecture -> self-interpretation loop

_..todo..would it work better just calling these examples?.._

I shall now return to the question of control processes and meta-management, by examining them in terms of semiotics. I shall present three examples of processing, and in so doing we will see that their objects, representations, and interpretations have some important differences:
* body action control
* task-focused CP state trajectory control
* meta-learning

In any computational processing, the purpose of the process is to produce its result. In evolved systems, the information made available to the process is partly a result of the needs of the process to produce those particular results. We shall mirror that fact by working backwards from the interpretation to the object. For this exercise, we will define the interpretation produced by a computational process as the _effect_ of processing: any changes to state, any actions that are triggered by the process, and any new representation that it makes available for subsequent processing. We will consider the representation to be the synaptic signals received by the process in question. The object is the (mostly unknowable) state of the thing that the process is "focussed on" - ie: the thing that the processing attempts to understand in some way in order to produce appropriate results.

### Body action control
For control of body actions via a multi-iteration control process, we can look at habitual and rational processing separately. The generated interpretation by habitual processes are simply the outcomes that we'd expect of a body control process: body actions that affect the state of the body and the environment around it, plus CP state updates as it executes its multi-iteration processing.

Interpretation from rational processes is a little more interesting. It includes modelling of the problem space for later use (ie: modelling of environment and body), deliberative outcomes in terms of environment and body, strategy selection with regards to the overall type of response required against the current environment/body problem (eg: the individual is getting wet in the rain, so built a hut or find a cave), and body actions. 

To make that work, the habitual and rational control processes require information about the environment and body. This includes knowledge about their dynamics. Furthermore, the more the individual knows about the future of the environment and body, the better it can make decisions. These are the attributes of the object.

Notice that the object is dominated by state that the individual needs but will never have, or will only have after the fact. This is a feature of the object in any semiotic system where the interpreter must learn about the object from scratch (more or less). We gain wonderfully complex and nuanced understandings of the world around us and of our own body through experience and through education. But the truly amazing thing about that learned knowledge is just how little we have and yet manage to survive.

The representation presented to the standard control process includes the individual's raw senses that sample some practically insignificant portion of information about the environment and body. It includes those learned approximate models of the dynamics of the environment and body produced through prior interpretations. And it includes working memory, for example so that a given aspect of state can still be responded to even when no longer in sight.

### Meta-management of CP state trajectory
For meta-management of the state trajectory of a multi-iteration control process, the generated interpretation most predominantly includes some action that affects the CP state trajectory. This could be through any of the mechanisms described in section III.3, including but not limited to direct state manipulation, adjusting bayesian biases, or through manipulation of input signals to the control process.

Arguably another form of meta-management against CP state trajectory includes directly initiating body action. This can be seen in the example when someone consciously chooses to avert their eyes to aid in distracting themselves from a thought that was associated with the previous visual scene (as opposed to an instinctual revulsion aversion response).

The object in this case is the control process as it performs processing against a particular task. That includes its state, the trajectory that it has taken, and its progress in relation to the task. The object also includes the CP state trajectory that it will take going forwards on the current task, as knowing that is key to what meta-management actions need to be taken now. Of course the future is unknown. So models stand-in as a means to estimate the most likely future.

The representation provided to this meta-management process includes that provided by the meta-management feedback loop: a high-level summary of the current CP state, and its trajectory so far on the current task. It includes learned dynamic models of CP behaviour. The identification of the current task would presumably be represented within the state of the control process itself. For inline meta-management, that state could be easily accessed directly or somehow directly influence the meta-management processing. Or perhaps the meta-management feedback loop includes a higher-order representation of the current task if it is more suitable for the needs of meta-management processing.

### Meta-learning
The idea of _meta-learning_ captures the ability for an individual to examine their abilities and to make decisions that directly influence their subsequent learning. For example, after observing that their friends have become proficient in use of a skipping-rope after spending a day practising, an individual may set a goal to do the same. Meta-learning is thus about long term skill observation and development.

For meta-learning applied against the control process, the interpretation, encompassing state changes and actions, includes a number of things. Firstly, it requires the construction of a broad understanding of the behaviours and abilities of the control process across many problem domains. This includes strengths and weaknesses. It also includes building models of the comparative behaviours, strengths and weaknesses of comparable individuals. Finally, interpretation includes meta-cognitive decisions that drive further learning, such as through setting goals, acknowledging and remembering certain behaviours that need to be avoided, or likewise for behaviours that should be repeated.

The object is once again the control process itself, but the focus is on a much longer term than in the example in the prior subsection. It now encapsulates a measurement of the relative effectiveness of the control process against the range of all potential problem domains. Like for the other examples, the object has much that the individual is entirely unaware of, including what the optimum set of behaviours really is, and what the future holds. And once again, learned models stand in as approximations of dynamics in order to make predictions about those optimum behaviours.

Contrast this to the object in the case of CP state trajectory meta-management. There the object was the immediate state trajectory. Here, the object is about the collection of learned abilities and how they can be used in different scenarios.

The meta-management process infers what it can about the object through the representations made available via the meta-management feedback loop, and via models. Here the models are built up over time to capture the CP behaviours and abilities on different kinds of problems. Separate models capture the individual's understanding of how other individuals fit against those measures.

### Summary
There are a few key takeaways from the above that help us understand the similarities and differences between standard control and meta-management and the effects on how these respective systems could cooperate and coexist, particularly within an inline architecture.

**Objects differ substantially**. The discussion of objects above identify information that the systems need in order to carry out their purpose, but that they can only guess at. Thus a tremendous amount of processing (and neural mass) is devoted to approximating that knowledge as closely as possible. These are a key focus of the processing systems. That focus differs significantly for the different processes: a) trying to understand and predict the outside world and how the body interacts with it, b) trying to govern the stability of short-term computational behaviour, c) trying to distinguish different problem domains and how changes in learned behaviour could improve future outcomes against those disparate problem domains.

**Overlapping pathways**. The inferred state of the environment, the inferred state of the body, the inferred state of the control process, and predictive models of the dynamics thereof. In one way or another these are all important information that plays an important part of processing and meta-management. This is likely the case in all scenarios where meta-management is required, because at the end of the day meta-management is a process that helps the individual survive in the environment. The raw representations supplied by these pathways is likely re-used for multiple processing levels.

**Significantly differing interpretations from same representations**. If the similarity between likely pathways is impressive, that is matched equally by the difference in outcomes produced by different forms of processing/meta-management.


..todo.. still feels like it's got a bit of course. Need to get back to ultimate purpose of this section...why am I yakking about this?
* Regarding object: in the sample case the object is the external world. But more realistic understanding is that the object is "what could and should be done to afford best results for the individual" (ie: the ground truth). And the representation & interpretation are all about drawing a best guess about that object. (This description is more inline with the Interface Theory of the human brain)

- Takeaways
	- Objects of focus differ
	- Representations used differ substantially. 
	- Overlap in actions, but sub processes differ substantially

## Trains of Thought
[citation, research investigations of how the necessary outcomes of a process lead to certain evolved input representations and representational capacities, thus limiting what can and cannot be captured as input]

.._todo: do I need to be clearer that "pathways" can include both state, direct feedback, and MM feedback?_...

There is another key takeaway from the semiotic analysis above that needs a more thorough discussion. This regards the kinds of thoughts that are possible.

A common turn of phrase is to refer to a "train of thought". For example, when someone suddenly speaks to us after a period of silence we complain that they "broke our train of thought". There are two notions behind that statement. One is that thought progresses. For example when trying to solve a problem, thought progresses from problem to solution through a series of steps. Another notion refers to there being one particular basic grounding idea, or _topic_, being considered which is held onto for the duration of a period of thought. For example, the topic may be the underlying problem that one is attempting to solve. So that while thought shifts from step to step, and between different possible solutions, the topic remains the same for the duration of that sequence of thoughts. When our train of thought is "broken", our attentional focus shifts from that topic to some other, and we loose some of the details held as temporary state in the progression from problem to solution.

For the discussion that follows, I shall define a _train of thought_ as the finite sequence of processing that occurs while a given topic is attended to, with that train of thought ending and another starting when the attended-to topic changes. A _topic_ is to defined intuitionally from the example given above. The definition here is somewhat vague but that is not important for the discussion to follow. More generally, we can say that a thought belongs to the same train of thought as before to the extent that the topic is similar to before.

Now, given a computational system, and given some particular potential topic and associated train of thought, what is required for that train of thought to inhabit the computational system? Or in other words, is it even possible for the given computational system to produce such a train of thought, and what would be required in order to enable that?

![diagram](files/diagram.png)

* _**Semiotic cycle.** todo_

Illustrated in the above figure, we have seen that all thought is the act of interpreting representations, producing more representations requiring interpretation, in an endless cycle. The questions around trains of thought translates to questions around the capacities of those representations and interpretations. By this I mean that a representation only captures a certain amount of information, about a certain thing. Something that is never represented is never available for interpretation. And a representation with a coarse granularity makes less information available to the intepreter than a fine-grained representation. Likewise, an interpreter can only produce interpretations (or rather, interpretational representations) according to its degree of computational complexity (ie: the number of neurons and synapses that make it up) and the learned knowledge available to it.

Furthermore the question of capacities of those representations and interpretations comes down to their purposes. Despite many historical claims of evolution producing features without utility [citations], most have been eventually debunked [citations]. Thus we have a strong reason to believe that evolution would only produce representational and interpretational capacities that meet the needs of the individual. More specifically, evolution would only produce representational and interpretational capacities that increase the individual's likelihood of producing progeny that also go onto to produce more progeny.

So, what kinds of trains of thought can be entertained by a given computational processing system? Those that provide utility according to the given system's function in maximising evolutionary survival.

There are fascinating philosophical discussions that can stem from this idea, like asking what kinds of thought we have never had and will never have simply because our evolved structures are incapable of entertaining them [citation?]. But I am more interested in something a little more concrete.

The first key message I wish to convey is simply the fact that representational and interpretational capacity is not arbitrarily large - it is finite, and tuned according to specific needs. Thus the trains of thought that are possible according to a given system are _constrained_ by that system.

In our semiotic analysis of control and meta-management processes, we identified three examples where interpretational purposes were very different. Thus, viewed on their own, the multi-iteration pathways involving those interpretations very significantly in the potential trains of thought that they may entertain. Even when their capacities are combined in some way, the potential trains of thoughts are still constrained by the purpose-defined capacities of those components.

Secondly, successive iterations of interpretation, representation, and re-interpretation will tend to _attenuate_ the train of thought down to the capacity of some weakest, least complex stage. As we have stated before, representation is almost always an informational bottleneck, so whatever receives that representation has only the informational capacity of the representation plus its own (learned) knowledge. The brain is an extremely complex system, with many sub-processes interacting in complex ways. Any information that is obtained, but not retained through all those interactions, is lost. We can see this effect in the apparent limitation on the number of things that can we can retain within working memory........[citation and details]....

A concrete example of attenuation at play can be directly experienced. It is experienced anytime that we are unable to focus. Imagine this scenario: it's 2pm, you finished your lunch an hour or two ago, and you forgot to have your coffee. You're attempting to complete the work you started earlier in the morning. Something mentally difficult, like doing the accounts for your tax return. You're finding, like many around this time of day [citation], that you're struggling to remain focussed on the task at hand. You start to think about the problem immediately in front of you, you start to form the idea in your mind, and then you realise you can't remember what the next step is. You shift focus to recall the next step, but then can't remember the details of the result you'd just obtained from the prior step. The underlying issue here is one of attention [citations], energy use of digestive processes [citation], and the way our circadian rhythm impacts our cognition [citation], rather than there being anything wrong with our fundamental potential for such thought. However, it illustrates what our experience might be if we had some of the computational and representational capacity for such a task, but that during multi-iteration processing it quickly became too attenuated to be operated against.

The last key message I want to draw out here is that a given thought only exists for the duration that it is repeatedly cycled between representation and interpretation. As we have seen, representations in the brain are fleeting transient sequences of energy spikes travelling along synapses, and interpretations are merely the action of target neurons in receiving those signals and producing new signals. Once those spike trains stop representing a given thought, it ceases to be a thought.

"But what about memory?", I hear you say. Indeed, through mechanisms that we are only beginning to understand, individual neurons do hold temporary state [citation] that modifies their behaviour [citations]. So interpreters could "hold onto" the thought representations that they receive or produce. Likewise, we easily recall past thoughts, indicating that they are somehow recorded within our episodic memory. However, the point I wish to make is that these representations are not "thought" while they are stationary. It is only through re-interpretation that they become thought.

The argument here may seem somewhat tautological to some (thought only exists while thought exists), but the message is more fundamental: that thought only exists as a fleeting interaction between representation and interpretation and that a given thought collapses (ceases to exist as a thought) when that cyclic interaction ends or changes topic. This argument will make more sense when used in the discussion of subjective experience that follows in the next part.

---


# Part V - Solution

The sections before laid out a sequence of logical inferences. Working from a basic need to cope with complexity, we have seen that this concludes with meta-management processes superimposed over the same systems that perform primary control of the body, enabled through a feedback loop that captures a high-level summary of the state of that control process. And we have seen that this results in the control process state having both a "from the inside" representation and a separate "from the outside" representation.

We are now in a position to state the core thesis of this article, which is this:
* Subjective experience is the result of the meta-management feedback loop, an inline meta-management architecture, and the cyclic processing of self-referential state interpreted from that feedback loop.

In more colloquial terms, subjective experience is a _strange loop_ [citation, Hofstadter] produced by the meta-management feedback loop.

This part explores that core thesis in detail. It starts by summarising the processes underlying subjective experience within the human cognitive processes, and then attempts to define subjective experience in more general terms that might be applicable to arbitrary evolved and synthetic agents. A later part examines some possible statements about subjective experience in the wider animal kingdom.
    
# V.1 The Architecture of Subjective Experience
- Setup:
	- Reminder: the core reason-for-being of this paper is to explain the mechanisms of subjective experience in humans. So don't worry about the bigger more general picture yet. Just pull this all together and show how SE occurs in humans.
    
The following illustration pulls together the various processes described in sections above, creating a description of the major _functional_ components involved in the construction of subjective experience within humans. The implication is not that the brain contains specific components and pathways as per this diagram, but that these broad functions and connectivities are present in some way:
    
![architecture of human subjective experience](files/A-coherent-theory-v1-solution-human-architecture.drawio.png)

* _**Functional processes underlying subjective experience in humans**. Habitual, rational, and innate control processes receive sensory input about the state of the body and the environment and produce body actions that effect change against the state of the body and environment. Control processes retain state, enabling multi-iteration processing. The current and recent trajectory of control process state (CP state) is captured and a dimensionality reduced high-level representation is made available as an additional sense to the control processes via the meta-management feedback loop. Environment, body, and cognitive schemas attach additional contextual and meaning information to sensory input, for example providing source labelling to the control processes. Emotions/feelings add an extra level of "importance" to some information. Attentional control mechanisms "choose" which sensory information is attended to._
    
At its core, these functional processes take the externally focussed physical senses (sight, sound, smell, touch, taste) and the internally focussed physical senses (proprioception, balance, etc.), and process them through the action of the innate, habitual and rational control processes, producing appropriate body actions. Schemas for body and environment attach additional contextual and meaning information to the raw senses, including "source labelling" - identifying whether the sense indicates an external or internal source. Emotions/feelings likewise attach additional meaning information to the raw senses. Emotions likely also a have more direct manipulative effect on the control processes, but that is not important for our discussion. Attention affects which information from those sense modalities becomes the focus of the control processes at any given time.

Over the course of multi-iteration processing, the state and recent trajectory of the control processes are captured through some means and a dimensionality reduced representation is constructed. That is made available as an additional sense, a _cognitive sense_, via the meta-management feedback loop. That cognitive sense goes through the same processes for meaning attachment and source labelling as any other sense, including through the development of cognitive schemas.

The cognitive sense likely also encounters the same attentional control as for any other sense. The full extent to which attention attenuates the meta-management feedback loop cannot be clarified at this stage. Anecdotally there is definitely a way in which we can attend less or more to our own mental states, but conversely the arguments of the need for meta-management suggest that the data feed from the feedback loop should always be available. The answers are not important for an understanding of subjective experience. For now we will simply assume that handling of meta-management feedback has the same mixture of "unconscious" and "conscious" processing that we are familiar with for other things - to whatever extent that actually means.

Through the action of multi-iteration processing, this system is capable of entertaining trains of thought. The kinds of trains of thought, the topics that are possible to be thought about, and the duration of any given train of thought are all constrained by the computational capacity and representational qualities of the components of this system.

Memory enables past computational states to be recovered.
        
Before proceeding further, it is important to briefly clarify what the above description is _not_. As a functional description, it makes no claims about the specific neurological pathways or components involved. For example, the meta-management feedback loop may follow a single neurological pathway, forming a single integrated representation, in the style of a _cartesian theatre_ [citation]. Alternatively, it may be the effect of many independent feedback pathways, for example in the style of Dennetian _multiple-drafts_ [citation]. The functional description presented is focused on the most significant processing underlying subject experience and thus omits a lot of other cognitive processes and even omits other connectivities between processes identified. For example, as identified in an earlier section, the emotions can be viewed as a meta-management process themselves and likely directly influence the behaviour of the identified control processes. I have also not attempted to capture in this illustration _how_ the control processes might perform their meta-management functions.

# V.2 Subjective Experience State
I believe that the processes described above are entirely sufficient for the creation of all of our subjective experiences. These processes can be used to explain the specific nature of the content of subjective experience, and of the existence of subjective experience in the first place.

Subjective experience does not "just happen" in some mystical way. It is a specific sequence of computational steps. I hold that, together with circular processing forming a train of thought, subject experience is a specific kind of computational state; a state that represents the presence of subjective experience, ie: a _subjective experience state_ (SES). That computational state doesn't just happen either. It must be constructed. And it takes a few steps to get there.

First, you need a topic. We can have subjective experience of anything that we are capable of representing within our computational system. We can stand at the top of a mountain, staring out wordlessly in awe of the beautiful scene before us, and having no apparent thoughts save for a general sense of wonderment. We can loose ourself in the narration of a good book, with words and pictures, sounds, and even smells flowing through our mind like an excitable babbling river. We can examine our past actions and thoughts, searching for the source of a disagreement with a loved one. We can talk to ourselves "in our head", having lengthy and detailed arguments and disagreements with ourselves. At any time during any of those moments we can catch ourselves and ask the question "do I have subjective experience of this moment?" and we will surely acknowledge in the affirmative. Likewise at any time later we can think back to those moments and claim that we were aware of the event at the time and so had subjective experience of it. And, while having such thoughts about our own thoughts, we can catch ourselves and ask the same question: "do I have subjective experience of this moment?". Any of these suffice for a topic that can become part of the subjective experience state.

Note that I am not considering the truth of statements like "yes, I had subjective experience at the time", merely that most individuals would reach that conclusion. The question of accuracy of such statements will be addressed a little later.

So the first step is that the brain generates a representation of some topic. Let's call it _x_. The topic _x_ does not itself need to have anything to do with subjective experience, and in order to understand the logic here it is best not to think of such an example. I find a good grounding example to be the representational state obtained when I look at an apple on the table and merely notice some particular attribute of the texture of the skin of the apple, with no other specific thought beyond that. So _x_ is, for example, "apple with odd shaped mark, on table".

Skipping a few steps, when subjective experience of a topic occurs, it is because the brain has constructed a subjective experience state about that topic. The SES is a (non-language, non-visual) representation of this:
* "[I] [OBSERVING] [_x_]".

The "I" here captures a few things, constructed from the schema and meaning attachment processes described above:
* It is a statement (in a figurative sense) of location - ie: the place where the observation is occurring is within the bounds of my body.
* It is a statement of identity - ie: the thing doing the observing is me; it is not some other individual.
* It is a statement of source - ie: the observation came from "my" senses.

At this stage, this is not a worded "I" as in the form of worded thoughts. It is more of a raw feeling, a knowing.

The representation of "observing" is important too. It is not just a statement that _x_ "is". Rather:
* It is an acknowledgement that a relationship is present: a relationship between _x_ and something else (in this case "I").
* It is a statement that the relationship is an action that has occurred: the act of observation.

This may sound like some mere play on language, where we take our culturally acquired conceptual baggage and hold it against a word (here the word "observing") in order to grant it more meaning than is appropriate for the context in which it is used. On the contrary, I suspect the existence of the word "observing" is a cultural attempt (a reverse engineering of sorts) at identifying and labelling a phenomenon that existed before the word, and that this phenomenon is the product of our brain structure and the self-referential representation that it produces - the very representation that I am attempting to identify here. [citation: there are theories that language affects how we think, there must also be theories that language is a reverse engineered labelling of phenomenon we observe about ourselves]

In order to construct this SES, the brain needed to invoke at least two key features, likely over a sequence of multiple iterations of processing. Firstly, it invoked a model of the concept of "observing" and identified that such an action was taking place. It is important to note that this model does not need to have any socially constructed language or meaning attached to it. It is merely a model that captures a cause and effect relationship. For example, through a long series of experiments during infancy, we develop a cause and effect model that when we see (observe) something through our visual sense, then that something exists and can be interacted with. If that's not clear enough, consider a hypothetical opposite - where our visual senses are predominated by random hallucinations. The same series of infantile experiments would learn us to ignore the visual sense because there is no cause and effect relationship between the seen objects and anything else. Likewise to the real case of the cause-effect model that we build from our visual sense, we can build a cause-effect model from our cognitive sense. It is to this kind of model that I refer when I state that the brain identifies an act of "observing". All of the extra meaning and connotations that we attach to that concept through or socially acquired knowledge just adds extra nuance and depth to a concept that we already have.

Secondly, the brain used its schemas and source labelling to identify that the action (the "observing") was performed by the individual. The same statements about modelling apply here. The brain does not require any form of spoken language to understand or represent the concept of "I" or that an action was performed by "I". It is a learned model of cause-effect relationships that associates the kinds of subsequent interactions that are possible.

# V.3 Interpretation of Subjective Experience States
With a representation of SES, a few things may happen next. Illustrated in the following diagram.

![SES processing options](files/A-coherent-theory-v1-ses-processing-options.drawio.png)

* _**Options for consequent interpretation of a subjective experience state.** From an example subjective experience state representing "[I] [OBSERVE] [x]". Further thought stemming from the ses. Physical actions that report the existence of the SES. "Storage" to memory, particularly episodic memory. Discarding of the SES without any further processing._

**More thought.** The SES may be further interpreted resulting in additional thought. For example, the wordless representation of "[I] [OBSERVING] [_x_]" may be turned into a verbal language representation "I am observing _x_" in the mind. Such further thought could also entail logical rationalisation about the fact that I am "aware" of what I observe, leading to more general statements about consciousness. Those more general statements could then be further acted upon, such as by constructing SES about them, producing physical action, or remembering them for later.

**Physical action.** The SES may lead to physical action, such as a spoken report or some other physical action (eg: a thumbs up) that acknowledges awareness of observing _x_ [citation, recognition from non-verbal half of split brain patient].

**Memory.** The SES may be merely "saved" to episodic memory before attention switches to something else. Later, that same SES (or some approximation thereof [citation, recall is reconstructed]) may be recalled and further processed. Such further processing could be in the form of more thought or physical action, both of which may be further remembered and recalled.

**Forgotten.** The SES may be simply discarded, with no further processing nor memorisation of its existence.

The outcomes of all of the above entail the content of subjective experience. Most importantly, this includes the specific property of the content that claims "I am experiencing this". So this also explains the existence of subjective experience - that it is processing of a state that claims "I am experiencing this". And why should we such a state and associated processing occur? Because it is necessary for meta-management.

# V.4 The Properties of Subjective Experience
To show more clearly how the above creates subjective experience, let us examine some specific properties of subjective experience. We shall focus on heterophenomena - [define, cite].

## Homonculous
...[details and citation of old ideas of homonculous in brain]...

The existence of an impression of a homonculous has a simple explanation:
* schema, SES constructed from the schema
* MM needs that source identification in order to model appropriate actions

The apparent location of the homonculous within the bounds of our head is curious.
* the brain constructs body schema to identify the specific location of its senses. This provides the important purpose of guiding where actions should be targeted. Many of our physical senses are hosted within our head (sight, sound, smell, taste), and so the schema naturally locates them as such. Although our vision is purposed to gain information about the world outside, our visual sense organs are located within our head. This affects interpretation of the perspective of our vision (things at the centre of our visual field are at about the height of our head, while things at the bottom of our visual field are below our heads), and of actions we need to take if our visual sense organs are in danger of being damaged. These locations encoded within our schema are learned through exploration of cause and effect.
* For the cognitive sense, there are no cause and effect relationships that could be explored under normal circumstances in order to build a schema that locates the cognitive senses within the head. So it is not obvious why the brain chooses the head as the location of the cognitive sense. A possible explanation is that it is an artifact of the fact that most of our senses are located within our head. But I suspect the real answer is not so simple.

## Conscious and Unconscious Thought
* Seem to have some thought that is always unconscious, some that can be selectively accessed (even after the fact), and some where we are actively involved.

* For most of entirely unconscious thought simply has no need to be represented by the meta-management feedback loop. The meta-management feedback loop will be optimised by evolution to contain the minimal set of information needed for effectively meta-management of control processes. Anything else would serve to consume extra neural capacity without further benefit, and would simply be evolved away. Thus, anything that is not represented, is by extension superfluous - for the purpose of meta-management.

* For some processing, the specific steps used to reach an outcome are not important for meta-management. Perhaps for example this is because the processing occurs as the result of habitual processes that do not need higher-order intervention. For most of us, the answer to the maths question "5 + 3" is recalled rather than worked out - the answer simply appears in our thought some time after we consider the question. There is perhaps a lot of activity occurring in the intermission between originally considering the question and the answer appearing. However, if that activity is the result of habitually learned processes, then meta-management likely applies as a training mechanism that only takes effect once a result is produced.

* For more elaborate multi-iteration processing, and in particular where rational control processes are involved, thought appears to proceed in a more slow-paced sequential way with many intermediate states. And it is exactly this kind of thought where I have argued that meta-management is important. Thus those intermediate states are represented via the meta-management feedback loop.

In summary, conscious thought is the collection of processing iterations where aspects of the processing behaviour require meta-management, and the content information of that conscious thought is constrained to the information that is needed for the purpose of meta-management. So called unconscious thought is all other processing that occurs within the brain.

## Subjective experience is "always on"
- example of driving/walking with no memory of it
- Q: are we always SE for the rest of the time?
- What about when we are lost in thought about a hard problem, are we SE at the time, or is it constructed after the fact when we reflect back on it?

Subjective experience states and associated interpretations may occur in a number of different scenarios, and such states may be constructed through a number of different sequences of events. By examining this, we may be able to form some accurate statements about whether subjective experience can be said to be "always on".

Let us start by considering some initial topic _x_ that has no representation of subjective experience. For example the textured apple on a table from above.

From a processor state representing _x_ a number of things may occur next, illustrated in the following diagram.

![x processing options](files/A-coherent-theory-v1-x-processing-options.drawio.png)

* _**Options for consequent interpretation of a representation of x.** Further thought stemming from x. Physical actions that relate to x in some way. "Storage" to memory, particularly episodic memory. Discarding of x before it has been "stored" to memory._

**More thought.** The representation _x_ may immediately be further processed (interpreted) in some way that produces new representations. Perhaps this results in further representations about different aspects of _x_ ("that apple looks tasty"), or a deeper analysis of _x_ in relation to the individual ("I saw that apple yesterday"). Such thought might gradually or rapidly "wander" from _x_ to something else entirely. It might also involve converting the form of the representation or "enacting" it within the mind, for example as verbal language in the mind.

One of the kinds of thought possible here is to combine additional context with the existing representation. So, based on whatever attentional or motivational trigger that may cause it, a thought of _x_ ("there is an apple") may become a thought of "[I] [_x_]" ("there is an apple near me"), and then a thought of "[I] [OBSERVE] [_x_]". This likely occurs via a series of intermediate steps that are hard to quantify without a deeper understanding of the representations actually employed within the brain.

**Physical action.** A representation of _x_ may be further processed (interpreted) as requiring or enabling an external action. For example it may lead to the individual reaching for and taking the thing in question. It may lead to the individual speaking something about _x_: "oh look, an apple".

**Episodic memory.** The representation may be merely "stored" to memory, particularly to episodic memory, and recalled at a later time. When recalling memories we (usually) have some idea of where the memory came from, known as _meta-memory_ [citation]. If we saw an apple, we remember that it was ourselves who saw the apple. If however we were told about an apple by a friend, with that friend going to elaborate details about how it looked and where they found it, creating a detailed visual image within our imagination, we still know that the image we remember was described to us rather than directly observed through our eyes. This is the result of the labelling function. Our recalled representation includes labels attached at the time of original representation.

So, for any recalled _x_, there is a recalled label that identifies the original source of _x_. That is sufficient to construct further representations of many statements about _x_ well after the event where _x_ originally occurred. In particular, it enables construction of representations of new statements about _x_ in relation to "I". For example, "I was told about _x_", "I saw _x_", "I observed _x_".

A subjective experience state about _x_ does not need to be constructed at the time of the original observation of _x_. It is sufficient that _x_ can be recalled, and that it is labelled with "I".

**Forgotten.** Attention may suddenly shift before _x_ has had time to be "stored" into episodic memory, and it is forgotten. For some _x_ that has the potential of leading to a subjective experience state, if it is entirely discarded before being "stored", there may be no evidence available for the absence of the ability to recall that event. So it is entirely possible that there are many moments in our life for which we never have subjective experience. Whether this kind of forgetting without evidence actually occurs in humans, and to what extent it occurs, may not be easy to measure.

- also, computationally no reason why the brain would waste resources constructing a representation unless it is needed, and there would not seem to be a reason to construct an SES unless there is intent to further process it in some way such as in the above.

# V.5 Sufficient Conditions of Subjective Experience
- setup:
	- Describe as part of the process to define the necessary and sufficient conditions.
	- Tononi's IIT outlines _necessary_ conditions.
	- 
	- May work to just have each of the following as sections and to discuss them in terms of variations, sufficiency, necessity, and degree.
    
    
The following outlines _sufficient_ conditions to ensure subjective experience. However, not all may be _necessary_ - to be discussed later.
    
## MM feedback loop
feedback loop that provides summary of CP state and feeds it back in at the level of a sense (ie: with same capacity for applying modelling, and meaning attachment as for any other sense)

## inline mm architecture

## iterative processing
- any form of recurrent state is sufficient here, including associative memory and episodic memory.
- though already required the use of a feedback loop
- there may be a more abstract concept here

## representational and processing capacity
sufficient complexity in processing capability to be able to represent and interpret, to re-represent and to re-interpret

## topic attenuation avoidance

## attention
if has an attention system, must choose to attend.
degree: extend of attention on this topic.

## modelling

## meaning attachment
- emotions/feelings to attach extra meaning
- identity identification

_todo: emotions......This does not do justice to the full extent to which emotions and feelings play a role in cognition. For a full account see Damasio (...)._

## Conditions for evolution of Subject Experience
Conditions necessary for the above to evolve in the first place
	- complexity of environment
	- limit on depth of brain network requiring evolution of iterative processing - ie: reached some point where it is more efficient to evolve iterative processing than to make the brain network deeper.
	- 

# V.6 Necessary and Sufficient Conditions of Subjective Experience

Here's a first attempt at defining the general conditions for subjective experience in any agent. Notice that many of the human-like features are missing here, implying that the quality of subjective experience comes in degrees.

conceptual description:
- any form of representation->interpretation->repeat loop that can observe, represent and process the state of its own process

degrees
- degree: depends on extent to which that source of info is attended to.
- degree: depends on extent of application of knowledge of the _identity_ of that process state, as independent from state external to the process
- degree: depends on breadth/depth of modelling of that information
- degree: depends on length of _topic attenuation avoidance_

example of alternate mechanical descriptions
- independent MM, but it MM's itself (MMM😄)
- only inputs available for cyclic processing is the CP state + MM state -- ie: 100% only cognitive state, no direct access to env/body state. But it would have some idea of env/body state indirectly by what's captured in CP state.
- probably with its own habitual + rational systems.
- seems pretty plausible, but it would be different to human experience:
    - it's like it would have only one core "sense" of external things, like what it "sees" is the standard CP.
    - there would be nothing special about the env/body state that it could infer from that, and in many cases access would be very vague if even there at all.


---


# Part VI - The Intuitional Gap

_todo_


---


# Part VII - Predictions

_todo_


## Convergence of Meta-Management
In developing this theory I have been palpably aware of concerns that what I am proposing makes no sense because such a system could never be stable enough to operate effectively. I have made the claim that habitual and rational system learn off each other. That alone can produce unstable results. Indeed, I have made the claim that they are so unstable that they need a meta-management process in order make them stable. But then I've twisted that assumption on its head by claiming that somehow those very same unstable systems can meta-manage themselves. Without sound empirical results what basis do I have to believe that this could possibly work? And if it's not a feasible architecture, then my entire argument for the basis of subjective experience is in question.

I have attempted to keep this article focused on the theoretical for two reasons. One is that I am not really attempting to prove exactly _how_ the human brain generates subjective experience through material means; but rather merely to prove that it is _plausible_ and _likely_ that material means are sufficient. The detail that I have included hopefully provides a reference point for others to pick up from. The second reason is that I only have so much time in the day. It takes long enough to generate and write about a plausible theory. It takes longer still to do all the empirical research needed to provide data proof behind such a theory. Thus my original intent was not to provide a watertight solution for every question, and I certainly did not intend to prove how such a system could attain stability.

So, perhaps it is more to alleviate my own discomfort than that of anyone else that I shall now offer a few suggestions about how such a system could attain stability.

For this endeavour I shall once again borrow from the AI literature, in particular the concept of _convergence_. ......_todo: introduce the AI concept of "convergence": meaning "stable" + "leading towards the desired outcome"_.

_todo: the description of "narrowing convergent boundaries" and how I've used it aren't quite aligned._

_todo: also describe habitual and rational systems as being part of an adversarial co-training system - the level to which they are co-convergent indicates how accurate or inaccurate they are. This is probably the first thing to mention. And then go into the narrowing convergent boundaries are a more specific concrete description of that._

I suspect that interactions between the habitual system, the rational system, and pressures from the external environment, create an effect of narrowing convergent boundaries. With respect to a single learning system, negative and positive feedback from its surroundings causes it to converge towards an optimum behaviour, but that convergence may be slow. If, at the same time, a second system builds up a model of the surroundings and its feedbacks, and if it applies additional feedback on the first system, then it applies a kind of an additional soft boundary against that first system. More importantly, as that second system gradually improves its model, the boundary that it applies to the first also converges. Thus, the range of behaviours of the first system that are allowed by the second system gradually narrows over time.

Panel A in the diagram below illustrates how the external environment and the rational system may act to apply narrowing convergent boundaries against the learning within the habitual system. Feedback signals received from the environment apply an after-the-fact convergent pressure, in the form of negative and positive rewards and in the form of prediction error. When the rational system is operating near its optimum it provides a before-the-fact convergent pressure, in the form of prevention (usually to avoid a catastrophic error occurring) and in the form of encouraging exploration. For example, the individual may have developed a habit of walking a particular route through the forest to the nearest watering hole, but the rational system will prevent that habituated path because it remembers that a tree had fallen and blocked the path at a location that is currently out of sight.

![Narrowing convergent boundaries](files/A-coherent-theory-v1-mm-convergence.drawio.png)

* _**Narrowing convergent boundaries.**_ ...todo...

When the rational system is not operating near its optimum, the environment and habitual system act to apply a narrowing convergent boundary, illustrated in Panel B. The external environment applies after-the-fact feedback in the form of positive and negative rewards that the rational system can use for future improvement through both rational adaptation and through whatever underlying learning mechanisms it operates on. As actions become more strongly habituated, it becomes harder for the rational system to counteract them, thus applying a before-the-fact prevention against the most catastrophic errors.

The modalities of environmental pressures requires some further discussion. Discussion in a section above already mentioned pure positive and negative rewards such as hunger satiation and pain. It also mentioned learned higher-order feedback mechanisms that layer on top of those innate learning mechanisms.

One further learning layer exists on top. With such advanced and flexible learning and meta-management comes a high degree of freedom. For example, many different modes of behaviour are potentially equally effective. Most negative short-term outcomes can be adapted to, so that the total outcomes is net positive. This can lead to a high degree of instability - if so many modes of behaviour are equality advantageous, there is little learning pressure to maintain a consistent mode of behaviour. In turn, that can lead to constant re-learning within the habitual system. Ultimately, the individual may converge extremely slowly towards its most optimum set of behaviours. It has been suggested...[citations, including Damasio's emotion book].... that society plays an important role here.

Effectively, society is a collective behavioural exploration and learning system that spans a longer time scale than that of an individual. There are many possible systems of societal norms, and the societies that thrive will tend to have produced systems of societal norms that benefit the society and the individuals within it and those systems will tend to remain relatively stable over time. Through constant feedback from adults and peers, a naive individual's higher order processes are trained to produce behaviours that are consistent with the norms of the society in which they live. That societal pressure thus provides a significant portion of the narrowing convergent boundary exerted by the environment on the individual's learning, particularly for its rational systems including meta-management.


![societal convergence pressure](files/A-coherent-theory-v1-societal-convergent-pressure.drawio.png)

* _**Convergence pressures operating against the control systems of an individual.** ..todo.._

## Does it exist?
_todo: better in prediction part_

The subjective experience state is not itself subjective experience. It is merely the content of the experience: a statement that the individual has observed whatever is the topic of the so called subjective experience.

The processing that follows is also not itself subjective experience. It is merely the interpretation of the representation, which has as its output another representation. In the brain, that interpretation occurs through the action of millions of individual neurons. There is no place to pinpoint as the thing that has subjective experience.

There is also no time to pinpoint as the moment of subjective experience. At any given moment in time, the only thing that exists of subjective experience is a representation that subjective experience occurred plus the in-flight action of millions of individual computational units interpreting that representation.

The only evidence we have for the supposed existence of subjective experience is the actions that follow from the above: further thought plus further representations of subjective experience, external actions such as verbal report with regard to our observations, and the subsequently processed memories of the former two.
---


# Part VII - Next Steps

_todo_

# References

* Estimating or Propagating Gradients Through Stochastic Neurons for Conditional Computation
    - https://arxiv.org/abs/1308.3432
    - 2013. Yoshua Bengio, Nicholas Léonard, Aaron Courville.
    
* Borţun, D., & Purcarea, V. L. (2013). Marketing and semiotic approach on communication. Consequences on knowledge of target-audiences. Journal of medicine and life, 6(1), 103–108.

* Burnum J. F. (1993). Medical diagnosis through semiotics. Giving meaning to the sign. Annals of internal medicine, 119(9), 939–943. https://doi.org/10.7326/0003-4819-119-9-199311010-00012

* Nessa J. (1996). About signs and symptoms: can semiotics expand the view of clinical medicine?. Theoretical medicine, 17(4), 363–377. https://doi.org/10.1007/BF00489681

* Peirce (1982-). The Writings of Charles S. Peirce: A Chronological Edition. Volumes 1–6. And 8. Eds. Peirce Edition Project. Bloomington I.N: Indiana University Press.