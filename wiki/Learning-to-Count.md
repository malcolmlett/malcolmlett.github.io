---
title: Learning to Count
layout: wiki
parent: Wiki
---

Can I teach my AI to count and do arithmetic?

What's the minimum prior knowledge? From gut instinct, let's assume the following is sufficient to learn to count:
* Am understanding of having nothing
* An understanding of having something (ie: 1)
* An understanding of having the same thing twice (ie: 2) 
* An understanding of having lots of something. 

The above would be understood without understanding a specific relationship between them, and without any reference to "number". 

One last thing is needed: Sufficient input signal processing.
*  Let's say :
    * "" as nothing
    * "A" is observed as having a thing
    * "A A" as the same thing twice
    * "A A A" as lots
* And that it can see "+" as a label, with unknown meaning. 

For learning addition, we'll need some more concepts. It turns out that we'll need this for learning to count too:
* Having things being given, when previously not acquired them. 
* Having things being taken away, that were previously acquired. 

Process follows how I've wound teach a child:
* Present "A" and say "1", and make AI repeat "1"
* Present "A A" in such a way that it is interpreted as adding one more A. Say "2" and make AI repeat "2".
    * AI observes 'having a thing provided' and "2"
* Keep repeating, adding and incrementing the number. 
    * Sequence learning learns the sequence of 1, 2, 3,.... 
    * With each item in the sequence being associated with a 'having a thing provided' event. 
* Over time, this should translate into a learned sequence of labels (numbers), with the understanding that to move forward in the sequence requires having additional items added. 

Being able to learn this will be a step towards proving this approach as a solution for artificial general intelligence. But it won't be sufficient in its own. 

The next step is to prove that additional concepts can be built up upon this. If I can demonstrate that, then I have proven that arbitrarily complex concepts can be learned, thorough an inference-style proof (ie: base case, plus 1, to infinity).

Options for next concepts:
* Greater than / smaller than
* Addition
* Anything that relies on being able to refer to numbers as their labels + rules, without having to refer back to their building block concepts. 

The next step before embarking on this is to research what solutions already exist for teaching an AI to count. Whatever solutions and/or discussions out there are sure to give me inspiration.

_(Added 2019-11-19. Labels: work-in-progress)_