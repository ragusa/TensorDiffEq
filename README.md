# TensorDiffEq - Efficient and Scalable Multi-GPU PINN Solvers

[![Build Status](https://travis-ci.com/levimcclenny/TensorDiffEq.svg?token=v7YRnTJ5sKUDc2sKNqG5&branch=main)](https://travis-ci.com/levimcclenny/TensorDiffEq)

![TensorDiffEq logo](tdq-banner.png)

Collocation-based PINN solvers on top of Tensorflow for multi-worker distributed computing. 

Use TensorDiffEq if you require:
- A meshless PINN solver that can distribute over multiple workers (GPUs) for
  forward problems (inference) and inverse problems (discovery)
- Scalable domains - Iterated solver construction allows for N-D spatio-temporal support
  - support for N-D spatial domains with no time element is included
- Self-Adaptive Collocation methods for forward and inverse PINNs
- Intuitive user interface allowing for explicit definitions of variable domains, 
  boundary conditions, initial conditions, and strong-form PDEs 

What makes TensorDiffEq different?
- Completely open-source
- [Self-Adaptive Solvers](https://arxiv.org/abs/2009.04544) for forward and inverse problems, leading to increased accuracy of the solution and stability in training, resulting in 
  less overall training time 
- Multi-GPU distributed training for large or fine-grain spatio-temporal domains
- Built on top of Tensorflow 2.0 for increased support in new functionality exclusive to recent TF releases, such as [XLA support](https://www.tensorflow.org/xla), 
[autograph](https://blog.tensorflow.org/2018/07/autograph-converts-python-into-tensorflow-graphs.html) for efficent graph-building, and [grappler support](https://www.tensorflow.org/guide/graph_optimization)
  for graph optimization* - with no chance of the source code being sunset in a further Tensorflow version release
  
- Intuitive interface - defining domains, BCs, ICs, and strong-form PDEs in "plain english"
  



*In development


