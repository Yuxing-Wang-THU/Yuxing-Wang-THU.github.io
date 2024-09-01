---
title: "Curriculum-based Co-design of Morphology and Control of Voxel-based Soft Robots"
collection: publications
permalink: /publication/2023-01-01-paper-title-number-1
excerpt: "Learning to design and control modular soft robots from easy to difficult. <br/><img src='/images/cuco.png' width=300>"
date: 2023-01-01
venue: 'International Conference on Learning Representations (ICLR)'
citation: 'Yuxing Wang, Shuang Wu, Haobo Fu, Qiang Fu, Tiantian Zhang, Yongzhe Chang, Xueqian Wang'
---
**Abstract:** Co-design of morphology and control of a Voxel-based Soft Robot (VSR) is challenging due to the notorious bi-level optimization. In this paper, we present a Curriculum-based Co-design (CuCo) method for learning to design and control VSRs through an easy-to-difficult process. Specifically, we expand the design space from a small size to the target size gradually through a predefined curriculum. At each learning stage of the curriculum, we use reinforcement learning to simultaneously train the design policy and the control policy, which is enabled by incorporating the design process into the environment and using differentiable policy representations. The converged morphology and the learned policies from last stage are inherited and then serve as the starting point for the next stage. In empirical studies, we show that CuCo is more efficient in creating larger robots with better performance by reusing the practical design and control patterns learned within each stage, in comparison to prior approaches that learn from scratch in the space of target size.

&#x1F4C2; [Download paper here!](https://openreview.net/pdf?id=r9fX833CsuN)<br />
&#x1F449; [Code is available here!](https://github.com/Yuxing-Wang-THU/ModularEvoGym)<br />
&#x1F449; [Poster is available here!](https://iclr.cc/media/PosterPDFs/ICLR%202023/10693.png?t=1679636195.527249)

**Bibtex**<br />
```bash
@inproceedings{wang2023curriculum,
  title={Curriculum-based Co-design of Morphology and Control of Voxel-based Soft Robots},
  author={Wang, Yuxing and Wu, Shuang and Fu, Haobo and Fu, Qiang and Zhang, Tiantian and Chang, Yongzhe and Wang, Xueqian},
  booktitle={The Eleventh International Conference on Learning Representations},
  year={2023}
}
```
&#x1F3A6;**Video**

<video id="video" controls="" preload="none" width=510>
    <source id="mp4" src="/images/cuco_video.mp4" type="video/mp4">
</videos>