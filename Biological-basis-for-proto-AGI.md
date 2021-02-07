This page summarises some of the known neuroscience, observations, and assumed mechanisms that underly the design in [[Designing a Proto Artificial General Intelligence]].

# Building up a theory
## Low level motor control and senses
During fetal development, the mammallian brain does not know about the existence of its limbs, nor about how to interpret the senses it receives. As it does not know about the existence of its limbs, it cannot intentionally attempt to move them and to use the observed error to train itself. It's a classic _chicken-and-egg_ problem problem. So how to bootstrap learning about limb movement (ie: motor control) and sense interpretation?

One observation I made about my own child during their first few months is that their legs and arms flailed around a lot, seemingly without intent. Over time I observed that the flailing seemed to become more intentional. Eventually the flailing was altogether replaced by intentional controlled movement. It turns out that this flailing may have a definite purpose in bootstrapping development (citation needed), as it acts as a form of exploration of the motor control signal space, and simultaneously provides a source of data labelling to correlate with sense inputs.

(diagram: jitter -> motor control -> sense inputs -> train predictions)

In the diagram above, this provides a feedback loop where jitter on the motor control causes visual stimuli that in turn are used to train interpretation of the visual sense. For the fetus in a darkish and blurry womb, the visual stimuli are probably not going to be clear enough to form strong associative connections. But there is another feedback loop, involving the touch sense instead. We do not directly sense our muscle contractions, but the movement of mucles and tendons cause our skin to move, and thus we do observe touch senses as an indirect result of motor control. So that jitter -> motor control -> touch input feedback loop can be used to bootstrap learning in a similar way to sight. Additionally, it likely helps to build up the mental map of our body, forming tightly coupled relationships between muscle control and the touch sensitive areas of the body closest to the muscles.

And finally, after birth, the touch-based bootstrapping gets extended into vision and all the other senses.


# Layering of Motor Control
## Low-level motor control
(tbd)

## Tool use
There's something interesting about the limitations of the above model when you consider it in the context of tool use. A good example is that of driving a car. The car is a tool with relatively simple controls but moderately complex behaviours (eg: the effects of speed and weight on how it corners; the delay in acceleration). In order to control this tool, we use our limbs. While driving, we rarely consciously examine the particular movements that we make to drive the car. Instead, our attention is focused on the environment and how the tool can be used within that environment. When we wish to turn the wheel a certain amount to the left, our ability to control the wheel is agnostic to the particular position of our arms, even though the position of our arms will lead to very different arm movements in order to achieve the same outcome (eg: left hand to pull up or down, depending on where it is at the time). Our mental control is operating at the level of the steering wheel, as if it was a limb.

One way of producing that outcome is through the use of bayesian modelling at the executive control layer. Where we would consciously examine our mental model of a car, including its steering wheel, and use that to decide how to move our arms in order to turn the wheel. But I don't think that's how it works -- the act of turning the steering wheel is too automatic. It's easy to drive a known route on auto-pilot: where we're off in thought about something else, and all we're consciously doing is to keep our eyes open and the automatic systems are doing the rest -- including steering.

Another option is that the human primary motor cortex, in conjunction with the cerebellum, is sufficiently advanced that it can learn these second order instructions with the same network. My hunch is that this isn't the case. For one reason, the architecture of our ML agent shows that the low level motor control network is specifically trained against direct motor control objectives (eg: moving an arm to a particular location), and cannot extend that to higher level abstractions (eg: turning a steering wheel through whatever means is convenient at the time).

What seems like a more realistic explanation is that there is an extra layer of indirection between executive control and the low-level motor control. One which operates at a medium-level representation, and which can plan limb movements based on high-level requirements like the examples above. Conveniently, neuroscience has uncovered just such a layer in the mammalian brain: the secondary motor cortex.

(more tbd, includign diagram)

## Meta tool use
So let's assume the above is accurate enough. What happens if we attempt to take this one step further? Driving on a road with clear road signs, good conditions, and following a known route is quite a simple goal. What happens if we want to use a tool like that for a more complex goal. For example, driving a digger to shape land. The act of planning how to use the tool (the digger) to achieve a particular result is a third order problem. 

We've shown that low-level motor control (first order control), and tool use (second order control) can both be achieved without the involvement of executive control. Can a third order control requirement be achieved without executive control as well?

I think the answer here is that, to the largest extent, this is not possible. The desire to dig a hole in a particular place in front of you, requires you to intentionally move the digger arm down to the ground, and then scoop it back up again. This leverages the bayesian model of the digger and its behaviours in your conscious thought.

To some extent though, you can learn to do that on auto-pilot. The simple act of digging a hole is as repeatable a process as driving the car to your regular grocery store, and requires you to merely play out a well learned series of actions (on the tool). So there is an extent to which it becomes automatic, but still not entirely automatic. And this seems to fit with the lack of a tertiary motor cortex.

(diagrams tbd)