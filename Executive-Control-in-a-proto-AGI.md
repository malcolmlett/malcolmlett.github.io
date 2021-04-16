This page forms part of the [[Proto AGI v1]] series.

I present an examination of executive control for the purpose of building a proto AGI.

# Key features
I now suspect that the following features are key to general intelligence:

* Mental modeling
* Brain as a deconstructed RL algorithm
* Prediction
* Goals
* Learned rewards

tbd: diagram

# Progression of Capabilities

In what is certainly an oversimplication, we will use the following view of evolutionary progression as a way to understand the important differences between three kinds of policy that might be possible at the higher-order control layer.

![evolutionary progression](files/Executive-control-evolutionary-progression.png)

* Simple Hierarchical Policy
    * Here, the high-order policy is of the sort that is currently achievable with Deep Reinforcement Learning and [hierarchical learning](https://thegradient.pub/the-promise-of-hierarchical-reinforcement-learning/). It is trained to naively follow a particular policy that was found through unconscious experimentation to approximately maximise rewards. The policy operates only on immediate sense feedbacks, perhaps using a recurrent neural network (RNN), but without any more advanced system for holding state (eg: working memory), or for understanding the environment at a higher level.
    
* Modelling Adaptive Control
    * At this stage, the system employs persisted high-level modelling of the environment and its behaviours, including other individuals. The model is constantly updated and thus adaptations can be made from only a few or single experience. The policy network is still similar in structure to the simple hierchical policy, however it now integrates with the modelling and working memory systems. This system does not have the conscious feedback loop, and thus cannot model its own internal mental state, nor can it perform any of the more advanced behaviours that depend on that.
    * The inclusion of self-driven goals and rewards is contentious. In biology, this stage would likely incorporate self-driven goals, however to make that work I believe it requires the conscious feedback loop in order to maintain stability. So biological systems would most likely evolve abilities in tandem for self-driven goals/rewards and conscious feedback handling. Thus for our purposes, and in order to maintain a clear distinction between the stages, we'll try to leave self-driven goals and rewards out of the picture for this stage.
    
* Self-aware Executive Control
    * This stage builds on the previous by adding self-driven goals and rewards, and the conscious feedback loop that enables the system to maintain stability.
    
    
With these three stages in mind, we can measure the progression of capability of our proposed solutions.

# Rewards

## Reward Categories
The rewards that a high-functioning general intelligence learns from are complex. In order to attempt to make sense of that, the following diagram categorises the rewards and illustrates how complex those rewards are to learn useful policies from.

![reward categories](files/Executive-control-reward-categories.png)

|Reward Category|Reward Description|Policy Description|
|---|---|---|
|Primitive Rewards|These are rewards that can be supplied to a network through hard-coded mechanisms, using simple raw signals such as from primitive senses. In biology, these would be the earliest to evolve. In a complex environment, a 'teacher' may choose to leverage some of these mechanisms (eg: pain or pleasure). These signals are often sparse, and with low-fidelity (eg: I'm either hungry or I'm not). Examples: pain, hunger, hunger satiation, pleasure, effort, predictive errors.|It is hard for an AI to learn a good policy from such rewards, particularly due to their sparse and low-fidelity nature. However, given that this occurs at the most basic level of agent learning, the policy search space is very large. In many AI settings, resultant limb movements can be jerky. This can be improved by including suitable additional primitive rewards that help to improve the 'quality' (eg: effort can be used to influence the efficiency of ligament movement). Biology has the same problems as AI does with primitive rewards: in complex environments with high dimensionality, it takes a long time to optimise for a good result. Evolution took a long time from single-celled organism to mammals.|
|Sense-interpretation Dependent|This category of reward requires trained neural networks for interpretation of senses. It may even require some level of cognitive ability, but it does not require the level of high-order intelligence required for general intelligence. It includes rewards received by interpreting social feedback, such as from someone critiquing our actions (a 'teacher' in general terms), or from the result of our social interactions with potential friends. It also includes other cognitive interpretation of senses, such as 'surprise' or 'uncertainty' (_a la_ the free energy principle). Examples: teachers saying "good boy" or "no", teacher smiles, teacher frowns, popularity, de-friending, isolation. This form of feedback is often higher-fidelity, but can be frequent or sparse.|Complex networks are required to undestand social cues, based on interpretation of the senses. This form of policy builds on top of the policy learned from primitive rewards, in the sense that the agent likely would never reach the cognitive ability to intepret its senses sufficiently to understand social feedback it it were not for the primitive rewards acting as a bootstrap mechanisms for learning.|
|Achievement|Rewards that depend entirely on the agent's own measure of success. In other words, rewards that the agent gives to itself, based on a reward measure that it has devised itself. These rewards depend on mental models that the agent builds about the world, based on experience and its ability to deduce self-consistent meaning from its experience. Examples: achieving goals, reflecting on one's own character and/or lifestyle, perfectionism.|Determination of these rewards depend on systems that support dynamic mental-modelling of the world, and for determining goals based on those mental-models.|

Each higher-order reward builds upon the policy trained via the lower-order reward. Thus they form a hierarchy. There are approximately two ways in which these categories of reward can interplay:
* Refinement
    * Each higher-order reward provides higher fidelity or a more fine-grained frequency of feedback, making it easier to train the policy to follow the best path.
* Supersedence
    * Each higher-order reward provides (or at least is interpreted to provide) a "better" measure of success, and thus can override the lower-order reward.
    
The refinement hierarchy leads to efficient convergence, and predictable outcomes, however it looses from its inflexibility. The supersedence hierarchy appears more relevant to human learning, as it recognises that a higher-order understanding of the situation enables a more accurate interpretation than is possible from the more primitive layers. Additionally, the higher-order rewards may trade off longer term larger rewards against small short term penalties. For example, an agent may be willing to tolerate a certain amount of pain in order to gain a worthwhile large reward. So the supersedence hierarchy can lead to more adaptable and interesting results, but at the cost of being less likely to converge.

![hierarchical rewards](files/Executive-control-hierarchical-rewards.png)

In practice, we must find some way of combining the two, as they both have considerably important benefits. One approach might be to adjust a weighting between the two over the course of training, with strict preference to refinement hierarchy at first. Another likely variation over the course of training, is to start with only primitive rewards, and to slowly add reward layers over time.

So, a likely training approach is:
1. Primitive rewards only
    * The machinery for other kinds of reward will be in place, so that they can learn, but they won't be allowed to actually influence the final reward value.
    * This phase will carry on for a long time, until the agent has good motor control that produces smooth movements.
    * During this phase, the instructor's "unsaid implicit" goal is the only thing that directs training: avoid getting hurt, use unergy efficiently, eat when hungry, and learn to correlate senses and motion control.
2. Sense-interpretation as refinement
    * A 'teacher' provides visual or tactile cues to train towards some arbitrary goal.
    * Question: how does agent understand that these cues are rewards, and whether they are positive or negative? Does initially associating them with pain/pleasure work? Does it make sense to look at how people train animals? For humans, have evolution just hard-wired recognition of social cues (smiling, etc.) to such an extent that we don't have to teach the association? Or do we do it instinctively from a child's birth and we don't realise it?
    * During this phase, the instructor's "unsaid implicit" goal is again the learning direction, but the agent is interpreting the rewards itself.
3. Achievement as refinement
    * Assumption is that a capability for mental modelling is learned during the first two phases, and that mental models about the world have already been constructed. Thus, now, those mental models and goals derived from them, can be used to measure success.
    * During this phase, the mental models are expected to help the agent more efficiently and accurately achieve the instructor's "unsaid implicit" goal by way of providing high-frequency high-fidelity rewards.
    * Effective reward calculation is heavily weighted towards lower-order rewards if they are available. When they are not available, then higher-order rewards are accepted without change.
4. Achievement as supersedence
    * Finally now we take the reigns off, let the agent explore the world more fully, and really let it develop its own character.
    * The base assumption is that we don't need to change anything about what feedback we're giving. We assume that the internalised reward function from the last phase already conflicts (disagrees) with the lower-order reward functions, but that we were previously constraining the effect of its deviation. So, now we just stop constraining the effect of its deviation, and the policies will adjust.
    * Effective reward is taken as an equally weighted average across the three reward layers, thus a strong high-order reward can counteract a weak primitive penalty.

## Reward components
Some rewards that we might use, as per the categories above:
* Primitive rewards
    * pain
    * satiation
    * learning amount
    * predictive errors (eg: in training sensorimotor network)
* Sense intepreted
    * Uncertainty / curiosity
    
    
_more analysis: tbd_

# Importance of Conscious Feedback

In prior work I've hypothesised that conscious feedback (CF) is important because it acts as a feedback mechanism that the higher-order brain uses against itself to maintain stability. But how exactly does that work?

## Analogue to Physical Senses
Learning of low-level motor control and physical sense interpretation incorporate feedback signals that act as measures of predictive error. In many cases part of the construction of those feedback error signals depend on higher layers. The executive control layer also needs to learn, and it needs error signals to help it with that. But when it's already the highest layer, where does it get its error signals from?

When the executive control layer decides on a physical action, its sense inputs become the feedback signal. They are interpreted and compared to the goal, and the difference becomes the feedback signal that the executive control layer applies to itself for that physical action. Importantly, the feedback signal is fine-grained and immediate. This leads to significantly more efficient learning and smoother actions than possible with sparse rewards.

What about thought? Many thoughts don't lead to physical actions, so the senses cannot be used to provide immediate feedback. Even for the thoughts that do lead to physical actions, the immediate action feedback may not provide much direct feedback about the quality of the thought process that lead to the action. The critiquing of a thought process requires domain knowledge that ony exists within the executive control layer, so it is only that layer that can produce and handle the feedback. Thus, CF provides a means for the executive control layer to critique its own thought processes.

How does it learn to do that critiquing? One way is for it to act as a form of sparse-to-dense reward transformation. Almost all thought leads to physical action of some sort eventually. It may be immediate body action (eg: I want to go somewhere, so I start walking). It may be immediate talking action (eg: I say what I was thinking). It may be delayed physical action. All of those physical actions have the possibility of providing some sparse reward from the environment (eg: I find that I've walked to the wrong place; the person I'm talking to looks confused). All of the executive control layer capabilities (prediction, mental models, memory, etc.) can be employed to learn that certain thought processes tend to be productive, while others tend to lead to negative rewards. So those processes can then provide constant critiquing of the thought process, and provide immediate feedback.

## Inputs vs Outputs
Why would the executive control layer need CF when it's already got access to all the sense inputs and internal state? It because those are all _inputs_ to the neural network of the executive control layer. CF is the only direct way of observing the network's _output_.

## Action Learning
In RL, we learning mappings from actions to probabilities or reward expectations. The actions here are the _output_ of the neural network of the executive control layer. So the RL algorithm needs to directly observe those outputs. Under a hypothesis that the brain implements something akin to RL, but embedded within all its other processes, then it is that same executive control layer that is involved with the RL training. Thus it needs to directly observe those outputs.

# Working Memory

In humans, working memory appears to be a decentralised process. But we don't necessarily need to repeat that for an AI. We could perhaps achieve the same thing with a single 'working memory' (WM) component. One option is the main executive control (EC) system passes some of its output into working memory, and the current state of working memory feeds into EC as an input sense.

![working-memory-variations](files/Executive-control-wm-variations.png)

At this point the question becomes about what state, if any, that WM component holds. Or, is WM just a pass-through?

# Training and Hard-wired Rewards

We want to be careful to offload the executive control layer from having to manage lower level aspects of the system. So we will need to carefully tune which layers receive the RL rewards related to specific things.

![reward-layers](files/Executive-control-reward-layers.png)

## Examples
Learning to balance when walking (intermediate layer reward)
* Old-brain performs this without conscious control.
* Signal from vestibular system provides feedback signal that intermediate and low-level layers use to control balance.
* Same signal from vestibular system can be used as fine-grained reward function.
* But reward shoudln't kick in when lying down, so need a simple automatic mechanism to switch that reward on/off.
* Possible mechanism:
    * Switch on/off based on pressure on soles the feet.

