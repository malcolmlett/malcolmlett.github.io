# Introduction

Much of the research into consciousness had asked the question "what". And much had been gained from that question. But I think it's time to focus more on the "why". 

Many aspects of the "what" have already been answered. We have vague high level understanding of what kinds of processes assets happening within the brain. We have a good collection of well studied correlates of consciousness, so that we know to some extent which parts of the brain are involved and in what ways. We have strong evidence of the resonant form of brain activity. But much of that leads to high level explanations, without specifics. We can see that dreams seem to be a form of half - consciousness, but we don't understand it. We can see and observe in fMRI when things make it into conscious awareness versus not, but we don't understand the specifics of why some things make it to conscious awareness and others don't. 

The best model we have to date is surprisingly easy to construct out of the various theories. Neural Darwinism, Adaptive Resonance Theory, Global Workspace Theory, Active Inference, and Visceral Loop Theory, and are mutually compatible. Together they produce a unified theory that explains a lot. Eg: IWMT (world models). But even that still fails to provide a strong and detailed explanation of the "why" of conscious awareness. 

The Visceral Loop begins to directly tackle that. But more needs to be done. 

A detailed investigation of the why needs to produce, with mathematical accuracy, a schematic of a self organising, self architecting, self learning, agent. In a multi layered cognitive architecture, each lower layer is trained by the layer above. Boyd what trains the top most layer? Active Inference, in combination with evolutionarily preconfigured loss measures and  attractors are part of this. But to really design such a system requires answering many more nuanced and detailed questions. Answering those, is answering the question of "why". 

It will answer:
- with greater specificity and clarity, why are we conscious at all (phenomenal consciousness)
- why we are conscious of some things and not others (access consciousness)
	- "The big puzzle is, why is the conscious aspect so limited, and the unconscious part so vast? What is the meaning of this odd conjunction?" (Baars, 2022)
- why we have the perception of volitional control (free will)
- why we have conscious subjective experience of dreams. If it is something to do with learning, why is learning so tied to subjective experience?
- Why conscious priming is apparently needed to trigger learning and unconscious problem solving (as mentioned by Baars, 2021). Ie: we just hold something in awareness and we magically learn from it, or magically produce a solution to the question.
- to what level infants are conscious. Eg: probably fully conscious so that the system can learn too. 
- Why Cs is a single stream, not multiple parallel Cs streams. 
- if consciousness is a meta management system, why is it aware of not just the main processes that it is tasked with managing, but of itself as well. Exactly what learning measure or loss function requires that such meta self reference is available? 
- why such a system doesn't need infinite regress on its meta meta-ness.

## How

Having recognised a "why", in the form of a need for better capabilities, the next thing to address is "how". What biologically plausible mechanism may provide the necessary capability? 

So the task at hand is to use the "design stance" to theoretically (or actually) build such a system. It needs to incorporate the Visceral Loop. It needs to be able to operate within a sufficiently complex environment. It needs to be able to learn (long term). It needs to be able to adapt (short term) and presumably it needs to meta-adapt (ie: adapt its meta management).


# Background

See:
* [[Focusing on the why for Animal Kingdom]]

## How to train your Network 

An example for consideration is the difference between a feed forward network, and one that uses predictive coding. Feed forward networks are the predominant type of network in AI today. After decades of research, we now have very efficient and effective learning mechanisms for large scale feed forward networks. This depends on the back propagation algorithm. In AI, it is governed by external control which : records a buffer of past observations, and uses automatic differentiation to propagate the errors.

This approach is generally considered to be not biologically plausible. 

In contrast, we have generally believed that biology uses Hebbian learning : "those that fire together, learn together". But the biological plausibility of that too had proven elusive. 

A different model is that of predictive coding. Here, two feed forward networks play in concert, but in opposite directions. The top-down network predicts the internal layer outputs of the bottom-up network, and the difference is used as an error signal that drives dynamic behaviour and convergence.

