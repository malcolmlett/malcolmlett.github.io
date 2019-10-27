## Problem
The current implementation of Processors iterates over each event within WorkingMemory (in strength order), and emits for the first event it can produce a result for. This is not biologically plausible, because it moves the code over the data.

## Solution
A far more plausible implementation involves two steps:
1. Processor picks single most actionable event within working memory, based on simple heuristics.
2. Processor applies its main processing against that event.
3. Processor emits whatever it can produce from that one event.

Biological design:
* Step (1) would be a neural net that takes all of WM as input, and outputs just the selected event. This seems quite reasonable.

Consequences:
* This design has a drawback in that it cannot iterate over multiple actionable events in WM, as it will potentially always attempt to action the same event. The management of this comes down to "meta-learning": the ability to learn to work _with_ the mind's limitations.

## See Also
This design is in contrast to the [[Processors as Cloud Lambda Functions]] model.