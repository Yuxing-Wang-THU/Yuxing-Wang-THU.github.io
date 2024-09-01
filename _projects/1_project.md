---
layout: page
title: ModularEvoGym
description: Co-designing modular soft robots with ModularEvoGym
img: /assets/img/robot.gif
importance: 1
category: work
related_publications: true
---

<div align="center"> <img src='/assets/img/robot.gif' width=500 height=300> </div>

ModularEvoGym [1] is based on Evolution Gym [2], a large-scale benchmark for co-optimizing the design and control of Voxel-based Soft Robots (VSRs). We modified the original state representation to formulate a new modular observation space. The input state of the robot at time step $t$ is represented as $s_{t}^{c}=\lbrace s_{t}^{v},s_{t}^{g}\rbrace$, where $s_{t}^{v}=\lbrace s_{t}^{v_{1}}, s_{t}^{v_{2}},...,s_{t}^{v_N}\rbrace$, $s_{t}^{v_i}$ is composed of each voxel's local information which contains the relative position of its four corners with respect to the center of mass of the robot and its material information (e.g., soft voxel, rigid voxel, horizontal actuator and vertical actuator). $s_{t}^{g}$ is the task-related observation such as terrain information of the environment and goal-relevant information. During the simulation, voxels (except empty voxels) only sense locally, and based on the input sensory information, a controller outputs control signals to vary the volume of actuator voxels. The morphology of the robot is unchangeable during the interaction with the environment.

<div align="center"> <img src='/assets/img/robot.gif' width=500 height=300> </div>

With the support of ModularEvoGym, we can do many interesting things. We modeled the local observations of all voxels as a sequence and adopted the self-attention mechanism [3] to develop a more efficient controller (shown below) that handles incompatible state-action spaces. This controller can be trained by popular Reinforcement Learning algorithms (e.g., PPO [4]) to simultaneously control a variety of robot morphologies.

<div align="center"> <img src='/assets/img/controller.png' width=500 height=300> </div>

For encoding a VSR's morphology, apart from using methods such as direct encoding and Compositional Pattern Producing Network (CPPN) [5], which rely on having access to the whole design space, we provided another choice, Neural Cellular Automata (NCA) [6], which takes multiple actions to grow a robot from an initial seed (morphology), as shown below. NCA encodes complex patterns in a neural network and generates different developmental outcomes while using a smaller set of trainable parameters.

<div align="center"> <img src='/assets/img/design.png' width=500 height=300> </div>

Built upon the aforementioned successes, we also presented an efficient Curriculum-based Co-design (CuCo) method for learning to design and control VSRs through an easy-to-difficult process [7]. The following pictures show a developmental process of a walker agent.

$3 \times 3$ design space, $9$ voxels.
<div align="center"> <img src='/assets/img/1.gif' width=500 height=300> </div>

$5 \times 5$ design space, $25$ voxels.
<div align="center"> <img src='/assets/img/2.gif' width=500 height=300> </div>

$7 \times 7$ design space, $49$ voxels.
<div align="center"> <img src='/assets/img/3.gif' width=500 height=300> </div>

$9 \times 9$ design space, $81$ voxels.
<div align="center"> <img src='/assets/img/4.gif' width=500 height=300> </div>

$11 \times 11$ design space, $121$ voxels.
<div align="center"> <img src='/assets/img/5.gif' width=500 height=300> </div>

**Reference**

[1] [ModularEvoGym](https://github.com/Yuxing-Wang-THU/ModularEvoGym)<br/>
[2] [Evolution Gym: A Large-Scale Benchmark for Evolving Soft Robots](https://evolutiongym.github.io/)<br/>
[3] [Attention Is All You Need](https://arxiv.org/abs/1706.03762)<br/>
[4] [Proximal Policy Optimization Algorithms](https://arxiv.org/abs/1707.06347)<br/>
[5] [Compositional Pattern Producing Network](https://link.springer.com/article/10.1007/s10710-007-9028-8)<br/>
[6] [Neural Cellular Automata](https://distill.pub/2020/growing-ca/)<br/>
[7] [Curriculum-based Co-design of Morphology and Control of Voxel-based Soft Robots](https://openreview.net/forum?id=r9fX833CsuN)
