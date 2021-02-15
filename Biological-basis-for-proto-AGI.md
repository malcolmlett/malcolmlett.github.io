This page summarises some of the known neuroscience, observations, and assumed mechanisms that underly the design in [[Designing a Proto Artificial General Intelligence]].

# Neuroscience
## Senses
(tbd)

* https://en.wikipedia.org/wiki/Body_schema
* https://en.wikipedia.org/wiki/Proprioception

## Motor Control
Significantly, some important motor control actions are performed without brain involvement. For example, in order to maintain balance while standing, the [_stretch reflex_](https://en.wikipedia.org/wiki/Stretch_reflex) automatically contracts any muscle that feels a stretch; without any brain involvement.

![simple sensorimotor pathways](files/sensorimotor-pathways-simple.png)

The most basic form of motor control are [_reflexes_](https://en.wikipedia.org/wiki/Reflex). These are nearly instantaneous involuntary movements in response to some stimuli, and are present at birth. They occur through neural pathways called _reflex arcs_, which act on the stimuli impulse before the impulse even reaches the brain. [_Primitive reflexes_](https://en.wikipedia.org/wiki/Primitive_reflexes) (a.k.a. infantile or newborn reflexes) are a subset that disappear as a neurotypical child develops.

## Sensorimotor Development
* https://en.wikipedia.org/wiki/Developmental_psychology

Piaget's theories on human child intellectual development come from the 1950s and 60s, and are still basically accepted today. They break development into four stages: _sensorimotor_, _pre-operational_, _concrete operational_, and _formal operational_. Sensorimotor development has six substages that build on top of each other (McLeod, 2019):
* **Reflex acts**: within first month of life, the neonate responds to external stimulation with innate reflex actions. For example, it will reflevively suck if a finger is brushed against its mouth or cheek. Piaget theorised that these are essential for bootstrapping sensorimotor learning.
* **Primary circular reactions**: from 1 to 4 months old, the baby will intentionally repeat pleasurable actions centred on its own body. Examples: wiggle its fingers, kick its legs, and suck their thumbs.
* **Secondary circular reactions**: typically from 4 to 8 months old, babies repeat pleasurable actions that involve objects as well as actions involving their own bodies. For example, shaking arattle for the pleasure of hearing the sound that it produces.
* **Co-ordinating Secondary circular reactions**: typically from 8 to 12 months old, babies show signs of an ability to use their acquired knowledge to reach a goal (ie: in contrast to simply prolonging interesting events). For example, it will reach out and knock to one side an object that stands in the way of it getting hold of the rattle.
* **Tertiary circular reactions**: from 12 to 18 months old, similar to secondary circular reactions, but actions are now intentional adaptations to specific situations. The infant who once explored an object by taking it apart now tries to put it back together. For example, it stacks the bricks it took out of its wooden truck back again or it puts back the nesting cups - one inside the other.
* **Symbolic/representational thought**: from 18 to 24 months old, babies learn to form mental representations of objects, enabling them to mentally visualise things that are not physically present. This is crucial to the acquisition of _object permanence_, which Piaget considered to be the most fundamental achievement of the whole sensorimotor stage of development. The symbolic substage is transitional to the pre-operational stage of cognitive development.

A couple of good writeups can be found on the [massey.ac.nz](https://www.massey.ac.nz/~wwpapajl/evolution/assign2/MH/webpage.htm), and [lumenlearning.com](https://courses.lumenlearning.com/suny-lifespandevelopment/chapter/piaget-and-the-sensorimotor-stage/) websites, including descriptions of the other stages.

# Examples
* Wilderbeast calves can [walk within minutes of their birth](https://en.wikipedia.org/wiki/Wildebeest#Breeding_and_reproduction). While many aspects of walking (muscle development, basic muscle control) can be developed while in the womb; there is no way that the complicated act of walking (coordinating motion, maintaining balance) can be learned from experience while in the womb. The systems involved with walking are very complex. Importantly, they cannot be governed by hard-wired basic signals - like for reflexes. They require the use of complex trained neural networks. Surely the only reasonable explanation here is that evolution has encoded the exact neural configuration (including synaptic strengths) into the DNA, for those systems that are required immediately upon birth.

# Building up a theory
## Low level motor control and senses
During fetal development, the mammallian brain does not know about the existence of its limbs, nor about how to interpret the senses it receives. As it does not know about the existence of its limbs, it cannot intentionally attempt to move them and to use the observed error to train itself. It's a classic _chicken-and-egg_ problem problem. So how to bootstrap learning about limb movement (ie: motor control) and sense interpretation?

One observation I made about my own child during their first few months is that their legs and arms flailed around a lot, seemingly without intent. Over time I observed that the flailing seemed to become more intentional. Eventually the flailing was altogether replaced by intentional controlled movement. It turns out that this flailing may have a definite purpose in bootstrapping development (citation needed), as it acts as a form of exploration of the motor control signal space, and simultaneously provides a source of data labelling to correlate with sense inputs.

(diagram: jitter -> motor control -> sense inputs -> train predictions)

In the diagram above, this provides a feedback loop where jitter on the motor control causes visual stimuli that in turn are used to train interpretation of the visual sense. For the fetus in a darkish and blurry womb, the visual stimuli are probably not going to be clear enough to form strong associative connections. But there is another feedback loop, involving the touch sense instead. We do not directly sense our muscle contractions, but the movement of mucles and tendons cause our skin to move, and thus we do observe touch senses as an indirect result of motor control. So that jitter -> motor control -> touch input feedback loop can be used to bootstrap learning in a similar way to sight. Additionally, it likely helps to build up the mental map of our body, forming tightly coupled relationships between muscle control and the touch sensitive areas of the body closest to the muscles.

And finally, after birth, the touch-based bootstrapping gets extended into vision and all the other senses.


## Layering of Motor Control
### Low-level motor control
It's pretty clear from our understanding of neuroscience that the primary motor cortex, in combination with cerebellum, and brain stem perform motor control functions at a low level.

(more tbd)

### Tool use
There's something interesting about the limitations of the above model when you consider it in the context of tool use. A good example is that of driving a car. The car is a tool with relatively simple controls but moderately complex behaviours (eg: the effects of speed and weight on how it corners; the delay in acceleration). In order to control this tool, we use our limbs. While driving, we rarely consciously examine the particular movements that we make to drive the car. Instead, our attention is focused on the environment and how the tool can be used within that environment. When we wish to turn the wheel a certain amount to the left, our ability to control the wheel is agnostic to the particular position of our arms, even though the position of our arms will lead to very different arm movements in order to achieve the same outcome (eg: left hand to pull up or down, depending on where it is at the time). Our mental control is operating at the level of the steering wheel, as if it was a limb.

One way of producing that outcome is through the use of bayesian modelling at the executive control layer. Where we would consciously examine our mental model of a car, including its steering wheel, and use that to decide how to move our arms in order to turn the wheel. But I don't think that's how it works -- the act of turning the steering wheel is too automatic. It's easy to drive a known route on auto-pilot: where we're off in thought about something else, and all we're consciously doing is to keep our eyes open and the automatic systems are doing the rest -- including steering.

Another option is that the human primary motor cortex, in conjunction with the cerebellum, is sufficiently advanced that it can learn these second order instructions with the same network. My hunch is that this isn't the case. For one reason, the architecture of our ML agent shows that the low level motor control network is specifically trained against direct motor control objectives (eg: moving an arm to a particular location), and cannot extend that to higher level abstractions (eg: turning a steering wheel through whatever means is convenient at the time).

What seems like a more realistic explanation is that there is an extra layer of indirection between executive control and the low-level motor control. One which operates at a medium-level representation, and which can plan limb movements based on high-level requirements like the examples above. Conveniently, neuroscience has uncovered just such a layer in the mammalian brain: the secondary motor cortex.

![steering wheel](files/Biological-basis-for-proto-AGI-steering-wheel.png)

### Meta tool use
So let's assume the above is accurate enough. What happens if we attempt to take this one step further? Driving on a road with clear road signs, good conditions, and following a known route is quite a simple goal. What happens if we want to use a tool like that for a more complex goal. For example, driving a digger to shape land. The act of planning how to use the tool (the digger) to achieve a particular result is a third order problem. 

We've shown that low-level motor control (first order control), and tool use (second order control) can both be achieved without the involvement of executive control. Can a third order control requirement be achieved without executive control as well?

I think the answer here is that, to the largest extent, this is not possible. The desire to dig a hole in a particular place in front of you, requires you to intentionally move the digger arm down to the ground, and then scoop it back up again. This leverages the bayesian model of the digger and its behaviours in your conscious thought.

To some extent though, you can learn to do that on auto-pilot. The simple act of digging a hole is as repeatable a process as driving the car to your regular grocery store, and requires you to merely play out a well learned series of actions (on the tool). So there is an extent to which it becomes automatic, but still not entirely automatic. And this seems to fit with the lack of a tertiary motor cortex.

# References
McLeod, S. A. (2019, April 09). Sensorimotor stage. Simply Psychology. https://www.simplypsychology.org/sensorimotor.html
