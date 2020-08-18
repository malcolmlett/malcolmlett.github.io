(WORK IN PROGRESS: This is a re-work that will replace the existing [[A Theory of the Human Mind]] page)

This page presents an engineering investigation of conscious experience, and forms a consistent explanation that is useful enough for it to be emulated today. A likely architecture for the logical components of high-order thought are presented. It is shown that the content of conscious experience is governed by a representational 'model' upon which all high-order thought is based. It is shown how this theory can explain the majority of the phenomena of consciousness, and it is suggested that this architecture will ultimately form the basis for artificial general intelligence. An investigation of the gaps remaining is also covered.

# Introduction
The "Hard Problem of Consciousness" (Chalmers) has been a conundrum for many centuries. In modern times, disciplines as varied as philosophy, neuroscience, physics, and computer science all discuss the topic. 

The theories here have been developed by considering our current understanding of neuroscience, the characteristics of biological and artificial neural networks, and through introspection. While the theory uses the human mind as the primary example, it is focused on the theoretical fundamental architectures of consciousness, irrespective of whether that is in the form of a human biological consciousness, or some other alien mechanical consciousness.

_Unified Theory_ presents a shallow overview of the whole of the theory. _Analysis_ presents a rationale for the theory, and examines some of its consequences......

# Background
(brief lit survey)

# Unified Theory
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
All mammals have a neocortex, and birds have a similar structure called the dorsal ventricular ridge (DVR) that neuroscience suggests provides similar capability to the neocortex [SDOct2012].

Main conclusion:
* Physical computational machines have bulky data processing circuits, and bulky memory storage, and they need a small working area to hold the current set of data being worked on.

## Logical View
The full set of data processing that occurs within our brain is immensely complicated, occurring at many levels with complicated interactions. For example, some behaviours are the result of entirely unconscious brain activity. No one paper could hope to explain all of that, and must focus on a narrow subset of brain functions. This paper is no different. The theory presented here focuses on the mechanisms behind high-order thought, and how they are associated with conscious experience.

The theory claims that the high-level thought system of the human brain is a state machine with a tightly integrated control mechanism, whereas the low-level older part of the brain is something much more akin to our current deep-learning artificial neural network models - basically just pattern matching/prediction engines. High-level thought is achieved through a combination of a relatively simple state machine architecture, with the pattern matching and prediction power of those low-level neural networks.

The proposed high-level state machine of the brain is illustrated in the following diagram. Externally sourced senses (our nominal five senses), plus internal senses (eg: mental tracking of limb position), are received as inputs (likely in a pre-processed form), then used in conjunction with the current state (held in Working Memory) to produce a new state.

![logical view diagram](files/A-theory-of-consciousness-v2-state-machine.png)

In the diagram above, the Logic Processing box represents what is likely the bulk of the brain. While it is likely an oversimplification, it is assumed that the logic processing components are largely stateless, in that they merely compute a result given the inputs. It is further assumed that we can think of the multiple logic components of the brain as a single aggregate.

In the terminology of Danial Kahneman, the logic processing components on their own are of the form of _System 1_ thought (_Fast Thinking_), while the net result of multiple steps being executed by the state machine form _System 2_ thought (_Slow Thinking_).

### Working Memory
Neuroscience currently believes that we hold about 7 items in working memory, for up to about 1 minute.

This is the state data store of our state machine. The presence or absence of certain data items directly influence which logic processes activate or are dormant.

The most simple state machine may be able to operate with only a single data item, and the larger the working memory the more efficient computation can be in theory. In practice, there are trade-offs affecting the size of working memory. If too small, then it is not sufficient to hold all data needed for a particular thought process - more logic processing actions are required for low-level swap-in/swap-out of data from long term storage. If too large, then the data transmission channels between working memory and logic processing become too wide.

The state representation within working memory is likely fairly high-level. It is likely at the level of what we observe within our consciousness.

### Control Mechanism
tbd...

![logic and control loops](files/high-level-data-cycles-v1.png)

## Virtual View
![virtual view diagram](files/A-theory-of-consciousness-v2-model-layer.png)

# Rationale
This section provides an account of why I believe the theory presented here is a good explanation of our experienced phenomena. 

I should first point out that this is a working hypothesis. Some of the premises here may not be universally agreed and need further corroboration. 

If the theory is correct, then there is very little of our internal brain structure that we can observe directly. Thus there should be little that we can deduce about it. However, it turns out the model that I purport we operate on is much like the sort of 'abstraction layer' that is often used in software engineering; and it is well known within the software development field that every abstraction leaks internal details. So in practice we can deduce a lot through observations of the particular computational behaviours and edge cases that we experience, combined with the understanding from modern neuroscience.

## Working memory
Brain neurons exist in physical space and thus are subject to a simple physical law: they cannot be moved around easily. When a regions of neurons have developed a structure and learned firing pattern that produces useful computational capability, that computational capability might be useful for processing of data retrieved from arbitrary sources. Those sources might include long term memory. As memory becomes larger, it becomes inefficient to provide direct access from the computational region to the whole of memory - the data transfer channel could become physically very wide. Furthermore, as the brain evolves greater computational dexterity, it ends up with multiple regions with specialised capabilities. Direct access between those 'processors' and memory would now require multiple wide data transfer channels.

From a physical space perspective, a far more efficient solution is to have a central area where data-to-be-processed is temporarily stored, and for the processing regions to access data in that temporary storage, rather than directly access full memory. Essentially, it is necessary to bring the data to the processor because the processor is large and unmovable.

## High-level thought as a state machine
As we are discovering through the development of artificial neural networks, a simple non-cyclic network of neurons can be very effective for pattern matching and prediction. However it isn't suitable for high-level thought because of a number of limitations:
* it's only capable of producing results from a single pass of the network
* it's hard to combine results from multiple arbitrarily selected processing regions
* it's inflexible across short time scales

High-level thought involves multiple steps and intermediate states. Working memory serves to hold those intermediate state. Multiple steps are supported through operating in cycles, with each cycle taking the current state of working memory, applying one step of computation, and storing the result back into working memory. In other words, a 'state machine'.

It's possible that the evolution of working memory was the catalyst for the evolution of a state-machine processing loop, which further formed the basis of the high-level thinking that we enjoy today.

## Evolutionary reason for awareness of thoughts
### The problem with state machines


### Control mechanism
## Different options.
* Possibility of alien kinds of minds. Eg: two separate cycles. 
* We have phenomenal experience of our senses equally as we experience our own thoughts. Thus, evolution has selected a self controlled processor. 

### Sense labeling: needed in order for control mechanism to know which senses to use. Senses need to be labelled in some way, either through explicit addition of labels, location of source neurons, or some other means.

## Consciousness: natural consequence of visceral loop

 
## Learning
* Why I don't talk about it much. 
* Evolutionary advantage to auto-learning.



# Analysis

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

This remains an open question. And I believe it is an important question. It was a continual attempt to answer that very question that has driven the direction of this theory. However, it's scope is now significantly reduced. In fact, our physical state controls our experiential state so strongly that it is hard to conceive of experience as being anything other than entirely passive. 

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
[SDOct2012] University of Chicago Medical Center. "Homolog of mammalian neocortex found in bird brain." ScienceDaily, 1 October 2012. www.sciencedaily.com/releases/2012/10/121001151953.htm.



