This page presents an examination of executive control for the purpose of building our proto AGI.

# Key features
I now suspect that the following features are key to general intelligence:

* Mental modeling
* Brain as a deconstructed RL algorithm
* Prediction
* Goals
* Learned rewards

tbd: diagram

# Rewards

## Deep Reinforcement Learning Background
One way of slicing the range of RL algorithms available at the moment is to classify them as using one of two approaches:
* Value function estimation
* Policy representation and the policy gradient method.

In value function estimation, the agent attempts to learn a function `V(a(t) | s(t))` that predicts the value (expected sum of rewards) of the path beginning with action `a` at time `t`, given the current state `s(t)` and in implicit fixed goal. The expected value of each action depends on the likely subsequent actions, which are again decided based on the same value function, thus the value of action `a` at time `t`, depends on the expected subsequent actions. Algorithms based on this include the Q-learning algorithm originally proposed by Watkins and Dayan (1992) and the Sarsa algorithm proposed by Rummery and Niranjan (1994). The advantage of this type of algorithm is that the process is simple and easily implementable; however, it does not solve the problem of continuous action space well.

Typical algorithms based on the policy gradient method include the REINFORCE algorithm proposed by Sutton et al. (2000) and the actor-critic algorithm proposed by Konda and Tsitsiklis (2000) are typical algorithms based on policy gradient method. The main idea of these algorithms is to link the parameterization policy with the cumulative reward and continuously optimize the policy to obtain the optimal policy. This type of method can solve the problem of continuous action space, but can easily converge to the local optimal solution (Zhao, Liu, Zhao, and Tang, 2018).

Deep Q Networks (DQN) is one of the simplest algorithms to write in equation form, and while far more advanced techniques are now used, for the purposes of what we need to examine here, the difference is not too important. In particular, currently another popular algorithm Proximal Policy Optimization (PPO) essentially looks the same, but with some extra refinements. Both of these follow the policy gradient method, with an actor-critic used to calculate "advantage" for a given action - which has been found to reduce variance and improve convergence.

The following is a very brief summary of the DQN functions (source: https://www.tensorflow.org/tutorials/reinforcement_learning/actor_critic):

Reward:
```
r(t) = actual reward at time t
```

Expected returns, at time `t`:
```
G(t) = sum(t'=t..T: gamma^(t'-t) * r(t'))
```

Networks:
```
policy(a(t) | s(t)) = policy network, parameterized by theta (network weights)
```

```
V(s(t)) = value network, parameterised by the same theta
```

Actor loss:
```
actor-loss = - sum(t=1..T: log(policy(a(t)|s(t))) * [G(s(t), a(t)) - V(s(t))])
```

Critic loss:
```
critic-loss = huber-loss(G, V)
```

Learning is usually accomplished by recording events into a replay buffer (as tuples of state, action, reward), then running supervised learning against batches retrieves from the replay buffer.


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

# References

Konda, V. R., and Tsitsiklis, J. N. (2000). Actor-critic algorithms. Advances in Neural Information Processing Systems, pp. 1008–1014, MIT Press, Cambridge, MA, USA. [Google Scholar link](https://scholar.google.com/scholar_lookup?title=Actor-critic%20algorithms&author=V.%20R.%20Konda%20&author=J.%20N.%20Tsitsiklis&publication_year=2000)

Rummery, G., and Niranjan, M. (1994). On-line Q learning using connectionist systems. Cambridge University Engineering Department, Cambridge, UK. Technical Report CUDE/F-INFENG/TR 166. [Google Scholar link](https://scholar.google.com/scholar_lookup?title=On-line%20Q%20learning%20using%20connectionist%20systems&author=G.%20Rummery%20&author=M.%20Niranjan&publication_year=1994)

Sutton, R. S., McAllester, D. A., Singh, S. P., et al. (2000). Policy gradient methods for reinforcement learning with function approximation. Advances in Neural Information Processing Systems, pp. 1057–1063, MIT Press, Cambridge, MA, USA. [Google Scholar link](https://scholar.google.com/scholar_lookup?title=Policy%20gradient%20methods%20for%20reinforcement%20learning%20with%20function%20approximation&author=R.%20S.%20Sutton&author=D.%20A.%20McAllester&author=S.%20P.%20Singh%20et%20al.&publication_year=2000)

Watkins, C., and Dayan, P (1991). Q-learning. Machine Learning, vol. 8, no. 3-4, pp. 279–292. https://doi.org/10.1007/bf00992698

Zhao, Y.-N., Liu, P., Zhao, W., and Tang, X.-L. (2018). Twice sampling method in deep Q-network. Acta Automatica Sinica, vol. 45, no. 10, pp. 1870–1882. https://doi.org/10.16383/j.aas.2018.c170635