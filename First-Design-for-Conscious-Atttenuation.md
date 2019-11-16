Problem : how do I incorporate the idea that CF is fundamental to high order thinking in order to attenuate unwanted processor outputs? 

Inspired by noticing how I keep turning on the tap too early while brushing teeth, I think I have an idea. 
1. Subconscious processor emits problematic event. 
2. Another processor notices that thought has veered off and is no longer productive. 
3. It emits a discouragement event. 
4. Further subconscious event emits attenuated by AA. But subconscious processor keeps trying. 
5. Conscious processor has flagged the unwanted event as a bad output. Over time this is used to retrain that subconscious processor. 

So, there's no mechanism for one processor (B) to attenuate another (A) in an inline way. Ie: one processor cannot receive the output of another and preempt it before its output has reached WM. Rather, in the short term, it can only react to what's already gone into WM. 

In the long term, processor A learns to not emit false positives. 

The question remains, how does an event in WM attenuate events emitted from processor A.

This is a interesting kind of thought. It's an example of a very focused meta thought, that has direct control over standard thoughts. Not a passive meta thought, but am active one. It also seems natural that the ability to do this has some architectural basis, with a preconfigured fitness function, but can be learned and improved over time. 

However, for a first cut, it will be sufficient to hard code this into the Attention Attenuator. 
* special AttenuationEvent, with a range of optional filters or can apply : by processor instance, by percept type. 
* strength of AttenuationEvent is subtracted from emitted event strengths to determine their effective strengths. Events are omitted altogether if their effective strength hits zero. Otherwise they compete with others according to their attenuated effective strength. 

Any processor can learn to emit AttenuationEvents.

_(Labels: work-in-progress)_