---
title: An Investigation of Active Inference
layout: wiki
parent: Wiki
---

# Some mathematical background

## Expected values
https://en.wikipedia.org/wiki/Expected_value




# Active Inference using Model Predictive Control

This section breaks down the solution proposed by Tschantz _et al_ (2020).

Negative expected free energy of a potential policy is given by the sum over time horizon, via the following equation (the derivation of which is explained by Friston _et al_ (2017)):

    −G(π,τ) ≈ E:q(r|π)[ln p(r)]
            + H[q(o|π)] − E:q(s|π) . H[q(o|s,π)]
            + H[q(s|π)] − E:q(θ) . H[q(s|π,θ)]

where:
* `r` = observed reward at time `τ`
* `o` = state observation at time `τ`
* `s` = true (hidden) state at time `τ`
* `H` = entropy
* `E` = expectation


# Active Inference for Goal Selection

A first naive approach could be to take advantage of the model predictive control implementation by Tschantz _et al_ (2020). That approach executes imagined rollouts (via fixed horizon, Monte Carlo particle propagation) in order to evaluate the "negative expected free energy" of a potential policy. In that solution, ultimately the rollouts are discarded, and only the very next action is emitted by the chosen policy at each time step. However, we could use the imagined rollouts to identify a future state that minimises negative expected free energy - under the assumption that the agent will follow a trajectory with similar benefit to the one taken by the imagined rollout.

The issue there is the assumption about the actual trajectory taken versus the imagined rollout, and the fact that this customisation reduces the Tschantz _et al_ solution to a greedy-selection of goal state. A better solution needs to measure the statistics of potential goals across all potential rollouts.

The best approach would obviously be to start from first principles and work up to a solution that makes more sense.


# References

Tschantz, A., Baltieri, M., Seth, A., & Buckley, C. (2020). Scaling Active Inference. 2020 International Joint Conference on Neural Networks (IJCNN), 1-8.

Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., Pezzulo, G. (2017). Active inference: A process theory. Neural Computation, 29(1):1–49. https://www.mitpressjournals.org/doi/pdf/10.1162/NECO_a_00912