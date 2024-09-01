---
title: "Dynamics-Adaptive Continual Reinforcement Learning via Progressive Contextualization"
collection: publications
permalink: /publication/2023-05-01-paper-title-number-1
excerpt: "Continual Reinforcement Learning (CRL) via Progressive Contextualization. <br/><img src='/images/daco.jpg' width=300>"
date: 2023-05-01
venue: 'IEEE Transactions on Neural Networks and Learning Systems'
citation: 'Tiantian Zhang, Zichuan Lin, Yuxing Wang, Deheng Ye, Qiang fu, Xueqian Wang, Xiu Li, Bo Yuan'
---
**Abstract:** A key challenge of continual reinforcement learning (CRL) in dynamic environments is to promptly adapt the RL agent’s behavior as the environment changes over its lifetime, while minimizing the catastrophic forgetting of the learned information. To address this challenge, in this article, we propose DaCoRL, i.e., dynamics-adaptive continual RL. DaCoRL learns a context-conditioned policy using progressive contextualization, which incrementally clusters a stream of stationary tasks in the dynamic environment into a series of contexts and opts for an expandable multihead neural network to approximate the policy. Specifically, we define a set of tasks with similar dynamics as an environmental context and formalize context inference as a procedure of online Bayesian infinite Gaussian mixture clustering on environment features, resorting to online Bayesian inference to infer the posterior distribution over contexts. Under the assumption of a Chinese restaurant process prior, this technique can accurately classify the current task as a previously seen context or instantiate a new context as needed without relying on any external indicator to signal environmental changes in advance. Furthermore, we employ an expandable multihead neural network whose output layer is synchronously expanded with the newly instantiated context, and a knowledge distillation regularization term for retaining the performance on learned tasks. As a general framework that can be coupled with various deep RL algorithms, DaCoRL features consistent superiority over existing methods in terms of the stability, overall performance and generalization ability, as verified by extensive experiments on several robot navigation and MuJoCo locomotion tasks.

&#x1F4C2; [Download paper here!](https://ieeexplore.ieee.org/document/10145851)<br />

**Bibtex**<br />
```bash
@article{zhang2023dynamics,
  title={Dynamics-Adaptive Continual Reinforcement Learning via Progressive Contextualization},
  author={Zhang, Tiantian and Lin, Zichuan and Wang, Yuxing and Ye, Deheng and Fu, Qiang and Yang, Wei and Wang, Xueqian and Liang, Bin and Yuan, Bo and Li, Xiu},
  journal={IEEE Transactions on Neural Networks and Learning Systems},
  year={2023},
  publisher={IEEE}
}
```