# Deep Generative Models for Offline Reinforcement Learning and Imitation Learning
This repository provides a survey on the applications of deep generative models for offline reinforcement learning and imitation learning. We cover multiple deep generative models, including VAEs, GANs, Normalizing Flows, Transformers, and Diffusion Models.

### The paper has been accepted in TMLR with a Survey Certification: [https://openreview.net/pdf?id=Mm2cMDl9r5](https://openreview.net/pdf?id=Mm2cMDl9r5)
The content of the paper has been significantly improved during the submission process compared to the initial version.
Please consider citing this paper:
```bash
@article{
chen2024deep,
title={Deep Generative Models for Offline Policy Learning: Tutorial, Survey, and Perspectives on Future Directions},
author={Jiayu Chen and Bhargav Ganguly and Yang Xu and Yongsheng Mei and Tian Lan and Vaneet Aggarwal},
journal={Transactions on Machine Learning Research},
issn={2835-8856},
year={2024},
url={https://openreview.net/forum?id=Mm2cMDl9r5},
note={Survey Certification}
}
```

### 1. Variational Auto-Encoders (VAEs)

##### 1.1 Background Survey and General Knowledge Papers

* [ICLR 2014] [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114.pdf?source=post_page---------------------------)
* [Neurips 2015] [A Recurrent Latent Variable Model for Sequential Data](https://proceedings.neurips.cc/paper/2015/file/b618c3210e934362ac261db280128c22-Paper.pdf)
* [Neurips 2015] [Learning Structured Output Representation using Deep Conditional Generative Models](https://proceedings.neurips.cc/paper_files/paper/2015/file/8d55a249e6baa5c06772297520da2051-Paper.pdf)
* [Neurips 2015] [A Recurrent Latent Variable Model for Sequential Data](https://proceedings.neurips.cc/paper/2015/file/b618c3210e934362ac261db280128c22-Paper.pdf)
* [ICLR 2016] [beta-vae: Learning basic visual concepts with a constrained variational framework](https://openreview.net/references/pdf?fbclid=IwAR0ToM3wj4gBJFQBkTF-rvD2RKTfmEWyBQ_So-VNZOOHWMbEJLvxxh3VfHw&id=Sy2fzU9gl)
* [Neurips 2017] [Neural Discrete Representation Learning](https://proceedings.neurips.cc/paper/2017/file/7a98af17e63a0ac09ce2e96d03992fbc-Paper.pdf)
* [ICLR 2017] [DEEP VARIATIONAL INFORMATION BOTTLENECK](https://arxiv.org/pdf/1612.00410.pdf)
* [CVPR 2018] [Cross-modal Deep Variational Hand Pose Estimation](https://openaccess.thecvf.com/content_cvpr_2018/papers/Spurr_Cross-Modal_Deep_Variational_CVPR_2018_paper.pdf)
* [FTML 2019] [An Introduction to Variational Autoencoders](https://www.nowpublishers.com/article/Details/MAL-056)
* [IEEE FG 2020] [Gated Variational AutoEncoders: Incorporating Weak Supervision to Encourage Disentanglement](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9320221&casa_token=1NuD9zPCiQgAAAAA:8p0kC7zqkbWEWzrcw3PQOAIN0SyEEjhPoeOYboqEAZvRofY4HF35bMLtsOsLVy5bpuk5ng5T&tag=1)
* [AAAI 2022] [State Deviation Correction for Offine Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/20886)

##### 1.2 Imitation Learning Papers
* [ICRA 2018] [Vision-Based Multi-Task Manipulation for Inexpensive Robots Using End-To-End Learning from Demonstration](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8461076&casa_token=qXDKtEqT2-QAAAAA:PwL1ljHs_VxpLbCpv7QlV2nArsMifteUbgAcMVd82nFeC6BSmQfLfi-6BbSwRwuVzqzieovf)
* [ICCAS 2019] [Path Tracking Control Using Imitation Learning with Variational Auto-Encoder](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8971711&casa_token=jARtCQiMeeYAAAAA:onkkJlXxkmlIZwHbx1QjzhlWpm5KFsdiWyOac-n3MTd5NFO_nDZJI6oaiUaBFKjL-SP6y0nY)
* [ICML 2019] [CompILE: Compositional Imitation Learning and Execution](http://proceedings.mlr.press/v97/kipf19a/kipf19a.pdf)
* [CoRL 2019] [Task-Conditioned Variational Autoencoders for Learning Movement Primitives](http://proceedings.mlr.press/v100/noseworthy20a/noseworthy20a.pdf)
* [Neurips 2019] [Causal Confusion in Imitation Learning](https://proceedings.neurips.cc/paper_files/paper/2019/file/947018640bf36a2bb609d3557a285329-Paper.pdf)
* [ArXiv 2019] [Trajectory VAE for multi-modal imitation](https://openreview.net/pdf?id=Byx1VnR9K7)
* [CoRL 2020] [Generalization Guarantees for Imitation Learning](https://proceedings.mlr.press/v155/ren21a/ren21a.pdf)
* [CVPR 2020] [Imitative Non-Autoregressive Modeling for Trajectory Forecasting and Imputation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Qi_Imitative_Non-Autoregressive_Modeling_for_Trajectory_Forecasting_and_Imputation_CVPR_2020_paper.pdf)
* [IROS 2020] [Learning Visuomotor Policies for Aerial Navigation Using Cross-Modal Representations](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9341049&casa_token=z1V_OVjSYbYAAAAA:dDx2X6RLitFHfX_7xp7R2_a7J4KVZ3C2ZTP8eVRj0AQut8TKR9H_u9mmskFpp4Gy22jXltcf)
* [ICML 2020] [Intrinsic Reward Driven Imitation Learning via Generative Model](http://proceedings.mlr.press/v119/yu20d/yu20d.pdf)
* [ArXiv 2020] [Complex Skill Acquisition Through Simple Skill Imitation Learning](https://arxiv.org/pdf/2007.10281.pdf)
* [IROS 2021] [Self-Supervised Disentangled Representation Learning for Third-Person Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9636363&casa_token=8rxU25a5M30AAAAA:kQBK0REcLZdEMvLBgZ1zA701lehbkwJnHw-cN7pF1FJOncrs1RLK0qmsvlR8qGEzpyIqf6ZX)
* [Neurips 2021] [Object-Aware Regularization for Addressing Causal Confusion in Imitation Learning](https://proceedings.neurips.cc/paper/2021/file/17a3120e4e5fbdc3cb5b5f946809b06a-Paper.pdf)
* [Neurips 2021] [An Empirical Investigation of Representation Learning for Imitation](https://openreview.net/pdf?id=kBNhgqXatI)
* [RSS 2021] [Language Conditioned Imitation Learning over Unstructured Data](https://www.roboticsproceedings.org/rss17/p047.pdf)
* [IROS 2022] [SKILL-IL: Disentangling Skill and Knowledge in Multitask Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9981375&casa_token=cR1C-kYRmj4AAAAA:q__0TXiOVwxbRoH4dCLyR_wnQ-kPxO7jVJYaQD0K1VZ8Nj5H6-uzfvk_W915XAJ8zz8X2DcM?tag=1)
* [CoRL 2022] [Learning and Retrieval from Prior Data for Skill-based Imitation Learning](https://openreview.net/pdf?id=QgXArq7RIh)
* [ICML 2022] [Bayesian Imitation Learning for End-to-End Mobile Manipulation](https://proceedings.mlr.press/v162/du22b/du22b.pdf)
* [IEEE CDC 2023] [Initial State Interventions for Deconfounded Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10383252&casa_token=ZJyKVnPGGN8AAAAA:4uV47CMW5MgsBGknbyk4sjnMlNcBNFhP80jvPjZMdvHPmiuPq56T9ov5IUqhW6hZX8JU94HU)
* [RSS 2023] [Behavior Retrieval: Few-Shot Imitation Learning by Querying Unlabeled Datasets](https://www.roboticsproceedings.org/rss19/p011.pdf)



##### 1.3 Offline Reinforcement Learning Papers
* [ICML 2019] [Off-Policy Deep Reinforcement Learning without Exploration](http://proceedings.mlr.press/v97/fujimoto19a/fujimoto19a.pdf)
* [CoRL 2020] [PLAS: Latent Action Space for Offline Reinforcement Learning](https://proceedings.mlr.press/v155/zhou21b/zhou21b.pdf)
* [Neurips 2021] [Offline Meta Reinforcement Learning – Identifiability Challenges and Effective Data Collection Strategies](https://proceedings.neurips.cc/paper_files/paper/2021/file/248024541dbda1d3fd75fe49d1a4df4d-Paper.pdf)
* [Neurips 2021] [Offline Reinforcement Learning with Reverse Model-based Imagination](https://proceedings.neurips.cc/paper_files/paper/2021/file/f5e647292cc4e1064968ca62bebe7e47-Paper.pdf)
* [ICLR 2021] [Opal: Offline primitive discovery for accelerating offline reinforcement learning](https://openreview.net/pdf?id=V69LGwJ0lIN)
* [ACML 2021] [BRAC+: Improved Behavior Regularized Actor Critic for Offline Reinforcement Learning](https://proceedings.mlr.press/v157/zhang21a/zhang21a.pdf)
* [IJCAI 2021] [Boosting Offline Reinforcement Learning with Residual Generative Modeling](https://www.ijcai.org/proceedings/2021/0492.pdf)
* [ICLR 2021] [Risk-Averse Offline Reinforcement Learning](https://openreview.net/pdf?id=TBIzh9b5eaz)
* [L4DC 2021] [Offline Reinforcement Learning from Images with Latent Space Models](http://proceedings.mlr.press/v144/rafailov21a/rafailov21a.pdf)
* [AAAI 2022] [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/20855)
* [AAAI 2022] [Offine Reinforcement Learning as Anti-exploration](https://ojs.aaai.org/index.php/AAAI/article/view/20783)
* [Neurips 2022] [Supported Policy Optimization for Offline Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/caa934a507a952698d54efb24845fc4b-Paper-Conference.pdf)
* [ICML 2022] [Koopman Q-learning: Offline Reinforcement Learning via Symmetries of Dynamics](https://proceedings.mlr.press/v162/weissenbacher22a/weissenbacher22a.pdf)
* [IRAL 2022] [Hierarchical Planning Through Goal-Conditioned Offline Reinforcement Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9826807&casa_token=hG0zzkZ5t5cAAAAA:YbJettUnRFL2TaEkcLht0-hYtPM8IUFaKPvtG8V3_j-ikp6W9N1sAD8Q2uawkHL1NKDdWTwW&tag=1)
* [Neurips 2022] [Mildly Conservative Q-Learning for Offline Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/0b5669c3b07bb8429af19a7919376ff5-Paper-Conference.pdf)
* [ICCAS 2022] [Selective Data Augmentation for Improving the Performance of Offline Reinforcement Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10003747&casa_token=YfeS2Qp4l8sAAAAA:dPm8kLzIFuruHDbm-IagrTbBlvx3HvqH0aD3Xox2uITApexQMSE66uxCMLmwHYTv-a61snK_)
* [CoRL 2023] [Action-Quantized Offline Reinforcement Learning for Robotic Skill Learning](https://proceedings.mlr.press/v229/luo23a/luo23a.pdf)
* [CoRL 2023] [Generalization with Lossy Affordances: Leveraging Broad Offline Data for Learning Visuomotor Tasks](https://proceedings.mlr.press/v205/fang23a/fang23a.pdf)
* [CoRL 2023] [Latent Plans for Task-Agnostic Offline Reinforcement Learning](https://proceedings.mlr.press/v205/rosete-beas23a/rosete-beas23a.pdf)
* [IEEE TCDS 2023] [UAC: Offline Reinforcement Learning with Uncertain Action Constraint](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10158415&casa_token=QdkJztwbbyMAAAAA:jDUKJnQo7qZ-emdCrmWzAglYnhH3E68yXGVmY5-dFhv2LPGbr46O7Y2pM9Mic8y-gFpvXijm)
* [CoRL 2023] [Expansive Latent Planning for Sparse Reward Offline Reinforcement Learning](https://proceedings.mlr.press/v229/gieselmann23a/gieselmann23a.pdf)
* [ArXiv 2023] [On the Importance of the Policy Structure in Offline Reinforcement Learning](https://openreview.net/pdf?id=EJPWfoJRba)

### 2. Generative Adverserial Networks (GANs)
#### 2.1 Background Survey and General Knowledge Papers
* [Neurips 2016] [f-gan: Training generative neural samplers using variational divergence minimization](https://proceedings.neurips.cc/paper_files/paper/2016/file/cedebb6e872f539bef8c3f919874e9d7-Paper.pdf)
* [Neurips 2016] [InfoGAN: Interpretable Representation Learning by Information Maximizing Generative Adversarial Nets](https://proceedings.neurips.cc/paper_files/paper/2016/file/7c9d0b1f96aebd7b5eca8c3edaa19ebb-Paper.pdf)
* [Neurips 2017] [Triple Generative Adversarial Nets](https://proceedings.neurips.cc/paper/2017/file/86e78499eeb33fb9cac16b7555b50767-Paper.pdf)
* [ICML 2017] [Wasserstein Generative Adversarial Networks](http://proceedings.mlr.press/v70/arjovsky17a/arjovsky17a.pdf)
* [ICCV 2017] [DualGAN: Unsupervised Dual Learning for Image-to-Image Translation](https://openaccess.thecvf.com/content_ICCV_2017/papers/Yi_DualGAN_Unsupervised_Dual_ICCV_2017_paper.pdf)
* [IEEE TKDE 2023] [A Review on Generative Adversarial Networks: Algorithms, Theory, and Applications](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9625798)

#### 2.2 Imitation Learning - AIRL papers
* [ArXiv 2016] [A Connection Between Generative Adversarial
Networks, Inverse Reinforcement Learning, and Energy-Based Models](https://arxiv.org/pdf/1611.03852.pdf)
* [ICLR 2018] [Learning robust rewards with adversarial inverse reinforcement learning](https://openreview.net/pdf?id=rkHywl-A-)
* [ICML 2019] [Multi-Agent Adversarial Inverse Reinforcement Learning](http://proceedings.mlr.press/v97/yu19e/yu19e.pdf)
* [ICLR 2019] [Adversarial imitation via variational inverse reinforcement learning](https://openreview.net/pdf?id=HJlmHoR5tQ)
* [Neurips 2019] [Meta-Inverse Reinforcement Learning with Probabilistic Context Variables](https://proceedings.neurips.cc/paper_files/paper/2019/file/30de24287a6d8f07b37c716ad51623a7-Paper.pdf)
* [Neurips 2019] [SMILe : Scalable Meta Inverse Reinforcement Learning through Context-Conditional Policies](https://proceedings.neurips.cc/paper_files/paper/2019/file/2b8f621e9244cea5007bac8f5d50e476-Paper.pdf)
* [CoRL 2020] [f-IRL: Inverse Reinforcement Learning via State Marginal Matching](https://proceedings.mlr.press/v155/ni21a/ni21a.pdf)
* [ICML 2020] [Off-Policy Adversarial Inverse Reinforcement Learning](https://openreview.net/pdf?id=9mp5d073IhX)
* [ArXiv 2020] [oIRL: Robust Adversarial Inverse Reinforcement Learning with Temporally Extended Actions](https://arxiv.org/pdf/2002.09043.pdf)
* [IEEE RAL 2021] [Adversarial Inverse Reinforcement Learning With Self-Attention Dynamics Model](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9361118)
* [ICML 2023] [Multi-task Hierarchical Adversarial Inverse Reinforcement Learning](https://openreview.net/pdf?id=RBikc9cIZh)
* [IEEE TNNLS 2023] [Hierarchical Adversarial Inverse Reinforcement Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10250822&casa_token=28cHGDlHU3MAAAAA:PoOpgxYthGqgdlwq_OOX8UEZpn_CGBRqcMeudiuGE5NQp4ECeewp40G1AGXPkYW3XyqSJSNy)

#### 2.3 Imitation Learning - GAIL papers
* [Neurips 2016] [Generative adversarial imitation learning](https://proceedings.neurips.cc/paper_files/paper/2016/file/cc7e2b878868cbae992d1fb743995d8f-Paper.pdf)
* [ICML 2017] [End-to-End Differentiable Adversarial Imitation Learning](http://proceedings.mlr.press/v70/baram17a/baram17a.pdf)
* [Neurips 2017] [Robust Imitation of Diverse Behaviors](https://proceedings.neurips.cc/paper/2017/file/044a23cadb567653eb51d4eb40acaa88-Paper.pdf)
* [Neurips 2017] [Infogail: Interpretable imitation learning from visual demonstrations](https://proceedings.neurips.cc/paper/2017/file/2cd4e8a2ce081c3d7c32c3cde4312ef7-Paper.pdf)
* [Neurips 2017] [Multi-Modal Imitation Learning from Unstructured Demonstrations using Generative Adversarial Nets](https://proceedings.neurips.cc/paper_files/paper/2017/file/632cee946db83e7a52ce5e8d6f0fed35-Paper.pdf)
* [Neurips 2018] [Multi-Agent Generative Adversarial Imitation Learning](https://proceedings.neurips.cc/paper/2018/file/240c945bb72980130446fc2b40fbb8e0-Paper.pdf)
* [Neurips 2018] [A Bayesian Approach to Generative Adversarial Imitation Learning](https://proceedings.neurips.cc/paper_files/paper/2018/file/943aa0fcda4ee2901a7de9321663b114-Paper.pdf)
* [AAAI 2018] [OptionGAN: Learning Joint Reward-Policy Options Using Generative Adversarial Inverse Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/11775)
* [AAMAS 2018] [Burn-In Demonstrations for Multi-Modal Imitation Learning](https://www.ifaamas.org/Proceedings/aamas2018/pdfs/p1071.pdf)
* [ArXiv 2018] [Generative Adversarial Self-Imitation Learning](https://arxiv.org/pdf/1812.00950.pdf)
* [ICDM 2019] [Unveiling Taxi Drivers’ Strategies via cGAIL — Conditional Generative Adversarial Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8970802)
* [AISTATS 2019] [Risk-Sensitive Generative Adversarial Imitation Learning](http://proceedings.mlr.press/v89/lacotte19a/lacotte19a.pdf)
* [ICLR 2019] [Directed-Info GAIL: Learning Hierarchical Policies from Unsegmented Demonstrations using Directed Information](https://openreview.net/pdf?id=BJeWUs05KQ)
* [ICLR 2019] [Variational Discriminator Bottleneck: Improving Imitation Learning, Inverse RL, and GANs by Constraining Information Flow](https://openreview.net/pdf?id=HyxPx3R9tm)
* [AAMAS 2019] [Independent Generative Adversarial Self-Imitation Learning in Cooperative Multiagent Systems](https://www.ifaamas.org/Proceedings/aamas2019/pdfs/p1315.pdf)
* [AAMAS 2019] [Adversarial Imitation Learning from State-only Demonstrations](https://www.ifaamas.org/Proceedings/aamas2019/pdfs/p2229.pdf)
* [AISTATS 2019] [Sample-Efficient Imitation Learning via Generative Adversarial Nets](http://proceedings.mlr.press/v89/blonde19a/blonde19a.pdf)
* [ArXiv 2019] [Situated GAIL: Multitask imitation using task-conditioned adversarial inverse reinforcement learning](https://arxiv.org/pdf/1911.00238.pdf)
* [ACM KDD 2020] [xGAIL: Explainable Generative Adversarial Imitation Learning for Explainable Human Decision Analysis](https://dl.acm.org/doi/pdf/10.1145/3394486.3403186)
* [CoRL 2020] [Task-Relevant Adversarial Imitation Learning](https://proceedings.mlr.press/v155/zolna21a/zolna21a.pdf)
* [ICLR 2020] [State Alignment-based Imitation Learning](https://openreview.net/pdf?id=rylrdxHFDr)
* [IJCAI 2020] [Triple-GAIL: A Multi-Modal Imitation Learning Framework with Generative Adversarial Nets](https://www.ijcai.org/proceedings/2020/0405.pdf)
* [Neurips 2020] [f-GAIL: Learning f-Divergence for Generative Adversarial Imitation Learning](https://proceedings.neurips.cc/paper/2020/file/967990de5b3eac7b87d49a13c6834978-Paper.pdf)
* [ICML 2020] [Generative Adversarial Imitation Learning with Neural Network Parameterization: Global Optimality and Convergence Rate](http://proceedings.mlr.press/v119/zhang20d/zhang20d.pdf)
* [Neurocomputing 2020] [Deterministic generative adversarial imitation learning](https://pdf.sciencedirectassets.com/271597/1-s2.0-S0925231220X00117/1-s2.0-S0925231220300436/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEF8aCXVzLWVhc3QtMSJGMEQCIFzGA6e31VvdpghqiY05n6FhziJa9WTEs3sRK%2Fpb9B6kAiA6ehIRvRjsSquL77yBijC6IFdDcm77qpZuC6ngbFXWuCqzBQg4EAUaDDA1OTAwMzU0Njg2NSIMjOo9fjmbxnGUhTxPKpAFRu5Bk%2FEfPBl2axZ6KOl73KBA0g8lOJtg3D5E7YHmTrsRasgYU8O2T2Pk95P37lswutk9wTFWGvfphMBp3MEMjecYFaxMRPreaj95YuVazOzolFCp8w%2F6uLOOHVAbvsXMdnkfmTWc1hCkvnqka4jp%2BWQHbZj3KSLZmVDAHGc%2BoZwNHPKMOCtEJ5JBiTJ0nem4YS%2FLVJ%2BUz4img9BPERdqUrgO%2B3HAx3elXCH3m25OukwAb6PE5DyDjTODxJpEbtIYjbq3H8TbfhZ65E1ocola7sGhfN9gJXOMG2R42abkKgllyGS%2B4dnrj73s%2Ft8yO2ivr1AwSU7HAUTeX1HXGomlMx3sQ85OM1JLSkjAxNF8SwbG%2B6F4h5o7IbFkGkhVgc92PFF%2B7es7s29ZF4ARsHH%2Fq08hgyUDRFX2l1i9cl8BNOgtm4Yam%2FUx1WRf8CG%2Fdl6EcxGSIoVgxsUfK6wnBq6S%2BKtTxYRUHNRCtsU06FVEGb6%2FZ0NLyMXeahnVwVoZ%2F23tYzfJWQRXOX%2FR4zdVogUneIyvwzwYqSRvg%2BAkAYygMUZQgcV29zeg8QqBFEzZLDx6Y0up3Ojy6FktiS7QJIGYc%2BzA4aRTE%2BTmTi8%2BdcR8uY7kp6WWEmeRG2nCYVWQkBp0M7tu4ucfEXWQ5KCQ44h%2FJkeWBQK7kJcHC9r5hmBXk%2BWLSPynuuSKi%2BXKetJSDQD%2BnlA%2Bwze%2BiLpBWAeNXSztK8te84rxTYXbFKic04IGHUJjlUM6NkAYuvhTrulYo1wWw%2FZgQRFVJ4ndfp984QULVld1rR%2FtR3%2Fmx0oD19n5py6tJNtGtgJuk8XQQd385xSsHV8k%2B6JqBntfdlWtmn6MbRnEI1i1f92Hb%2F246iZ3v9EwsfyfrgY6sgHMOa0HHw0qoeSSxXcy0vbYhITeujMm0Hx2mUUql%2FtUPeAFCg1STgzk2xKhbuy9yz4aPjLNpE12mMpjJL78iyUedtCyjx%2BPonPUuiZdkxxoDqdq7XW51SBuvgwU8h9XWCCc9mzRmazPj7fdybVIljH5eisV4s1eZ8ODo%2BjcQ3TC88aEf8SbNHAJqsZQ%2FBbcHK7zYY0mO4WtYRcdT08PHS%2Fag4GzXn89za2f%2FBGbzL%2F1Fj5o&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240210T235008Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYSZSNF3FQ%2F20240210%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=b6a62c6e33fe721e1cf0e4aaee6992041a3a03b51aded2758e4a03404d46c823&hash=548b4efb7e4f8e48efa41363ce8aaed0ed05684bccc8582cd8a645a88159c38e&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0925231220300436&tid=spdf-ced13fed-c9d0-4db8-9b5f-784122515443&sid=dd934fcd41696140775af35847f8148c212dgxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=171c5d57555f52500e&rr=853840adef7c22df&cc=us)
* [ArXiv 2020] [ADAIL: Adaptive Adversarial Imitation Learning](https://arxiv.org/pdf/2008.12647.pdf)
* [ICML 2021] [Adversarial Option-Aware Hierarchical Imitation Learning](http://proceedings.mlr.press/v139/jing21a/jing21a.pdf)
* [ICML 2022] [Discriminator-Weighted Offline Imitation Learning from Suboptimal Demonstrations](https://proceedings.mlr.press/v162/xu22l/xu22l.pdf)
* [Neurocomputing 2022] [An imitation learning framework for generating multi-modal trajectories from unstructured demonstrations](https://pdf.sciencedirectassets.com/271597/1-s2.0-S0925231222X0026X/1-s2.0-S0925231222006579/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEGAaCXVzLWVhc3QtMSJHMEUCIQCmFSJP8YqT3ViOxQANyVVfrMKn5rQ3qcxKPfdNrabFUgIgefhAhhXqeLtAWuIgk7KvGxtuNBXISqgr4auLAVLl40MqsgUIORAFGgwwNTkwMDM1NDY4NjUiDNLNsY1TguIc5nzvWiqPBR48SsAhNj00oG9TOhhnXAT%2Bd0zxW79VL3h12CF2cM%2FNbJZ%2FADpY0lG7wbKdR%2FsA29H2Cx6ZagSE89kXbYyYVxqgGW4WU2%2BA6zA2NI%2FsRbsDSrII1KB%2FNcy4G7jsM3Ow%2B3AFDa%2FnoNNuerw1uNoSDQvYMNj1CuO2MmVrzg0LETMkhkdWVmEEX04pSuchn%2B6zeSZoTxHm1UXyImjx0g3E2OrYtIt%2F2mskhvR1WHJtzGPtkm2W3LzRwFAU6r0aTN2kkyYN88YcAD8coO8UuD8tGOrdatF4%2B1L4Z0tFvy7L9Js3dvZWq6yA9K4soN8aE87nhrNOOO1XIO5yNooWxc7hZev1HFqA9vvQ9AbGyG9t0lcx3jAmJENwUDnIrhBjThHH0A1crk581B4AyPvfEDmuOzfgo9TvJm7JwqEoZDEqkDTTyH7ADNxj1D9By1Is%2FK2NIdaQL7TDErRdY4Z%2FyR8Q7ptIekvmpO6Im12BNyKMo7GPQRQ30U%2BQtUT8sJveqrOVc8dGcRvJHwyGstp%2FI5zmDPG9CO9iWYDW8pH7xhzmTzX57nqC%2Bw%2B9voFqq9B%2B%2BqlD4X%2BDhdIwzG8kcntZKFNZoECwebHVYlwA5iWhwGFUS0Ce7A784OpAnDbkd1g4%2FlS4n%2F7ptdy7K7Qs%2FXzxcMRKWOh2VALgmlCkJMTZ6h4QMmpHONAEUExwzi8hrlDT6pDyBTMAsuDYEWDDzAnAalI1eR0ZQV17jhz7gdzfpejR477btpVF9XxkK5FPeKgfx53cyAxCMNTJO9hDrHx9QGQc%2BOxRcnhQhz2nMKFIrpGAG2VH92tr6v%2FaqkirAKDthOW2rbzxyQpAistX53E0TuFJYuD7zk%2ByvboyrM7JEnwz0FYwt4qgrgY6sQGn1Op4gTiSDfmCQCa4JHXWBvmLxCD9ai0ArzPn0Rtr%2FTCaheojnde3LShnU%2BexJgYSCUGGXAnjNNeHU62yn2Gd7eu%2BFzaJ52SpUNbo172cKaTe92HLzYWNmZjIYJZNopb9%2BofVMyJEwLWG%2FMlxzHQamWKcnND3hSiRT09zAfWsgZJqb7hAVwvFTiE5bqYoQSx1DTQ2YYWW1jhE7UcRMLMwqWDPZm8d8Etgx6%2BuSC%2Fu8ss%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240210T234825Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY2VJKYBRH%2F20240210%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=7d29941471139e1031e28a1ee168675bd71df9677bc2ea7b2669fd4a495eb445&hash=7bba7238f502bb133b6da5ce5c0ff7ffd40bfe15af5d3641dfd1e8a090cea016&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0925231222006579&tid=spdf-7ca04721-4cdd-48eb-80b2-fbe016b0f3d3&sid=dd934fcd41696140775af35847f8148c212dgxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=171c5d57555f55055d&rr=85383e2de8e22943&cc=us)
* [ArXiv 2022] [Latent Policies for Adversarial Imitation Learning](https://arxiv.org/pdf/2206.11299.pdf)
* [Neurips 2023] [Ess-InfoGAIL: Semi-supervised Imitation Learning from Imbalanced Demonstrations](https://openreview.net/pdf?id=jxhUNLoi4m)

##### 2.4 Offline Reinforcement Learning Papers
* [ICML 2022] [Regularizing a Model-based Policy Stationary Distribution to Stabilize Offline Reinforcement Learning](https://proceedings.mlr.press/v162/yang22b/yang22b.pdf)
* [Neurips 2022] [A Unified Framework for Alternating Offline Model Training and Policy Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/6dc02cf4905e873ca6fd0dfc7907e230-Paper-Conference.pdf)
* [Neurips 2022] [Model-based Trajectory Stitching for Improved Offline Reinforcement Learning](https://arxiv.org/pdf/2211.11603.pdf)
* [Neurips 2022] [Data-Driven Offline Decision-Making via Invariant Representation Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/559726fdfb19005e368be4ce3d40e3e5-Paper-Conference.pdf)
* [Neurips 2022] [Dual Generator Offline Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/fe51de4e7baf52e743b679e3bdba7905-Paper-Conference.pdf)
* [Neurips 2022] [S2P: State-conditioned Image Synthesis for Data Augmentation in Offline Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/4b32c2943a02331792877cc6b5205f49-Paper-Conference.pdf)
* [ArXiv 2022] [A Behavior Regularized Implicit Policy for Offline Reinforcement Learning](https://arxiv.org/pdf/2202.09673.pdf)
* [Neurips 2023] [GOPlan: Goal-conditioned Offline Reinforcement Learning by Planning with Learned Models](https://openreview.net/pdf?id=qU6tZmppN7)
* [Information Sciences 2023] [Safe batch constrained deep reinforcement learning with generative adversarial network](https://www.sciencedirect.com/science/article/abs/pii/S0020025523004322)
* [ArXiv 2023] [Model-based Offline Policy Optimization with Adversarial Network](https://arxiv.org/pdf/2309.02157.pdf)

### 3. Normalizing Flows (NFs)
#### 3.1 Background Survey and General Knowledge Papers
* [ICML 2015] [Variational Inference with Normalizing Flows](http://proceedings.mlr.press/v37/rezende15.pdf)
* [ICLR 2017] [Density estimation using real nvp](https://openreview.net/pdf?id=HkpbnH9lx)
* [IEEE TPAMI 2021] [Deep Generative Modelling: A Comparative Review of VAEs, GANs, Normalizing Flows, Energy-Based and Autoregressive Models](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9555209)
* [IEEE TPAMI 2021] [Normalizing Flows: An Introduction and Review of Current Methods](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9089305)
* [JMLR 2021] [Normalizing Flows for Probabilistic Modeling and Inference](https://www.jmlr.org/papers/volume22/19-1028/19-1028.pdf)

#### 3.2 Imitation Learning Papers
* [ICLR 2019] [Generative predecessor models for sample-efficient imitation learning](https://openreview.net/pdf?id=SkeVsiAcYm)
* [IROS 2020] [ImitationFlow: Learning Deep Stable Stochastic Dynamic Systems by Normalizing Flows](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9341035&casa_token=vkvNfCbglLgAAAAA:fTZxHVJsAjKKOXtsWZCyO0PfLRGs0elkygxRDjvbIoMwehpkIi-cQ8wWscof2MbOqxZ-6Cp_)
* [ArXiv 2020] [Imitative Planning using Conditional Normalizing Flow](https://arxiv.org/pdf/2007.16162.pdf)
* [Neurips 2021] [IL-flOw: Imitation Learning from Observation using Normalizing Flows](http://www.robot-learning.ml/2021/files/C6.pdf)
* [IEEE ITSC 2021] [Learning Normalizing Flow Policies Based on Highway Demonstrations](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9564456)
* [ICML 2023] [A Coupled Flow Approach to Imitation Learning](https://proceedings.mlr.press/v202/freund23a/freund23a.pdf)
* [Applied Intelligence 2023] [Imitation Learning by State-Only Distribution Matching](https://link.springer.com/article/10.1007/s10489-023-05062-w)
* [ArXiv 2023] [Stabilized Likelihood-based Imitation Learning via Denoising Continuous Normalizing Flow](https://openreview.net/forum?id=_fLxZ6VpXTH)
* [ArXiv 2023] [State-Only Imitation Learning by Trajectory Distribution Matching](https://openreview.net/pdf?id=qmf56RZbzFJ)
* [ArXiv 2023] [Universal Value Density Estimation for Imitation Learning and Goal-Conditioned Reinforcement Learning](https://openreview.net/pdf?id=S2UB9PkrEjF)

##### 3.3 Offline Reinforcement Learning Papers
* [Neurips 2022] [Uncertainty-Aware Reinforcement Learning for Risk-Sensitive Player Evaluation in Sports Game](https://proceedings.neurips.cc/paper_files/paper/2022/file/7f6e51d8298aa01b084b700ab91aff94-Paper-Conference.pdf)
* [AAAI 2023] [Flow to Control: Offine Reinforcement Learning with Lossless Primitive Discovery](https://ojs.aaai.org/index.php/AAAI/article/view/26286)
* [ArXiv 2023] [APAC: Authorized Probability-controlled Actor-Critic For Offline Reinforcement Learning](https://arxiv.org/pdf/2301.12130.pdf)
* [ArXiv 2023] [Let Offline RL Flow: Training Conservative Agents in the Latent Space of Normalizing Flows](https://arxiv.org/pdf/2211.11096.pdf)

##### 3.4 Reinforcement Learning Papers
* [CoRL 2019] [Leveraging exploration in off-policy algorithms via normalizing flows](http://proceedings.mlr.press/v100/mazoure20a/mazoure20a.pdf)
* [UAI 2020] [Randomized Value Functions via Multiplicative Normalizing Flows](http://proceedings.mlr.press/v115/touati20a/touati20a.pdf)
* [ICRA 2021] [Shaping Rewards for Reinforcement Learning with Imperfect Demonstrations using Generative Models](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9561333)
* [ICML 2022] [SAFER: Data-Efficient and Safe Reinforcement Learning via Skill Acquisition](https://openreview.net/pdf?id=N3Jwdt0GBrZ)
* [Neurips 2022] [CEIP: Combining Explicit and Implicit Priors for Reinforcement Learning with Demonstrations](https://proceedings.neurips.cc/paper_files/paper/2022/file/322e4a595afd9442a89f0bfaa441871e-Paper-Conference.pdf)


### 4. Transformers
#### 4.1 Background Survey and General Knowledge Papers
* [Neurips 2017] [Attention Is All You Need](https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)
* [AI Open 2022] [A survey of transformers](https://pdf.sciencedirectassets.com/777606/1-s2.0-S2666651022X00028/1-s2.0-S2666651022000146/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEIf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIQCZaCocasNuWxM8sqKoiTwKZz3WPkxU1ueLi%2BEIQasSpgIgJ%2BOKDycAfqWxA97Vfia%2BO6qM1Ts3%2BGyuxsdDGObOVIwqswUIXxAFGgwwNTkwMDM1NDY4NjUiDJp5WpY1NcTD77TsWiqQBY4HUGXZNR%2FZgEyBHCHpwaxHZbak0IV9wfbpz%2B3AmpZzBDl903cTYnjcrUEVJ%2Fj4VlOBT1E0lyDfDV%2BbSYeosAY7Zb9H0zIvZ4UpttRTNaXPTAeAwZVsSaCF%2F3eewc301xrJ3BHjr4RiNkYm1IZvEZQjiHY3r86EZPS1DC%2FIVnLAfIFNHriHfDPvSKF596JxIzDcYQ1brpbdMulQf5Bb6ngOZZJ7FeYYiFCsILEuP97pCRxOF3MjWDD1UTeCSY5dNpuFrUdg%2BLoXG7oOaTO6pf9SKHo88cG6If8izYgK45Wiho6Eubo4wZSnfdO%2BLtB0APIs%2Bp9LfCvMT2Etz4cXQutD8KEzsiKD6SFpK6i66MTRffWu84dMnjMOg47hTPLCnu%2FI%2BcWXMTwXpwuc9fPVNI2RIVTC8S96TdciZhmnkii%2FrBdVfZkXBtz6UTnaQ03Ux9y4Pw5S%2BY8x2dMHLnGbM0BKRVIT1I3pLRDzp6ilUPE1usQJrBEjSS3qNNBSTCIqbBEspmC%2BnlW%2FJJTYbXIvftnQ4QSoJ9xUyiSjNvYZJoeTeK7RKqJse1Se7PqjcykExFKwcU7chmfYCey48OAvxTHK%2BL9q44MEr9Ci8W444GtU1f6OKhSNNyK0s57RxXnicseHCPCfJfXbkHYN6yGLVSgG%2FlcqNUhBBXuNfOyK9EXp64JG8HVWhhCAa7ufox4dTX73LXwzcAI1cFLTYDJwJuIWuXxup%2FVKvvYY65WeS43uUDbyFibYLNS77B9G1xLcZaLITPrq6F4tQGnOXMWMn1wIpzMQ3NPrJpCCrZhhcZZHzjXa0xUbKehODfiACCLuXrWzIY5jhKM%2BLH%2FhfOZOoE9ZUy4j8Armnc%2B6R5M17pVmMJ3LqK4GOrEBZXPUKx16XlGiP%2B7dJMIAS88Ok02Mu65aWTgg94l9YG9UtsqqIMxQLDSCSllbcSHC%2FN6ZbNOh9vrGKuqFsTuT9lcXgbihbnLfNr0g5ICr6B8CgaW3WPHb2%2BoHeCueROQhHR%2FdjaflzUHqdjmGNZw9VwAqLn7izAtIqoKIxAusXguli6ZWtg0WiLMDkV9FYhsUh3eJ0k8GymMNAgxOVfCc3SwQnKc5e3gYF5gC8pqTh6H6&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240212T155913Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYWLVV6DXZ%2F20240212%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=aaf232ccb2cb226dd4b2b8097cd888dce74f63921d481c708da8950dfa4e8b2e&hash=c1c23ff70841cf4e4a8be81e3febfd2e819bf1f0c0c0114af6da0fbd3e1825da&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S2666651022000146&tid=spdf-265750b3-7515-45ac-bac9-c5a5f82bec1b&sid=98b334128e8fe047164a7af082f8b3992515gxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=171c5d575251565956&rr=8546099bc9942249&cc=us)
* [IEEE TPAMI 2022] [A Survey on Vision Transformer](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9716741&casa_token=1JgtZ09daqoAAAAA:nOlnra5Is6E5p5FQ1AgmCWf2iSAA69Q4eDRwCxqGp3HNvIgwIDI25LK-Iuh2feBRow0H2LaA&tag=1)
* [IJCAI 2023] [Transformers in Time Series: A Survey](https://www.ijcai.org/proceedings/2023/0759.pdf)
* [ArXiv 2023] [Transformer in Reinforcement Learning for Decision-Making: A Survey](https://arxiv.org/pdf/2301.03044.pdf)


#### 4.2 Imitation Learning Papers
* [IROS 2021] [Transformer-based deep imitation learning for dual-arm robot manipulation](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9636301&casa_token=9eYMYncsVVMAAAAA:yGUXKqLqOlqkXvn4C1YJqniC7DzzDvwSyyblL2G9xHTjg51QDn8ANXddiz44msBopROc4oiG)
* [CoRL 2021] [Transformers for One-Shot Visual Imitation](https://proceedings.mlr.press/v155/dasari21a/dasari21a.pdf)
* [ArXiv 2021] [Creating Multimodal Interactive Agents with Imitation and Self-Supervised Learning](https://arxiv.org/pdf/2112.03763.pdf)
* [Neurips 2022] [Behavior Transformers:Cloning k modes with one stone](https://proceedings.neurips.cc/paper_files/paper/2022/file/90d17e882adbdda42349db6f50123817-Paper-Conference.pdf)
* [CoRL 2022] [Transformer Adapters for Robot Learning](https://openreview.net/pdf?id=H--wvRYBmF)
* [CoRL 2022] [VIOLA: Imitation Learning for Vision-Based Manipulation with Object Proposal Priors](https://openreview.net/pdf?id=L8hCfhPbFho)
* [ICLR 2022] [Generalized Decision Transformer for Offline Hindsight Information Matching](https://openreview.net/pdf?id=CAjxVodl_v)
* [ICLR 2022] [Silver-Bullet-3D at ManiSkill 2021: Learning-from-Demonstrations and Heuristic Rule-based Methods for Object Manipulation](https://openreview.net/pdf?id=rNhxaETVybc)
* [ICRA 2022] [Memory-based gaze prediction in deep imitation learning for robot manipulation](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9812087&casa_token=qVvVYP1EdRsAAAAA:r9D4UcizjUVYzbA7TGK1GjxqKlqutxo0wQF-ibCyqDfEefSkZsmRM060GPEUglGWApQ3lJcd&tag=1)
* [IEEE RAL 2022] [What Matters in Language Conditioned Robotic Imitation Learning Over Unstructured Data](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9849097&casa_token=F0Abzk1YprsAAAAA:7FoqW0Dv2GO9haFQh95J8xPwj_AXYzfQRRuX6eLaaq7llL1PzwVDOt5NWR-1sTi37gYmawiS)
* [AAAI 2023] [Improving Long-Horizon Imitation through Instruction Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/25951)
* [ICCV 2023] [Is Imitation All You Need? Generalized Decision-Making with Dual-Phase Training](https://openaccess.thecvf.com/content/ICCV2023/papers/Wei_Is_Imitation_All_You_Need_Generalized_Decision-Making_with_Dual-Phase_Training_ICCV_2023_paper.pdf)
* [CoRL 2023] [PERCEIVER-ACTOR: A Multi-Task Transformer for Robotic Manipulation](https://proceedings.mlr.press/v205/shridhar23a/shridhar23a.pdf)
* [CVPR 2023] [A New Path: Scaling Vision-and-Language Navigation with Synthetic Instructions and Imitation Learning](https://openaccess.thecvf.com/content/CVPR2023/papers/Kamath_A_New_Path_Scaling_Vision-and-Language_Navigation_With_Synthetic_Instructions_and_CVPR_2023_paper.pdf)
* [ACM ICIKM 2023] [A Hierarchical Imitation Learning-based Decision Framework for Autonomous Driving](https://dl.acm.org/doi/pdf/10.1145/3583780.3615454?casa_token=tLvfQqF4h9MAAAAA:zPurBzWoArz72nLWcszF-astP2oD03S-fPwJkr0qWPRwYUMypaWR6_qEUcJ3sl9j0Amg9bTrBYhW)
* [IEEE RAL 2023] [Training Robots Without Robots: Deep Imitation Learning for Master-to-Robot Policy Transfer](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10083284&casa_token=6H3NHH_7MJ0AAAAA:wB4Xf3g-U3P2eRwFOQufe71ruGaclwjqANwM4o8CBwFgQH8INseLXAYCsovl3vSHXUEuVCB-)
* [ArXiv 2023] [Pretraining for Language Conditioned Imitation with Transformers](https://openreview.net/pdf?id=eCPCn25gat)
* [ArXiv 2023] [Detrive: Imitation Learning with Transformer Detection for End-to-End Autonomous Driving](https://arxiv.org/pdf/2310.14224.pdf)


##### 4.3 Offline Reinforcement Learning Papers
* [ICML 2020] [Stabilizing Transformers for Reinforcement Learning](http://proceedings.mlr.press/v119/parisotto20a/parisotto20a.pdf)
* [ICML 2020] [Working Memory Graphs](http://proceedings.mlr.press/v119/loynd20a/loynd20a.pdf)
* [ICML 2021] [Demonstration-Conditioned Reinforcement Learning for Few-Shot Imitation](http://proceedings.mlr.press/v139/dance21a/dance21a.pdf)
* [ICML 2021] [Decision Transformer: Reinforcement Learning via Sequence Modeling](https://proceedings.neurips.cc/paper_files/paper/2021/file/7f489f642a0ddb10272b5c31057f0663-Paper.pdf)
* [ICML 2021] [Catformer: Designing Stable Transformers via Sensitivity Analysis](http://proceedings.mlr.press/v139/davis21a/davis21a.pdf)
* [ICLR 2021] [Efficient Transformers in Reinforcement Learning using Actor-Learner Distillation](https://openreview.net/pdf?id=uR9LaO_QxF)
* [ICLR 2021] [UPDeT: Universal Multi-agent RL via Policy Decoupling with Transformers](https://openreview.net/pdf?id=v9c7hr9ADKx)
* [Neurips 2021] [Offline Reinforcement Learning as One Big Sequence Modeling Problem](https://proceedings.neurips.cc/paper/2021/file/099fe6b0b444c23836c4a5d07346082b-Paper.pdf)
* [ArXiv 2021] [Transfer learning with causal counterfactual reasoning in Decision Transformers](https://arxiv.org/pdf/2110.14355.pdf)
* [ArXiv 2021] [Offline pre-trained multi-agent decision transformer: One big sequence model tackles all smac tasks](https://arxiv.org/pdf/2112.02845.pdf)
* [ICML 2022] [Online Decision Transformer](https://proceedings.mlr.press/v162/zheng22c/zheng22c.pdf)
* [ICML 2022] [Prompting Decision Transformer for Few-Shot Policy Generalization](https://proceedings.mlr.press/v162/xu22g/xu22g.pdf)
* [ICML 2022] [Addressing Optimism Bias in Sequence Modeling for Reinforcement Learning](https://proceedings.mlr.press/v162/villaflor22a/villaflor22a.pdf)
* [ICLR 2022] [RvS: What is Essential for Offline RL via Supervised Learning?](https://openreview.net/pdf?id=S874XAIpkR-)
* [Neurips 2022] [Dynamics-Augmented Decision Transformer for Offline Dynamics Generalization](https://openreview.net/pdf?id=ReNyLYfUdr)
* [Neurips 2022] [On the Effect of Pre-training for Transformer in Different Modality on Offline Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/c5eddf0069fe150ac2c768e2969e38d1-Paper-Conference.pdf)
* [Neurips 2022] [Multi-Game Decision Transformers](https://proceedings.neurips.cc/paper_files/paper/2022/file/b2cac94f82928a85055987d9fd44753f-Paper-Conference.pdf)
* [Neurips 2022] [Offline Multi-Agent Reinforcement Learning with Knowledge Distillation](https://proceedings.neurips.cc/paper_files/paper/2022/file/01d78b294d80491fecddea897cf03642-Paper-Conference.pdf)
* [Neurips 2022] [Transformer-based Working Memory for Multiagent Reinforcement Learning with Action Parsing](https://proceedings.neurips.cc/paper_files/paper/2022/file/e1cf57f1e104c6c05e31894c15a65e99-Paper-Conference.pdf)
* [Neurips 2022] [Multi-Agent Reinforcement Learning is A Sequence Modeling Problem](https://proceedings.neurips.cc/paper_files/paper/2022/file/69413f87e5a34897cd010ca698097d0a-Paper-Conference.pdf)
* [Neurips 2022] [When does return-conditioned supervised learning work for offline reinforcement learning?](https://proceedings.neurips.cc/paper_files/paper/2022/file/0a2f65c9d2313b71005e600bd23393fe-Paper-Conference.pdf)
* [Neurips 2022] [You Can’t Count on Luck: Why Decision Transformers and RvS Fail in Stochastic Environments](https://proceedings.neurips.cc/paper_files/paper/2022/file/fe90657b12193c7b52a3418bdc351807-Paper-Conference.pdf)
* [Neurips 2022] [Bootstrapped Transformer for Offline Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2022/file/e0ccda3cb17b084a6f43c62cfac4784b-Paper-Conference.pdf)
* [Neurips 2022] [CLaP: Conditional Latent Planners for Offline Reinforcement Learning](https://openreview.net/pdf?id=OQP7leJkAu)
* [AAAI 2022] [Transformer-based Value Function Decomposition for Cooperative Multi-agent Reinforcement Learning in StarCraft](https://ojs.aaai.org/index.php/AIIDE/article/view/21954)
* [ECCV 2022] [StARformer: Transformer with State-Action-Reward Representations for Visual Reinforcement Learning](https://link.springer.com/chapter/10.1007/978-3-031-19842-7_27)
* [IEEE RAL 2022] [Efficient Spatiotemporal Transformer for Robotic Reinforcement Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9807399&casa_token=i7W7LBh5VPAAAAAA:A1iqJynv_QHd4f0Plko8vmW3-7GuKAqvAo-C_FJYss6MzXu55Tq_3MFCkRLcJ50xcToD-p87&tag=1)
* [ArXiv 2022] [TransDreamer: Reinforcement Learning with Transformer World Models](https://arxiv.org/pdf/2202.09481.pdf)
* [ArXiv 2022] [Can Wikipedia Help Offline Reinforcement Learning?](https://arxiv.org/pdf/2201.12122.pdf)
* [ArXiv 2022] [Semi-supervised Offline Reinforcement Learning with Pre-trained Decision Transformers](https://openreview.net/pdf?id=fwJWhOxuzV9)
* [ArXiv 2022] [Switch Trajectory Transformer with Distributional Value Approximation for Multi-Task Reinforcement Learning](https://arxiv.org/pdf/2203.07413.pdf)
* [ICML 2023] [Future-conditioned Unsupervised Pretraining for Decision Transformer](https://proceedings.mlr.press/v202/xie23b/xie23b.pdf)
* [ICML 2023] [Q-learning Decision Transformer: Leveraging Dynamic Programming for Conditional Sequence Modelling in Offline RL](https://proceedings.mlr.press/v202/yamagata23a/yamagata23a.pdf)
* [ICML 2023] [Constrained Decision Transformer for Offline Safe Reinforcement Learning](https://openreview.net/pdf?id=9VKCBHESq0)
* [ICML 2023] [Semi-Supervised Offline Reinforcement Learning with Action-Free Trajectories](https://proceedings.mlr.press/v202/zheng23b/zheng23b.pdf)
* [ICLR 2023] [Dichotomy of Control: Separating What You Can Control from What You Cannot](https://openreview.net/pdf?id=DEGjDDV22pI)
* [IROS 2023] [Hierarchical Decision Transformer](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10342230&casa_token=tLY6SeGLAM8AAAAA:eymIjTr2IR58xM-xSSW7qP8U2bM9Di3ndTz-fk7-kUAK7RR9l_dMWf9_zvICVsy1wn5YFCHH&tag=1)
* [IJCAI 2023] [Towards Long-delayed Sparsity: Learning a Better Transformer through Reward Redistribution](https://www.ijcai.org/proceedings/2023/0522.pdf)
* [TMLR 2023] [A Generalist Agent](https://openreview.net/pdf?id=1ikK0kHjvj)
* [CoRL 2023] [Q-Transformer: Scalable Offline Reinforcement Learning via Autoregressive Q-Functions](https://proceedings.mlr.press/v229/chebotar23a/chebotar23a.pdf)
* [UAI 2023] [A Trajectory is Worth Three Sentences: Multimodal Transformer for Offline Reinforcement Learning](https://proceedings.mlr.press/v216/wang23d/wang23d.pdf)
* [AI 2023] [Transform networks for cooperative multi-agent deep reinforcement learning](https://link.springer.com/article/10.1007/s10489-022-03924-3)
* [ArXiv 2023] [Self-Confirming Transformer for Locally Consistent Online Adaptation in Multi-Agent Reinforcement Learning](https://arxiv.org/pdf/2310.04579.pdf)
* [ArXiv 2023] [Contextual Transformer for Offline Reinforcement Learning](https://openreview.net/pdf?id=7pl0FRiS0Td)
* [ArXiv 2023] [Skill Decision Transformer](https://arxiv.org/pdf/2301.13573.pdf)
* [ArXiv 2023] [Environment Transformer and Policy Optimization for Model-Based Offline Reinforcement Learning](https://arxiv.org/pdf/2303.03811.pdf)
* [ArXiv 2023] [Graph Decision Transformer](https://arxiv.org/pdf/2303.03747.pdf)
* [ArXiv 2023] [Critic-Guided Decision Transformer for Offline Reinforcement Learning](https://arxiv.org/pdf/2312.13716.pdf)
* [ArXiv 2023] [MCTransformer: Combining Transformers And Monte-Carlo Tree Search For Offline Reinforcement Learning](https://openreview.net/forum?id=-94tJCOo7OM)

 
### 5. Diffusion Models (DMs)
#### 5.1 Background Survey and General Knowledge Papers
* [ArXiv 2022] [Understanding Diffusion Models: A Unified Perspective](https://arxiv.org/pdf/2208.11970.pdf)
* [ACM Computing Surveys 2023] [Diffusion Models: A Comprehensive Survey of Methods and Applications](https://dl.acm.org/doi/full/10.1145/3626235?casa_token=aCtHWddU7YcAAAAA:JIsxi-YuGFCzybKJWYMyRvekMMPX44nmNBnoG8XRVD2eb34UP-m1cQgsowJeDokACL10RV4Y1VxL)
* [Neurips 2023] [Understanding Diffusion Objectives as the ELBO with Simple Data Augmentation](https://openreview.net/pdf?id=NnMEadcdyD)


#### 5.2 Imitation Learning Papers
* [ICLR 2023] [Imitating human behaviour with diffusion models](https://openreview.net/pdf?id=-pqCZ8tbtd)
* [CoRL 2023] [Waypoint-Based Imitation Learning for Robotic Manipulation](https://openreview.net/pdf?id=X0cmlTh1Vl)
* [ArXiv 2023] [Constrained-Context Conditional Diffusion Models for Imitation Learning](https://arxiv.org/pdf/2311.01419.pdf)
* [ArXiv 2023] [Goal-Conditioned Imitation Learning using Score-based Diffusion Policies](https://arxiv.org/pdf/2304.02532.pdf)
* [ArXiv 2023] [Diffusion Policy: Visuomotor Policy Learning via Action Diffusion](https://arxiv.org/pdf/2303.04137.pdf)
* [ArXiv 2023] [Imitation Learning from Purified Demonstrations](https://arxiv.org/pdf/2310.07143.pdf)
* [ICLR 2024] [Memory-Consistent Neural Networks for Imitation Learning](https://openreview.net/pdf?id=R3Tf7LDdX4)
* [ArXiv 2024] [Good Better Best: Self-Motivated Imitation Learning for noisy Demonstrations](https://openreview.net/pdf?id=tIsYpRxMvr)


##### 5.3 Offline Reinforcement Learning Papers
* [ICML 2022] [Planning with Diffusion for Flexible Behavior Synthesis](https://proceedings.mlr.press/v162/janner22a/janner22a.pdf)
* [ICML 2023] [Contrastive Energy Prediction for Exact Energy-Guided Diffusion Sampling in Offline Reinforcement Learning](https://openreview.net/pdf?id=LucUrr5kUi)
* [ICML 2023] [MetaDiffuser: Diffusion Model as Conditional Planner for Offline Meta-RL](https://openreview.net/pdf?id=IKCk6th595)
* [ICML 2023] [AdaptDiffuser: Diffusion Models as Adaptive Self-evolving Planners](https://openreview.net/pdf?id=3ETNXs54HB)
* [ICML 2023] [Discrete Diffusion Reward Guidance Methods for Offline Reinforcement Learning](https://openreview.net/pdf?id=s4cSgzGudq)
* [ICML 2023] [Hierarchical Diffusion for Offline Decision Making](https://proceedings.mlr.press/v202/li23ad/li23ad.pdf)
* [ICLR 2023] [Diffusion Policies as an Expressive Policy Class for Offline Reinforcement Learning](https://openreview.net/pdf?id=AHvFDPi-FA)
* [ICLR 2023] [Is Conditional Generative Modeling all you need for Decision-Making?](https://openreview.net/pdf?id=SUnVLf3djD7)
* [ICLR 2023] [Offline Reinforcement Learning via High-Fidelity Generative Behavior Modeling](https://openreview.net/pdf?id=42zs3qa2kpy)
* [ICLR 2023] [Sample Generations for Reinforcement Learning via Diffusion Models](https://openreview.net/pdf?id=OQ1nwQpEPj)
* [CoRL 2023] [Fighting Uncertainty with Gradients: Offline Reinforcement Learning via Diffusion Score Matching](https://proceedings.mlr.press/v229/suh23a/suh23a.pdf)
* [Neurips 2023] [Efficient Diffusion Policies for Offline Reinforcement Learning](https://openreview.net/pdf?id=0P6uJtndWu)
* [Neurips 2023] [EDGI: Equivariant Diffusion for Planning with Embodied Agents](https://openreview.net/pdf?id=OrbWCpidbt)
* [Neurips 2023] [Diffusion Model is an Effective Planner and Data Synthesizer for Multi-Task Reinforcement Learning](https://openreview.net/pdf?id=fAdMly4ki5)
* [Neurips 2023] [Conformal Prediction for Uncertainty-Aware Planning with Diffusion Dynamics Model](https://openreview.net/pdf?id=VeO03T59Sh)
* [ArXiv 2023] [DiffCPS: Diffusion Model based Constrained Policy Search for Offline Reinforcement Learning](https://arxiv.org/pdf/2310.05333.pdf)
* [ArXiv 2023] [Boosting Continuous Control with Consistency Policy](https://arxiv.org/pdf/2310.06343.pdf)
* [ArXiv 2023] [Consistency Models as a Rich and Efficient Policy Class for Reinforcement Learning](https://arxiv.org/pdf/2309.16984.pdf)
* [ArXiv 2023] [Beyond Conservatism: Diffusion Policies in Offline Multi-agent Reinforcement Learning](https://arxiv.org/pdf/2307.01472.pdf) 
* [ArXiv 2023] [IDQL: Implicit Q-Learning as an Actor-Critic Method with Diffusion Policies](https://arxiv.org/pdf/2304.10573.pdf)
* [ArXiv 2023] [Instructed Diffuser with Temporal Condition Guidance for Offline Reinforcement Learning](https://arxiv.org/pdf/2306.04875.pdf)
* [ArXiv 2023] [MADIFF: Offline Multi-agent Learning with Diffusion Models](https://arxiv.org/pdf/2305.17330.pdf)
* [ArXiv 2023] [SafeDiffuser: Safe Planning with Diffusion Probabilistic Models](https://arxiv.org/pdf/2306.00148.pdf)
* [ICLR 2024] [Reasoning with Latent Diffusion in Offline Reinforcement Learning](https://openreview.net/pdf?id=tGQirjzddO)
* [IEEE RAL 2024] [Diffusion Policies for Out-of-Distribution Generalization in Offline Reinforcement Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10423845&casa_token=Ph7hKLqJjhEAAAAA:h28oE-_hh8Yy8e-4NbFLx7Syxz3CPmuKIYdm5WFn7m4WL1RxMQZ5jZg88DaIepv9lg38pFyh&tag=1)
