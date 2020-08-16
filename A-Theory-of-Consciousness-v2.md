(WORK IN PROGRESS: This is a re-work that will replace the existing [[A Theory of the Human Mind]] page)

This page presents an engineering investigation of conscious experience, and forms a consistent explanation that is useful enough for it to be emulated today. A likely architecture for the logical components of high-order thought are presented. It is shown that the content of conscious experience is governed by a representational 'model' upon which all high-order thought is based. It is shown how this theory can explain the majority of the phenomena of consciousness, and it is suggested that this architecture will ultimately form the basis for artificial general intelligence. An investigation of the gaps remaining is also covered.

# Introduction
The "Hard Problem of Consciousness" (Chalmers) has been a conundrum for many centuries. In modern times, disciplines as varied as philosophy, neuroscience, physics, and computer science all discuss the topic. 

The theories here have been developed by considering our current understanding of neuroscience, the characteristics of biological and artificial neural networks, and through introspection. While the theory uses the human mind as the primary example, it is focused on the theoretical fundamental architectures of consciousness, irrespective of whether that is in the form of a human biological consciousness, or some other alien mechanical consciousness.

# Background
(brief lit survey)

# Main
Terminology:
* Online
* Reinforcement
* Offline

## Views
The mechanisms that lead to consciousness are best explained by examining them in the context of different views.

![basic state machine](files/A-theory-of-consciousness-v2-layers.png)

The _biological_ view sees our brain as a collection of neurons of varying types forming a tremendously complicated network. Slowly science is beginning to understand the kind of processing performed by different regions, however our understanding at this level is still very much at its infancy. This article will largely omit discussion about the biological view. However, as we shall see, there is one particularly significant point that needs to be made about the nature of any physical computational machine such as the biological brain.

The _logical_ view attempts to present a simplified architecture of the components of the brain. The majority of discussions presented here are in the context of this view.

The _virtual_ view exists only as the data state that is produced, transferred, and examined by the _logical_ view. However, some important concepts and behaviours are best examined within the framework of the _virtual_ view.

## Biological View
Main conclusion:
* Physical computational machines have bulky data processing circuits, and bulky memory storage, and they need a small working area to hold the current set of data being worked on.

## Logical View
![logical view diagram](files/A-theory-of-consciousness-v2-state-machine.png)
The high-level thought system of the human brain is a state machine with a tightly integrated control mechanism, known as consciousness. The low-level older part of the brain is something much more akin to our current deep-learning artificial neural network models - basically just pattern matching/prediction engines. All thought, including high-level thought, is achieved through coordinating the function of the state machine with the low-level pattern matching/prediction components of the brain.

Ignoring the control-mechanism for the moment, the high-level state machine of the brain is illustrated in the following diagram. The senses are received as inputs, pre-processed, then used in conjunction with the current state (held in Working Memory) to produce multiple potential new states, which are selected by the attention control mechanism.

In the terminology of Danial Kahneman, the pre-processing and logic processing components on their own are of the form of _System 1_ thought (_Fast Thinking_), while the net result of multiple steps being executed by the state machine form _System 2_ thought (_Slow Thinking_).

## Virtual View
![virtual view diagram](files/A-theory-of-consciousness-v2-model-layer.png)

# Analysis
* why conclude all the above

## Explanation of Phenomena - Meta-problem of Consciousness
The remaining two sections of this chapter pick two particular phenomena of conscious experience and show how they are explained by the theory presented here.

Why do we conclude ourselves as conscious? We shall now examine the theory's ability to explain this.

In order for an individual to conclude themselves as conscious, they need to follow a particular logic path. That path is presented here first in the form of an example of a person reflecting on their own thoughts, and then at a more low-level how those thoughts can be produced:

Inner thought example:
1. "I am tired, therefore I want to sit down"
2. "I am aware that I just had the desire to sit down, and I have the strong sense that it was I who decided that"
3. "Because I make decisions, and I am aware of those decisions, then I am conscious".

Logical level example:
1. .
2. .
3. .

The is referred to as a 'Visceral Loop'.

## Explanation of Phenomena - Boundaries of Conscious Experience
The theory presents a possible explanation for why certain things produce phenomenological experience and others not; specifically, that the content of the model defines the content of conscious experience.

todo: offer some rationale for assuming that the scope of conscious experience is defined by what is represented within the model.
...

[WITHIN FIRST OR SECOND PHENOMENA SECTION?] It seems quite clear that there are portions of data processing within our brain that we are conscious of, other data states and processing that we are not aware of. Why, do we experience a particular subset of data processing as consciousness? It turns out that the boundary and content of what we can conclude as consciousness is dictated by what is representable within the model, and what processing can be performed against that model. 

# Why is this useful

* We can build it
* Basis of AGI
* Now that we understand it enough, we can modify it. Eg: learning algorithms don't have to be done exactly the same way. Reinforcement doesn't had to be fine exactly the same way. 

# Gaps in Explanation

* Doesn't explain phenomenal experience 
* Doesn't entirely explain why we don't experience other cyclic regions within in the brain 

This is best characterised as an intuitional gap: theories of consciousness exist that support it being an entirely physical phenomenon, and yet our intuitions about consciousness make it hard for us to accept that a simple physical explanation is sufficient. The leads many to assume a metaphysical explanation is necessary.

I posit that the error here is our intuition. Our intuitions on the subject tend to be contradictory. Even an individual talking about this area will often make statements that seem to contradict each other. Our intuitions are so strong that they make it hard for us to consider the possibilities rationally, and thus may actually be leading us astray.

Curiously, the theory presented here does leave open one important variable within the realm of the physical. It is possible that something physical, within the biology of the brain neurons, is required to turn the model into phenomenological experience. In other words, given two regions of biological neural network (in the same individual or in different individuals), both having equivalent model states and data processing capabilities, could it be that one has a biological structure that turns the model into experience, while the other does not? Our intuition is that there is something special about experience that requires more than just a self-serving data model.

At this stage, I am sympathetic to two possibilities:
1. That there does exist a biological difference between the aforementioned two neural network regions.
2. That there is no difference between the two neural network regions, and thus any system with a model and processing loop that replicates the behaviors of the visceral loop must be conscious.

I don't have any idea how to test which is true. And, furthermore, I fear that our intuition is of little help at this stage.

But, if I am to hazard a guess, I would argue in the case of the former, as per the following very simplistic logic:
* I am opposed to the theory that ordinary matter is conscious (pan-psychism) - ie: my intuition is that this is incorrect.
* Possibility #2 tends to suggest pan-psychism.
* Therefore, #1 is most likely, and we should spend time looking for that difference.

# FAQs

# Curious Effects
* [[The analogy of the Thalamic symbiote]]
* [[Visceral Loop]]
* Free will
* Properties of consciousness
* Meta problem of consciousness 

# Further research 
* Build it - see: [[Conscious Calculator v2]]
* Cause of phenomenological experiences

# References




