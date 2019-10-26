## Problem
Currently have a bit of a mess with the representation of events within WM vs STM/LTM, and then with storage and fetching of Percepts.
We have:
* MemoryEvent
* PerceptEvent
* Percept
* Other events

Memory Events wrap any event, which could, for example, be a PerceptEvent.
PerceptEvents always wrap a Percept. It's all getting very nested.

## Solution - Data Types
* We should probably get rid of MemoryEvent altogether and use tags instead.

Every Event should be labelled with its _source_. But best not to get too literal. So use tags() in a pretty loose way. A NN would just figure out what to do with it.

* Store facts/concepts and events both as first-class items within STM/LTM. For example, don't wrap Percepts in PerceptEvents unnecessarily when storing pre-programmed facts. _Can_ additionally store the Event of when the concept/fact was learned. This event memory may be independently forgotten.

## Solution - 'instanceof'
Also, try to move away from doing 'instance of' on events. Concrete sub-classes should probably only be there to help during event creation, to set required values etc. But they should not be subsequently used to indicate state or type. References and tags should probably be used instead.

## Solution - Clean up Event Creation
There's some work to do to clean-up how Event objects are created.
* Don't set Event timestamp in processors. Just want the processors to be simple and not worry about 'Emulation Context'.
* Processors should set strength according to their own level of confidence -- without having to consider the value relative to global importance.
* AA applies a (potentially learned) weighting factor against each processor.
* When emitting new events, processors should set 'ref' to triggering event, so that AA can use this to adjust strength.
* AA calculates absolute strength of emitted event, something like:
** absolute-strength = proc-emitted-strength * processor-weighting * trigger-event-strength
** (mind you, this particular equation needs some scaling-up, because otherwise it leads to zero over time)

## Solution - Granularity of Representation: Literal/Concrete vs Abstract/Flexible
Don't want to go adding too many meta-attributes to Event data type. For example, don't want to split 'references' up into 'concepts', 'triggers', 'relateds'.

Aim for a simple representational model that is flexible and flat. Think 'Twitter': extremely simple data structure and API, with lots of ways to use it.

So, prefer the use of the relatively meaningless 'references' and 'tags' fields...and even consider merging them. Simple and flat structures, with little type information work better for machine learning anyway.

## Solution - Searching STM/LTM
Memory Search:
* Don't try to pick concept/facts over other types of memory item. Just pick based on similarity. For example, when trying to solve a problem, may not yet any concept entry within LTM that helps, but could have a historical memory of a similar thing, that could prop some ideas.
* If the searcher cares about preference, then the searcher should look after that. Memory should only care about finding 'associated' things.

Search Request:
* Consider whether there should be some sort of optional flag/tag/reference to indicate a preference of concepts vs historical memory, and vise versa.

Result:
1. STM/LTM discovers Percept holding a concept or fact.
2. Emits new PerceptEvent, with 'tags=memory', and holding the percept.