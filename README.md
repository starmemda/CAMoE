# CAMoE + Dual SoftMax Loss (DSL): Improving Video-Text Retrieval by Multi-Stream Corpus Alignment and Dual Softmax Loss
This is official implement of ["Improving Video-Text Retrieval by Multi-Stream Corpus Alignment and Dual Softmax Loss"](https://arxiv.org/abs/2109.04290).

## Open source project

We intented to publish the dual softmax loss firstly, the entire version will be available before the end of this year.

## Abstract

Employing large-scale pre-trained model CLIP to conduct video-text retrieval task (VTR) has become a new trend, which exceeds previous VTR methods. Though, due to the heterogeneity of structures and contents between video and text, previous CLIP-based models are prone to overfitting in the training phase, resulting in relatively poor retrieval performance. In this paper, we propose a multi-stream Corpus Alignment network with single gate Mixture-of-Experts (CAMoE) and a novel Dual Softmax Loss (DSL) to solve the two heterogeneity. The CAMoE employs Mixture-of-Experts (MoE) to extract multi-perspective video representations, including action, entity, scene, etc., then align them with the corresponding part of the text. In this stage, we conduct massive explorations towards the feature extraction module and feature alignment module. DSL is proposed to avoid the one-way optimum-match which occurs in previous contrastive methods. Introducing the intrinsic prior of each pair in a batch, DSL serves as a reviser to correct the similarity matrix and achieves the dual optimal match. DSL is easy to implement with only one-line code but improves significantly. The results show that the proposed CAMoE and DSL are of strong efficiency, and each of them is capable of achieving State-of-The-Art (SOTA) individually on various benchmarks such as MSR-VTT, MSVD, LSMDC, DiDeMo, and Activitynet. Further, with both of them, the performance is advanced to a big extend, surpassing the previous SOTA methods for the average of around 4~5\% R@1 in various VTR datasets.


## The Experimental Result

| dataset | T2V-R@1 | V2T-R@1 |
| :---: | :---: | :---: |
| MSR-VTT-1k | 48.8 | 50.3 |
| MSR-VTT | 32.9 | 59.8 |
| MSVD | 51.8 | 69.3 |
| DiDeMo | 43.8 | 45.5 |
| Activitynet | 51.0 | 49.9 |

Note that all the results achieve the SOTA.

## Citing artical
Pleadse cite this article as:
```
@misc{cheng2021improving,
      title={Improving Video-Text Retrieval by Multi-Stream Corpus Alignment and Dual Softmax Loss}, 
      author={Xing Cheng and Hezheng Lin and Xiangyu Wu and Fan Yang and Dong Shen},
      year={2021},
      eprint={2109.04290},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
