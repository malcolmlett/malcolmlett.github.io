As much as possible, I'm interested in emulating the design of the human brain, at a high-level architectural level. This page services to collect together interesting human phenomena. Particularly those that help us make architectural decisions.

## Sub-consciousness
For most thinking, I don't actively figure out the conclusion. Rather, I think of a problem, and the answer just appears in my awareness. I believe this works by the subconscious monitoring the state of working memory. When a recognizable question is present, the part of the brain that knows how to answer it, populates the answer back into the WM. This makes biological sense: physical wirings cannot track data around, but must have the data moved into a single accessible place - namely, Working Memory.
* Design: Processors monitor WM, and bubble up the answer via Attention Attenuator.

## Granularity of Working Memory
I can observe my thoughts, one at a time, and maybe with sone vague sense of other things being in the background, but largely it's just one thought at a time.

I cannot directly observe my working memory. I can focus attention on something, and then I'm aware of it. My WM seems to influence what I focus on.
* Design: CF feeds from single top attention (event), not from WM.

## Short Term Memory and Long Term Memory
I can observe my short term and long term memories, but only after I have thought about it. I cannot just access it willy nilly. It requires a trigger, a specific thought, to start it.
* Design: Place query into WM. Processor searches STM and LTM and places result into WM.

## Waking-Up
On waking, I have no thoughts. Then my attention fills up with the memory of things that were happening before I fell asleep. Unresolved things come back stronger than resolved things.
* Design: Processor to reload unresolved events from STM when WM is empty. Works for general forgetfulness and on waking.

## Thought Mechanisms
I recognize "I don't understand" events by the lack of an answer from my subconscious, rather than a direct "don't understand" result. It's as if I learn the typical response time, and if I don't get one within that time then I say "I don't understand". If a result subsequently does arrive, then I say "oh, actually I do know".
* Design: Conscious awareness used to judge lack of knowledge. Individual processors don't explicitly detect a lack of ability to process. eg: expression parser doesn't emit a 'CannotParse' event.