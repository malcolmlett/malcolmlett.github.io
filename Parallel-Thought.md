## Current Model
1. All processors compete against each other
2. Attention Attenuator looks at the relative strengths of output from all processors, ignoring anything currently in WM.
3. AA picks the output of one processor (can be multiple events)
4. AA loads selected output into WM, slotting them in into order with what's already in WM

## Alternative Model
1. All processors compete against what's currently in WM and against each other
2. Attention Attenuator picks anything that can fit into WM, given the relative strengths of what's already in WM. Probably does this in two steps:
    1. Pick all emitted events, and order them relative to each other.
    2. Apply them to WM relative to existing WM entries
3. Entries in WM get pushed out if they have lower strengths than new events, and WM is full.

CF still only picks top-most event.

Has the interesting effect of allowing parallel thought, with the top-most thought stream being fed back via CF, but everything else being 'background' thought.