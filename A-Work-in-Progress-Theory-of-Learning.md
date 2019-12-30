In contrast to my theories on consciousness itself, I have no strong ideas on how learning must operate. I'm merely trying to put something together that would probably work.

The motivation is that I can't really prove general artificial intelligence without learning. Additionally, some of the algorithms /processors in my consciousness architecture are hard to write by hand, so a learning mechanism provides an alternative way of creating them.

However I don't believe consciousness itself requires the ability to learn. We assume them to be intrinsically linked because that's our expectation of it. In biology, that's the only way of acquiring sufficient knowledge and intelligence.

## Intro
Learning is likely the combination of many mechanisms working at different times. I expect there is a combination of online and offline learning for different things. For example, I suspect the Attention Attenuator's trust in each processors' accuracy can be online learned. While the training of individual processors likely requires offline learning because feedback is not always immediately available.

In humans, we suspect sleep is primarily used for offline strengthening of memories, although we know it also plays a part in strengthening skill learning. However, I think we assume that learning takes place during the day too.

In contrast, my architecture will mostly employ offline learning.

## Architected vs Deep Learning
Our brain is not one massive monolithic deep learning neural network. It is a collection of many different components of many different kinds. It combines learning with pre-architected structure.

The architecture is created and refined through evolution. Examples of this include the whole outline of working memory, conscious feedback, senses as streams vs thought acting on discrete events, how short term memory and long term are accessed and queried, and the mechanisms used to initiate and control learning.

Learning is done during life, but only within the bounds of the architecture.

A simple first step to understanding the distinction is that learning needs a "fitness function". The fitness functions are pre-architected through evolution, while the learning happens during life of an individual.

Fitness functions exist for certain things, and not for others. Something I call "hierarchical learning" enables learning of advanced concepts, discussed later. But apart from that, if there is no applicable fitness function, then we cannot learn "it".

## Hierarchical Learning
(todo: copy from other notes)

## Daydream / Nighttime Reprocessing
During these periods, learning mechanism takes control of the mind, and puts it into an offline mode :
* Takes control of Attention Attenuator 
* Directly uses output of processors 
* Applies back-propogation learning to processors. 

The idea is to take the events of the day, as they are available in short term memory. To pick cases where the processors produced less than optimal outputs. And to use that to train the processors.

The inputs and expecteds need to be extracted from the events of the day.

Users hierarchical learning for positive / negative reinforcement of complex ideas.

## Processor Creation
New processors can be created dynamically by the offline learning system.

It will somehow detect the need for a new processor and will attempt to train a new neural network locally. If it succeeds to some minimal level of accuracy, it will turned into a processor and added to the infrastructure.

That minimum level cannot be too high, or it will add too much inertia to forming new learning. In contrast, it will probably err on the side of optimism. Some sort of later mechanism will be needed to prune unuseful / unreliable processors.

New processors will have poor accuracy. They will initially not be trusted, and the "double-checking brain" mechanisms will ensure stable outcomes in the meantime.

## Streamlining
At first we learn lots of individual, fine gained steps. The overall learned process can be quite long, inefficient, and error prone. Eg:
* As I mentally solve some problem that I've been given, the last step should be to respond with the answer. However, at first it won't be that integrated. 
* ... 
* Final step of problem solving arrives at answer (without recognising it as "the answer") 
* Another step recognises this as the final answer to the original question. 
* Final step decides that the answer should be spoken back. 

Over time sequence learning improves the efficiency of moving from one step to the next, but that's still only a part way solution. As we carry out the sequence more, some subsequent steps become built into the prior step. Eg:
* Recognise answer and decide to speak it, in one go. 

## Sequence Learning
Executing a rehearsed set of steps in sequence is more efficient than figuring out what to do at each step. So as we repeatedly do steps in the same order, that strengthens the sequence learning. It is subsequently used to strengthen the appropriate next processor. I suspect it may also be used to "select" the execution of specific processors, but I haven't figured out what that might look like yet.

## Fitness Functions
So, with all of that, what are the fitness functions?

Some may be relatively simple, but a fitness function drives overall exploration and learning about the world is much harder. The simplest solution is to model it as a prediction engine, and the fitness function is its error in predicting. It turns out that this has a strong foundation in research by others, in particular in Karl Friston's "Free Energy Principle". In simple terms, that principle can be described as [1]:
> "Free energy is the difference between the states you expect to be in and the states your sensors tell you that you are in. Or, to put it another way, when you are minimizing free energy, you are minimizing surprise."

## References
1 - The Genius Neuroscientist Who Might Hold the Key to True AI, WIRED, Nov 2018, https://www.wired.com/story/karl-friston-free-energy-principle-artificial-intelligence/.

(Added 2019-12-30. Labels: work-in-progress, theory)