# Discussion - Fire-and-Forget Style
A lot of processes within the humain brain seem to operate on a "fire-and-forget-and-wait" model:
1. send a one-way request into the abyss
2. wait for the abyss to mysteriously contain information that can be used for a next step

There's some subtle implications here for my architecture:
* memory doesn't return the 'result' directly back to the processor that asked for it; instead, it pushes the result straight into working-memory -- perhaps like a sense.
* the result does not link back to the request (ie: Event.references() doesn't contain a link to the request)
* when the result is a list of possible matches, it shouldn't be contained in some sort of single wrapping MemoryListEvent; instead, each individual item should be pushed into WorkingMemory.
* the requesting processor, must identify useful results within workingmemory itself, without any direct 'result' indication.

This approach seems inefficient and overly loose, but it also fits with another phenomenon:
* We seem to have to "learn" how to drive our brain. There are many behaviours for which which there is no hard-wiring of an ability to know how to work with them, but rather we discover those behaviours over time and learn how to use them.
* Thus, the level of separation between request and response fits that. Over time we learn that a response may 'just appear' if we concentrate on something.

Advantages:
* Flat representation model.
* Feeds into the idea that LTM searches just happen based on whats in WM, continuously in the background, rather than always requiring an explicit request.

Disadvantages:
* Harder to implement the ability to try multiple alternatives
* WM filled up with noise.

# Discussion - Memory as a Sense
'Memory' could be a sense too. For humans, it appears to behave quite differently to other senses; primarily because it doesn't behave as a stream, like the other senses. So we perceive it in a very different way, and attribute very different rationalizations to its makeup.

But, if it could be quite reasonable to consider it a sense like any other, and that it feeds in in just the same way.

That would mean:
* It comes in as an input, not directly back into a processor as a 'response' or directly into working memory.
* Interceptors pick up its data and pre-process them before they are fed into processors and/or directly into working memory, as chosen by the attention-attenuator. Basically, STM and LTM start working almost like processors themselves, with an active component that injects data into the system -- as a 'sense' input.

It operates in response to triggers, which may be explicit requests, or just a strong correlation to something in working memory at the time. -- ie: memories that pop up out of the blue.
