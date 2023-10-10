---
title: Anecdotes for proto AGI
layout: wiki
parent: Wiki
---

This page forms part of the [[Proto AGI v1]] series.

Here I present a few anecdotes that present some particular aspects of mental behaviour.

## Getting more toothpaste
* I go to brush my teeth and I discover my toothpaste has run out.
* A goal bubbles up to my consciousness: get more toothpaste.
* A suggested course of actions further bubbles up: check cupboard.
* Upon finding the cupboard empty, I need to decide how/when to go to the shop to get more toothpaste.
* A thought bubbles up suggesting going for a walk. It's a nice day outside, so it would be nice even though quite far. However, I have to be somewhere soon, and I won't get back in time if I walk.
* Another thought bubbles up suggesting to use the car. I would get there and back in time and not need to rush. But taking the car for just toothpaste seems a waste.
* Another thought bubbles up to use my bicycle. That would not be such a waste, it get me there and back in time, and I would enjoy the nice day outside. So I choose that.

I think the above description in reflective of how the brain works to solve a problem:
1. First a target is produced. In our experience this seems like problem solving, but I think this might be more accurately interpreted as goal selection based on the current state and attention.
2. Next, planning kicks in suggesting a possible trajectory of actions that might reach the selected goal. The plan is analysed for expected reward/cost tradeoffs, and either accepted and actioned, or rejected.
3. When a plan is rejected, it is temporarily eliminated from future possible suggestions, and the planning engine runs again to produce an alternative plan towards the same goal.

## Solving a simple Maths Problem
I set myself a simple maths problem: to find the integer `?` that most closely solved `3 * ? = 27`. I intentionally constrained myself to a trial-and-error style approach.

My thought processes went like this:
1. The number `8` pops into my head.
1. I can't remember what `3 * 8` is, but I know that I'll know `2 * 8` so I first try to remember that: `16` appears.
1. I notice that there's a gap of `4` between `16` and `20`, which uses up half of the remaining `8`. That leaves another `4` to add to `20`, making `24` as the answer.
1. What number was I trying to reach again? `27`. Oh nice, `24` is pretty close to `27`, so `8` was a good guess.
1. Is `24` as close as I'm going to get to `27`? They seem pretty close, but maybe it's worth trying one more. (The idea of calculating the difference between `24` and `27` didn't cross my mind, as I had already primed myself to only consider trial-and-error.)
1. What was I trying to do again? `3 * ? = 27`. Right, I'll try the next number, `9`.
1. `3 * 9`? Don't remember. Ok, `2 * 9`? I remember `18`. Then I remember the trick with adding `9`s: each time I add `9` I simply jump to the next tens place and drop one. So, `18` ... `28` ... `27`. Oh wow, that's the number I'm trying to get.
1. Ok, quick, I must now review how I got here so I can write this down.

Some observations of the above:
* I had no logical reason to start with `8` as my first try. That number just appeared. Presumably it was generated from some heuristic prediction mechanism, as it was clearly very close.
* Assuming that functional areas hold their own working memory, then that same area must hold the original problem `3 * ? = 27`, along with the number being tried, e.g. `8`, while simultaneously working on the problem of how to calculate `3 * 8`. At the peak depth of calculation, that functional area could be holding as much as 5 layers of numbers and expressions: `3 * ? = 27`, `8`, `16`, `16 -> 20 = 4`, `4 remaining from 8`.
* Of all those numbers and expressions in working memory, only one or two are actively attended to at a time. While thinking about `2 * 8` I was no longer consciously aware of the original `3 * ? = 27` problem, or even of the `3 * 8` problem that I was partially solving via `2 * 8`.

Now, if each functional area holds WM that relates to it, we can see above that each functional area still needs to be available for other processing, even while holding onto its WM state. Could it be that each functional area has a little side storage for WM, and that attention mechanisms trigger the functional area to pull out specific values at certain times?

In the [biased competition theory](https://en.wikipedia.org/wiki/Biased_Competition_Theory) of attention (Desimone & Duncan, 1995; Beck & Kastner 2009; Turova and Rolls, 2019), attention is a bi-product of top-down biasing and bottom-up triggers. Additionally, there is some suggestion that competition for attention might be resolved within the targeted functional areas (Lindsay, 2020). I wonder, in the anecdote above, whether the maths functional area was the target of attention, or whether it was the source of the bottom-up claim for attention. In a decentralised system, perhaps any brain region can be the triggering source of activity. In which case, perhaps that functional area took "control" for a little while, continually firing signals into the rest of the brain indicating that there was a maths problem to focus on.

Of course, an open question affecting all this is how this supposed "maths functional area" is truly distributed within the brain, as it is unlikely to be a single focused brain region.
