This started as an idea about simplifying the implementation of processors emitting events (see [Issue #14](https://github.com/toaomalkster/conscious-calculator/issues/14)). Ultimately the theme was to make the implementation of processors more like functional programming.

Then I wondered how far this could be taken?

## Problem
Currently each Processor implementation contains an iteration loop over the items within WM. I've been copy-paste pasting the same code everywhere:
```
for (Event memoryItem in workingMemory.all()) {
  if (accepts(memoryItem)) {
     do some stuff

     Event result = generate resultant event
     
     Event update = memoryItem.clone().withTag(HANDLED);
     return new ArrayList<>({result, update});
  }
}
```

## Solution
Could processors be like a modern cloud-focused Lambda Function?

ie: Emulator runs the processor against each entry within WM and the processor executes functional-style code that either emits or doesn't. The AA decides what to do with the emitted event. The processor can still use the rest of WM as context, but it doesn't contain any loops.

Advantages:
* Very practical design, but still probably quite powerful. And could lead to rapid development.

Disadvantages:
* Potentially will cause processors to be more fine-grained, which could require greater use of WM for lower-level partial states.

Rebuttal:
* Seems biologically implausible, to move the "code" to the "data" in this way.

## See Also
* [[Processor-Design:-Only-attempt-single-event]]