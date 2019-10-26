## Problem
Currently have a bit of a mess with the representation of events within WM vs STM/LTM, and then with storage and fetching of Percepts.
We have:
* MemoryEvent
* PerceptEvent
* Percept
* Other events

Memory Events wrap any event, which could, for example, be a PerceptEvent.
PerceptEvents always wrap a Percept. It's all getting very nested.

## Solution
* We should probably get rid of MemoryEvent altogether and use tags instead.

Every Event should be labelled with its _source_. But best not to get too literal. So use tags() in a pretty loose way. A NN would just figure out what to do with it.

* Store facts/concepts and events both as first-class items within STM/LTM. For example, don't wrap Percepts in PerceptEvents unnecessarily when storing pre-programmed facts. _Can_ additionally store the Event of when the concept/fact was learned. This event memory may be independently forgotten.

## Aside: Clean up Events
There's some work to do to clean-up how Event objects are created.
* Don't set Event timestamp in processors. Just want the processors to be simple and not worry about 'Emulation Context'.


## Aside: Memory as a Sense
'Memory' could be a sense too. For humans, it appears to behave quite differently to other senses; primarily because it doesn't behave as a stream, like the other senses. So we perceive it in a very different way, and attribute very different rationalizations to its makeup.

But, if it could be quite reasonable to consider it a sense like any other, and that it feeds in in just the same way.

That would mean:
* It comes in as an input, not directly back into a processor as a 'response' or directly into working memory.
* Interceptors pick up its data and pre-process them before they are fed into processors and/or directly into working memory, as chosen by the attention-attenuator. Basically, STM and LTM start working almost like processors themselves, with an active component that injects data into the system -- as a 'sense' input.

It operates in response to triggers, which may be explicit requests, or just a strong correlation to something in working memory at the time. -- ie: memories that pop up out of the blue.