It can be shown that predictive coding is mathematically equivalent to empirical bayesian inference within a hierarchical bayesian network. This has excellent convergence characteristics.

Another way of looking at this is that the top-down network calculates the back propagated errors. 

Thus, predictive coding is equivalent to the learning algorithm of a feed forward network. Except that PC is :
- Biologically plausible, and
- Doesn't require an external system to drive the learning, and
- In an ART configuration has better protection against catastrophic forgetting, and, copes better with noise, and
- Isn't vulnerable to simple image tweaks causing it to mistake a very slightly corrupted apple image as a drill. 

Another way of looking at this, is that  predictive coding simultaneously trains a forward recognition model and a backward generative model, and trains them against each other. A feed forward model, in contrast, is only a recognition model, with the environment acting as the generative model  (see below for elaboration of this) and providing error signal with less frequency and lower precision. 

RNN: The purposes of this article, I treat RNNs as a special case of feed forward. Their recurrency is at a micro level. They're really just the temporal equivalent of the spatial convolution network (CNN) - ie: they employ information about the most recent events to adjust their output. But they don't operate at a macro-scale like a state machine. They don't follow an iterative process such as employed by predictive coding. And they don't have a generative model.

This distinction between feed forward and predictive mechanisms will play out in many places throughout what follows. 

## Predictive Coding

We don't really know how to practically build predictive coding yet. VAE are a simplified version, but they don't provide quite they level of dynamic behaviour that we're after. 

Additionally, predictive coding as a theory says nothing about catastrophic forgetting. In contrast, ART specifically addresses catastrophic forgetting. It also potentially supports familiarity based rapid learning /memory. 

ART is basically built upon predictive coding, but with a slightly different focus. 

The best is a combination of the two. 
So it's best to refer to "PD/ART" in place of either, however, for the remainder of notes here, any reference to predictive coding is assumed to refer to "PD/ART".

## Predictive Coding as Bayesian Inference

It is useful here to think of predictive coding as an implementation of Empirical Bayesian Inference running over a model that was optimised via either Expectation Maximisation or Markov Chain Monte Carlo. Note: TensorFlow has some built-in support for these sorts of things: https://www.tensorflow.org/probability/.

In biology and in AI, it is useful to break the problem down into a hierarchical bayesian network.
For example:
- inference of latent state R given raw sense data S.
- p(R|S) = p(S|R) p(R) / p(S)
- => leads to R = max p(S|R) p(R) / p(S), over something.
- But p(R) is actually a complex non-linear distribution, and probably a distribution from a mixture. So we model it as a gaussian mixture model (GMM).
- Thus we have: p(R) = sum p(R|θ) p(θ) over θ.
- And this is what leads to an iterative scheme, successfully improving the estimate of both p(R|S) and p(θ|R).
- see: https://en.wikipedia.org/wiki/Empirical_Bayes_method  (note that I've used θ where they've used η)

Why:
- easier to model p(R) by factorising as a gaussian mixture models (GMM)
- opportunity to train some layers from multiple sources (eg: learning actions from other people via mirror neurons)
- dimensionality reduction


# Stages of Improvement 

This section attempts to list a likely path from simplest to most complex architecture. At each stage, I'm trying to produce a "why" that the stage is an answer to. Or better put, I'm trying to find a "need" that earlier stages cannot fulfil, and that the newer stage does somehow. What variety of cognitive process and agent behaviours is possible with a given stage? When processes and behaviours are not feasible at that stage, or would be simpler if implemented on an architecture with a later stage?

Aa good example of that last point is that our current state of the art deep learning networks are often still feedfoward-only, the simplest of the networks, and one that correlates with the cognitive architecture of plants - but we've scaled up that architecture way beyond the capabilities of plants or the animal kingdom. That's because the animal kingdom found a more efficient architecture (a more advanced one) to achieve the same capabilities. (In this case, efficiency probably expands to "efficiency of learning").

