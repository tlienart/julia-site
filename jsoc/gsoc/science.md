
# Scientific Projects – Summer of Code

## Quantum Computation: Simualation of Noisy Circuits

[Noisy Intermediate-Scale Quantum (NISQ) technology will be available in the near future.](https://arxiv.org/abs/1801.00862) However, it would be much more convenient if we could test our algorithm with noise and simulate our quantum algorithm on noisy circuits to explore their stability, efficiency. To assist the research of NISQ, enhance the quantum circuit simulator in Julia [Yao.jl](https://github.com/QuantumBFS/Yao.jl) with noisy circuit simulation would be quite useful. We are planning to implement the algorithm in a recent paper as our SoC project: [Efficient classical simulation of noisy quantum computation](https://arxiv.org/pdf/1810.03176.pdf).

**Recommended Skills**: Background knowledge in quantum information and tensor networks and the ability of coding with Julia.

**Expected Results**: Provide Yao.jl an extension package that defines different kinds of noise and provide Yao.jl with the ability to simulate certain kind of noisy circuits efficiently.

**Mentors**: [Roger Luo](https://github.com/Roger-luo/)


## Computational methods using zonotopes

Zonotopes are representations of extended use in set-based analysis, since linear transformations and Minkowski sums can be computed efficiently. However, they are are not closed under intersections. In the literature there exist different alternatives for overapproximation of zonotope intersections with other set types. The package [LazySets.jl](https://github.com/JuliaReach/LazySets.jl) already offers support for zonotopes but lacks some of the state-of-the-art methods.

Zonotopes provide a very good middle ground between hyperrectangular approximations and general polyhedral approximations in terms of performance and accuracy. Applications of this project are the verification of hybrid dynamical systems (see [https://juliareach.github.io/JuliaReach-website/](https://juliareach.github.io/JuliaReach-website/)) and in neural network verification (see [AI2](https://ieeexplore.ieee.org/document/8418593) and [NeuralVerification.jl](https://github.com/sisl/NeuralVerification.jl) project).

**Recommended Skills:** Basic knowledge on convex geometry and polyhedral computations is preferred but can be learned along the way. A taste for writing efficient code.

**Expected Results:** Some possibilities are: overapproximation of zonotopes with polytopes, zonotope-polytope intersections, order reduction metods, Minkowski difference of zonotopes.

**Mentors:** [Marcelo Forets](http://github.com/mforets) and [Christian Schilling](https://github.com/schillic).

**References:** See [Reachability.jl#Publications](https://juliareach.github.io/Reachability.jl/stable/publications/) and references therein, or contact us in the [gitter channel](https://gitter.im/JuliaReach/Lobby).
