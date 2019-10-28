## Problem
When solving problems, we try out different strategies, and some strategies require us to make multiple attempts with different values, and we need a way of keeping track of all of that. My current solution involves creating some of TriedAttemptsEvent, held in Working Memory (WM), that can be updated with each attempt tried. But I'm not convinced it fits human phenomena.

I wonder if we just keep referring back to Short Term Memory (STM) and don't have any explicit attempt tracking information held in WM.

## Solution - Not Yet
To implement without explicit tracking, requires a reliable STM. My current implementation is not reliable enough - it misses some events out because the current 'active' event doesn't always make it to the top of WM.

For now use I'll use an explicit tracking event. But I need to be prepared to change that later.

I think I'll store that explicit tracking by emitting an event that makes explicit the decision to "attempt to solve" the current stuck thought. This will be emitted in response to a StuckThoughtEvent, and will be the pre-requisite for most of the problem solving strategies kicking in.

## Solution - Parallel Thought
The [[Parallel Thought]] model will not work well with purely-STM based tracking of attempts, as background thought won't get tracked. This could be either a good or bad thing.