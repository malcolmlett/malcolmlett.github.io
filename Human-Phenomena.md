As much as possible, I'm interested in emulating the design of the human brain, at a high-level architectural level. This page serves to collect together interesting human phenomena. Particularly those that help us make architectural decisions.

Some cases are also indicated with a brief summary of how the implications for design of the emulator.

## Sub-consciousness
For most thinking, I don't actively figure out the conclusion. Rather, I think of a problem, and the answer just appears in my awareness. I believe this works by the subconscious monitoring the state of working memory. When a recognizable question is present, the part of the brain that knows how to answer it, populates the answer back into the WM. This makes biological sense: physical wirings cannot track data around, but must have the data moved into a single accessible place - namely, Working Memory.
* Design conclusion: Processors monitor WM, and bubble up the answer via Attention Attenuator.

## Conscious Feedback
I can observe my thoughts, one at a time, and maybe with sone vague sense of other things being in the background, but largely it's just one thought at a time.

I cannot directly observe my working memory. I can focus attention on something, and then I'm aware of it. My WM seems to influence what I focus on.
* Design conclusion: CF feeds from single top attention (event), not from WM as a whole.

## Short Term and Long Term Memory
I can observe my short term and long term memories, but only after I have thought about it. I cannot just access it willy nilly. It requires a trigger, a specific thought, to start it.
* Design conclusion: Place query into WM. Processor searches STM and LTM and places result into WM.

## Waking-Up
On waking, I have no thoughts. Then my attention fills up with the memory of things that were happening before I fell asleep. Unresolved things come back stronger than resolved things.
* Design conclusion: Processor to reload unresolved events from STM when WM is empty. Works for general forgetfulness and on waking.

## Thought Mechanisms
I recognize "I don't understand" events by the lack of an answer from my subconscious, rather than a direct "don't understand" result. It's as if I learn the typical response time, and if I don't get one within that time then I say "I don't understand". If a result subsequently does arrive, then I say "oh, actually I do know".
* Design conclusion: Conscious awareness used to judge lack of knowledge. Individual processors don't explicitly detect a lack of ability to process. eg: expression parser doesn't emit a 'CannotParse' event.

Some thought is _hard_ - we actively try to avoid doing it. Like when a child learns to read, just looking at a character and remembering what sound it makes requires a lot of effort. Other thought, even if it requires remembering things, is easy. So thinking has a graduated scale of effort. This could make biological sense: more complicated thinking requires more energy expenditure (probably measured in terms of the redirection of oxygenated blood to the appropriate regions of brain), so it would make evolutionary sense to prioritise solving problems using the most efficient mechanisms available that give a good enough trade off between accuracy and effort. As an aside: oxygenated blood supply is how fRMI is used today to [measure brain activity](https://en.wikipedia.org/wiki/Functional_magnetic_resonance_imaging) - thus the theory seems to fit. Curiously, this implies that, for every thought, a prediction is made about what brain regions are required, and about how broadly energy needs to be supplied, in order to encourage/dissuade thought process that is about to begin. And we actually experience that within our conscious awareness, to some extent.
* Design conclusion: well, there's a lot going on here, but it's doable.

## Meta-Thought
We have some _control_ over our attention. For example, meditation is an act especially focused on influencing our attention. This plays into our ability to _monitor_ thought and attention, and to notice the "monkeys in the head". As we develop, we learn to recognise these effects, and we learn strategies for addressing them. Examples:
* I can choose to 'focus' on something
* I can choose to relax my focus and think 'broadly'
* I can immediately react to the thought of a particular strategy and choose to avoid it, for example based on past experience.

The ability to _control_ our attention seems to be something we learn. It his hard to learn. It takes a long time to learn to control it well, and our ability improves slowly over time. It feels much like learning to control a limb - at an early age we 'discover' that we can control the limb, and then we slowly improve the granularity of control. Presumably, for a long time during our initial development, we have no understanding that we can control our thought - or even have much of an awareness of our ability to monitor our thoughts.
* Let's call this "Meta-Learning"

Inhibiting thoughts: I have a learned habit of turning on the tap too early while brushing my teeth. I consciously counteract this my noticing that I have turned it on too soon, turning it off, and then holding onto a thought that counteracts the ongoing desire to turn it back on. In my case, I can actually still feel the ongoing impulse or urge, but it's not via the Conscious Feedback loop - more like a different sense. So it probably doesn't emit any further events into WM. Mind you, in this case, it probably never made it into WM in the first place. Not until I noticed I'd done an action I didn't want to do. 
* Design conclusion: Processors can emit events that are subsequently used to counteract or attenuate events from other processors.

## The Double-checking Brain
Our brain doesn't just produce a result and then act on it. It is continually double checking itself. 

The other day I used the wrong word in a conversation, potentially leading to an embarrassing situation. I knew immediately as the word exited my mouth. But why did I make a mistake in the first place? 

Our brains are not accurate computing engines, but flaky guessing machines. We continually take short cuts, bedstraw its efficient to do so. Our internal brain processors that produce language primarily work automatically. We can analyse each word consciously before speaking it, if we wish. And sometimes we do - you know when someone does that, because they talk slower. But mostly we trust that our subconscious will produce the right result and allow the words to flow straight out our mouths without checking them. 

But that's not the end of the story. We're listening in on ourselves. In a conversation we use that to build a mental model of the other person's state of mind. Or perhaps we just care about speaking in a particular way, and so we listen in and analyse the speech for mistakes. 

When people get brain damage in the region of the brain devoted to understanding spoken language, they lose the ability to understand their own speech. They can still generate language and talk, but cannot double check what they are saying. These people talk in long drawn out sentences with many mistakes.

Every part of our brain is unreliable. So our brain employs an architecture of continually double and triple checking checking itself, at each step of the way, and then listening/watching the final output, and of the resultant consequences. Sometimes a single action has gone through many layers of double checking. Many of those layers of double checking can be enabled/disabled through conscious thought. This explains the smooth transition when learning a new skill, from having to consciously orchestrate every step, to gradually allowing our automated systems to take over as we observe that they are doing a good enough job. 

I suspect these sorts of trust-and-act-then-double-check mechanisms are there throughout the brain, across many layers.

Curiously, this also explains so much of human behavior - it's such a normal human thing to make mistakes and correct ourselves; it's one of those uncanny valley things with robots that don't make mistakes. 