## Feed-forward only network
- May include some micro scale recurrence (ie: recurrent loops of signalling between nearby layers only), but not in a way that it can take from near the final output layer and feed back into near the input layer prior to producing an action.
- Almost all feedforward-only networks have "re-action" (a kind of recurrence) in the form of the sense-infer-act-effect cycle, but there is no macro-scale recurrence at a pre-action level.
- Many of our current state of art deep learning agents, trained through RL, fall into this first Naive category. 
- Recently shown to be very inefficient from learning point of view. 
- Notice also that RL is orchestrated externally using biologically implausible mechanisms. If the RL algorithm was reimplemented via NN as part of the agent, then it would no longer be in this class. 
- All behaviour is reflexive / reactive.
- It's hard to imagine how such an organism can exhibit any adaptation / learning, but it is likely that nature finds a way. 
- Most jelly fish fit into this class. 
- Inferences:
	- sense --> action: error propagation via environment as generative model

## Predictive network for Perception
- ie: adaptive resonance / predictive coding based networks.
- This is a form of macro-scale recurrence, but in a specific form limited to a cyclic swing between perception & prediction that "settles" over time (ie: over multiple cycles). Thus, on its own, it is closer to a feedforward-network than to a network with meta-management.
- Gives more chance for learning and thus behaviour adaptation, including some forms of rapid adaptation, but only in simplistic ways.
- All behaviour still reflexive / reactive.
- Box jellyfish may be here.
- Inferences:
	- sense --> latent state --> action: predictive coding (forward + generative model NN's) for latent state inference, error propagation via environment as generative model for action generation.
	- sense --> current latent state --> desired latent state --> action: full predictive coding
    
Sense --> representation:
- Inference of latent state given raw sense data. 
- p(R|S) = p(S|R) p(R) / p(S) 
- p(S) is learned. 
- p(R) is assumed prior, or given a bias by framing (eg: looking for something, or convinced to expect a certain thing) 
- p(R) is factorised as p(R|θ)p(θ), where θ is basically the selector for the specific model within the GMM of the latent space.
- Uses empirical bayesian inference to alternatively improve estimate in p(R|S) and p(θ|R).

## Predictive Coding for Action
Our entire experience of action is through our senses. We learn the effect of an action command by observing the result. Thus, under an assumption of Active Inference, it makes sense that action is achieved by desiring a particular observation, and letting the action system infer the correct commands. Further, the request itself is not constructed in terms of raw sense observations. Rather, it is constructed in terms of latent state - the same latent state that is inferred from predictive coding for perception. Thus, an action request is encoded as a latent state representation, which implies some strong (high confidence) requirements about certain areas of sense space, and doesn't care about others. eg: I want my hand to move to the cup, but I don't care about what's happening in the background or what my feet are doing.

The desired state itself must be inferred somehow based on current state and goal. Additionally, it might represent a state, or perhaps also encode a trajectory through latent space. I'll ignore those details for now. Thus we have:

Desired state ---> motor action:
- Inference of action, given latent state (representation) 
- p(A|R) = p(R|A) p(A) / p(R) 
- Uses empirical bayesian inference, factorising p(A) as p(A|θA)p(θA), where θA is basically the selector for the specific action model within the GMM of the latent space.
- Thus estimates A via iterative successive improvements of p(A|R) and p(θA|A).

### Predictive Coding for Desired State Inference
Current state + goal ---> desired state:
- Goal may be explicit and dynamic or implicit and static.
- I'm not sure about this inference. Maybe it's predictive coding too, maybe it's not.
- It's even possible that predictive coding evolved as: sense --> current latent state  + desired latent state --> action first, with current --> desired using simple gradient descent.
- ie: it's gradient descent with environment as the generative model, but operating at a higher-order representation. This still seems like an evolutionary advantage.

### Predictive Coding for Desired State Trajectory
Another possibility alluded to by (1), is that the desired state is represented as a trajectory.
Thus, we have:
- desired state trajectory  ---> an action is inferred
- efferent copy sent to perception processors
- perception processors predict trajectory given efferent copy
- predicted trajectory compared to desired trajectory, resulting in error
- subsequent adjustment to action inference, and repeat.

All of that probably occurs within the latent state space, as a much easier model to work with than raw sense space.

Reference 1: Predictive coding: an account of the mirror neuron system. James M. Kilner, Karl J. Friston, and Chris D. Frith. (see note: Predictive Coding).

### Predictive Coding for Direct Perception -> Action Inference
Presumably biology initially evolved a direct inference from raw percept to raw action, and only slowly added the different steps:
1. sense --> action
2. sense --> latent state --> action
3. sense --> current latent state --> desired latent state --> action

Without the hierarchical bayes, the modelling must employ approximations, so the first two stages presumably can be mathematically understood in that way.

Without the translation going on between current and desired latent state, there is less option for developing a consistent state space that can learn from multiple sources. Thus it presumably devolves into simple gradient descent. At that point, the environment is used for the generative model: actions are immediately executed, and error detections used to drive the direction of gradient descent. Thus, a neural net can indeed be used in stages 1 and 2, but they do not reflect true predictive coding.

## Attention
Inspiration 
- From Baars, 2022: " The idea that consciousness is a gateway — something that creates access to a vast unconscious mind — has interesting implications for understanding learning. It suggests that learning just requires us to point our consciousness at some material we want to learn,"
- This suggests an interpretation that attention is a "movable" thing, like a physical limb, and it needs similar control processes and learning. Likewise, it may be guided through Active Inference. 

If attention is a a form of action, then it must be trained through experience. This includes exploration to learn new capabilities and new things to avoid. It includes exploitation in order to achieve goals and avoid negative outcomes. 

Active Inference is a unified way of managing the often mutually exclusive needs of exploration and exploitation by measuring free energy as the amount of uncertainty (unknown) around some particular action, and the expected costs of re-performing past actions that had negative outcomes. It can also be extended to incorporate goals when they are present. 

A significant point of attention, brought out within Part II of Baars, 2022, is that while attention is key to consciousness and executive control, it is not under conscious control. We can (sometimes) influence our attention, but we lack direct control. In fact, specific damage can result in disorderly attention without a reduction in the apparent breadth or detail of subjective experience. 

Thus, it would seem that this Active Inference system operates independently. It obtains knowledge of the system-wide goal somehow (perhaps by inspecting WM like any other system), and presumably uses as inputs all of the conscious and unconscious data in working memory, plus the current external and endogenous sensory inputs.

Thus, consciousness can influence attention through selection of goal, but otherwise is subservient to attention. 

Even though attention selection may at times act counter to conscious goals, over time it will learn from negative outcomes. In fact those negative outcomes will also teach it to ignore goals at times when other more pressing concerns occur. 

*Why* is attention necessary? Why not feed all sensory data into the meson cognitive process and let it do filtering, unification, and processing in the same step? A: bandwidth, and training efficiency. 

Processing inputs include 5 external senses, proprioceptive, vestibular, gustative, endogenous (imagined), WM state, memory recall. That's a lot to process and works require a larger bandwidth if it's all passed verbatim into primary cognition network. So attention reduces bandwidth, reducing physical wiring requirements, reducing energy requirements, and reducing processing complexity. 

Additionally, as Friston showed, greater filtering and layering leads to less dimensionality of learning search. So it's more efficient to do with less. Thus, the task of attention is to filter out less important information so that main processing only has to deal with the most important stuff. 

Perhaps attention also had the goal of taking those disparate data sources and translating to a single unified representation. Because there's only one cognitive pipeline. But it doesn't explain why there's only one pipeline. 

## Multi-modality sensory, effector, and internal state integration
- Predictive-coding to integrate multiple sensory modalities.
- Predictive-coding to 
- Predictive-coding + afference copy to identify the difference between self-caused sensory change versus external environmental changes.
- Improved coordination for more complex environments / behaviours - but still all behaviour is reflexive / reactive.
- Some room for variations between decentralised and centralised processing models. However, this suggests a start towards a centralised control model.
- ie: this is the first part of the answer to why: centralised control?.
- Why: resolve some ambiguities (but not ones requiring reconsideration over multiple loop cycles). 
- Why: aggregate is more than sum of parts: eg: identify features as relationships between features in modalities. 
- Flies may be here.

### Sensory Integration Details
Motivating question: what is the difference between our raw sense perception (that we may not have subjective experience of), and the integrated summary that we are aware of within our subjective experience?

One possible answer may lie in a seemingly unrelated observation: that all our senses are fictitious:
- We see in colours. And yet in physics, they don't exist. At a stretch you could say that the primary colours exist, but the non-primary colours (especially white), totally do not exist. In physics, there is only distributions of superimposed electromagnetic radiation at different frequencies. Our perception of colour is a completely artificial representation, constructed from sampling certain points along the frequency range.
- Sounds are very similar. All that occurs in physics is air particles being shoved around by a motely mix of waves emanating from different sources with different frequencies. We accurately infer the source of those sounds. But what we actually hear doesn't necessarily bare any resemblance to what you could arguably call the real physical sound. Correlation, yes. But resemblance, no.
- Touch. There are so many different kinds of touch and touch-like sensations. Some use similar kinds of cells for touch perception, while others use differing kinds of cells.  And we experience them in different ways. It's hard to say what the "real" touch is, and how similar or different our perception is.
- Taste and smell. These are just like colours. Taste and smell do not exist in a physical sense. Mixtures of different compounds are in the food/water we consume, and in the air we breath, and chemical reactions occur that trigger a mixture of different nerve impulses, and we represent all that through what we experience as taste and smell. There's every reason to believe that the representations that we subjectively experience are entirely hallucinatory.

Importantly, in our subjective experience, each sense has its own unique characteristics. They feel different. This suggests that the subjectively experienced representations are constructed in different regions of the brain, with each region devoted to that particular kind of sense->processing->representation system.

Global workspace theory hypothesises that the content of the global workspace defines the content of our subjective experience. Since we experience the sense representations discussed above, it seems likely that they are the contents of the global workspace. And since we've also claimed that they are managed by different brain regions, finally we can conclude that it is likely that the global workspace is not a unified central representation, but rather a collaboration of multiple distributed representations.

And the apparent central integrated one-representation-to-rule-them-all that we have at the centre of subjective experience? Perhaps that is another illusion. In the same way that we perceive a vast solid image in front of us, but our eye takes in only a narrow field of view at a time, and the perceived image is combined together from multiple takes - perhaps our perception of a single unified representation is a the result of trickery.
...mind you, the vision example implies a mechanism that specifically holds and builds up the whole image. So the same would be needed for the central subjective representation.

From a bayesian inference point of view, it makes sense that there is indeed a central subjective representation. In the bayesian inference phrasing, the goal is to infer the latent state of the environment using all available information (ie: all sense modalities). And that single consistent latent state is then a better source of information for choosing action etc. In particular, inference of latent state that uses all sensory modalities is better than inference using only one.

### Conclusion
(note: duplicate of Sensory Integration as Global Workspace section below) 
Why:
- Action control is more effective if based on inference of latent state, rather than merely driving based on raw perception.
- This is because there is not a 1:1 mapping between raw perception and latent state. Inference requires use of past observation and knowledge to "fill in the gaps" and resolve ambiguities.
- It provides a dimensionality reduction for more efficient learning. 
- It also creates a lingua franca for inter-process communication. 
What:
- Single unified inference of latent state. 
- Attenuated by attention.
- Further processing all based on that single unified representation. 

## Context-free attention (aka naive attention, aka passive attention)
- Why: Minimises bandwidth requirements and learning complexity within higher-level control mechanisms in a more complex organism. 
- Sensory integration through a lossy bandwidth bottleneck (ie: doesn't attempt to produce full predictive generation of all input sense data)
- Learns to filter based on utility to higher-level control.
- The sensory integration step above probably includes this by default, but not necessary, so this is listed as a separate step.
- see section "Sensory Integration as Attention" below.

## Attention
- Why: Minimises bandwidth requirements and learning complexity within higher-level control mechanisms in a more complex organism.
- Why: Incorporates "goal" feedback from higher-level control processes to dynamically control the filtering, in order to improve the utility of the filtered data (relative to naive attention).
- Implies a form of centralised control in this sense:
	- that there is only one (ie: "central") aggregate interpretation of the current external + internal state
- ie: this is the second part of the answer to why: centralised control?.
- Still doesn't necessarily have meta control. 

## Multi-cycle processing recurrent network
- Can include multiple processing cycles "pre-action" - ie: before choosing to act on the inference. eg: consideration of multiple options before choosing best one.
- However, this level of processing likely requires many of the remaining evolutionary steps. So the exact position and nature of this stage needs some refining.
- eg: not obvious whether this can exist without meta-management, or whether meta-management could exist without multi-cycle processing.
- Why: resolve complex ambiguities that require reconsideration over multiple loop cycles. 

## Central executive control
- Why: handle novel situations. Eg: through deliberative selection of success measures (most habitual action embeds a fixed success measure). 
- Why: final say in unresolved competition. 
- Why: error handling (esp. as triggered by habituated error detection: Eg when missed a step in a normally habituated sequence and have a "feeling" of something being wrong but not conscious of it yet), and error detection in novel situations.

## Meta-management
- Why: self governance of learning. Eg: identification of learning opportunities. Hindsight identification/improvement of success measures. 

## Rational thought 
- Ability to perform some form of rational thought, at a higher level than brute slowly learned bayesian inference. Or perhaps this is bayesian inference at the high level. It's somehow different to brute pattern matching that NN do. 
- Not implying logical soundness. 
- Eg: ability to consider a mixture of pro- and anti- relationships in order to conclude something. 
- Eg: primal logic ability. 
- Eg: perhaps related to numbers. 
- We are lacking a fundamental theory of this kind of thought so it's hard to define accurately.
- Why: at some point the env interactions and agent behaviours need to be more advanced than simplistic pattern matching. 
- Is it something like a loop with  representation of problem + potential relation as input (recalled via associative memory) plus matching and generative abilities based on the relations. Then, by looping and generating/recalling subsequent relations it can proceed rationally. 
- Understanding this will likely put further dependency and constraints on sensory/representational integration (global workspace) and meta management. For example, is it only possible with memory? 

## Later stage - memory 
- How does a recalled memory cause a network to behave differently? Eg: how does recalled relation cause a generative process to produce a different result, or a matching process a different result? The process is a learned one that trains neural weights. Does the memory change the weights in a very dynamic system, something akin to fast single shot familiarity learning? Or, does the memory act as an input in a standardised representation? 
- For the latter, this would likely suggest that global workspace contents, particularly from memory recall, is held in a decentralised fashion, with parts stored in each brain Region devoted to that part of the data. This raises questions for what the central integrated experience is. 
- How does the central integrated representation get back out to the appropriate regions? Each region could do its own integration, but that could lead to ambiguous competing results. And it seems the role of central integration is to resolve ambiguities. 
- It suggests that perhaps central integration is : 1) only necessary for input to meta management. 2) still necessary for combining multiple senses, but then reprocessed and distributed back out to individual regions again.


# Unclassified 

Some other improvements with inobvious location.

## Uncertainty 
- At some point around about here, representation of uncertainty is needed. For example in controlling the level of over training induced from errors in predictive coding feedbacks. And in the optimal inferences drawn from varyingly accurate senses - eg: whether it's safe to strike on something when you aren't certain of its size. Or to flee when you aren't certain of the threat (there's a cost of unnecessary fleeing). 

## Later stage - Emotions
tbd