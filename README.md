# GM-for-offline-policy-learning-a-survey
This repository provides a survey on the applications of deep generative models for offline reinforcement learning and imitation learning. We cover multiple deep generative models, including VAEs, GANs, Normalizing Flows, Transformers, and Diffusion Models.

### 1. Variational Auto-Encoders (VAEs)

##### 1.1 Background Survey and General Knowledge Papers

* [CVPR 2018] [Cross-modal Deep Variational Hand Pose Estimation](https://openaccess.thecvf.com/content_cvpr_2018/papers/Spurr_Cross-Modal_Deep_Variational_CVPR_2018_paper.pdf)
* [ICLR 2017] [DEEP VARIATIONAL INFORMATION BOTTLENECK](https://arxiv.org/pdf/1612.00410.pdf)
* [Neurips 2015] [A Recurrent Latent Variable Model for Sequential Data](https://proceedings.neurips.cc/paper/2015/file/b618c3210e934362ac261db280128c22-Paper.pdf)
* [FTML 2019] [An Introduction to Variational Autoencoders](https://www.nowpublishers.com/article/Details/MAL-056)
* [ICLR 2014] [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114.pdf?source=post_page---------------------------)
* [ICLR 2016] [beta-vae: Learning basic visual concepts with a constrained variational framework](https://openreview.net/references/pdf?fbclid=IwAR0ToM3wj4gBJFQBkTF-rvD2RKTfmEWyBQ_So-VNZOOHWMbEJLvxxh3VfHw&id=Sy2fzU9gl)
* [IEEE FG 2020] [Gated Variational AutoEncoders: Incorporating Weak Supervision to Encourage Disentanglement](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9320221&casa_token=1NuD9zPCiQgAAAAA:8p0kC7zqkbWEWzrcw3PQOAIN0SyEEjhPoeOYboqEAZvRofY4HF35bMLtsOsLVy5bpuk5ng5T&tag=1)
* [Neurips 2015] [Learning Structured Output Representation using Deep Conditional Generative Models](https://proceedings.neurips.cc/paper_files/paper/2015/file/8d55a249e6baa5c06772297520da2051-Paper.pdf)
* [Neurips 2017] [Neural Discrete Representation Learning](https://proceedings.neurips.cc/paper/2017/file/7a98af17e63a0ac09ce2e96d03992fbc-Paper.pdf)
* [AAAI 2022] [State Deviation Correction for Offine Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/20886)

##### 1.2 Imitation Learning Papers
* [ArXiv 2020] [Complex Skill Acquisition Through Simple Skill Imitation Learning](https://arxiv.org/pdf/2007.10281.pdf)
* [ICML 2019] [CompILE: Compositional Imitation Learning and Execution](http://proceedings.mlr.press/v97/kipf19a/kipf19a.pdf)
* [IROS 2022] [SKILL-IL: Disentangling Skill and Knowledge in Multitask Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9981375&casa_token=cR1C-kYRmj4AAAAA:q__0TXiOVwxbRoH4dCLyR_wnQ-kPxO7jVJYaQD0K1VZ8Nj5H6-uzfvk_W915XAJ8zz8X2DcM?tag=1)
* [CoRL 2022] [Learning and Retrieval from Prior Data for Skill-based Imitation Learning](https://openreview.net/pdf?id=QgXArq7RIh)
* [CoRL 2019] [Task-Conditioned Variational Autoencoders for Learning Movement Primitives](http://proceedings.mlr.press/v100/noseworthy20a/noseworthy20a.pdf)
* [RSS 2023] [Behavior Retrieval: Few-Shot Imitation Learning by Querying Unlabeled Datasets](https://www.roboticsproceedings.org/rss19/p011.pdf)
* [CVPR 2020] [Imitative Non-Autoregressive Modeling for Trajectory Forecasting and Imputation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Qi_Imitative_Non-Autoregressive_Modeling_for_Trajectory_Forecasting_and_Imputation_CVPR_2020_paper.pdf)
* [IROS 2021] [Self-Supervised Disentangled Representation Learning for Third-Person Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9636363&casa_token=8rxU25a5M30AAAAA:kQBK0REcLZdEMvLBgZ1zA701lehbkwJnHw-cN7pF1FJOncrs1RLK0qmsvlR8qGEzpyIqf6ZX)
* [ICML 2022] [Bayesian Imitation Learning for End-to-End Mobile Manipulation](https://proceedings.mlr.press/v162/du22b/du22b.pdf)
* [CoRL 2020] [Generalization Guarantees for Imitation Learning](https://proceedings.mlr.press/v155/ren21a/ren21a.pdf)
* [RSS 2021] [Language Conditioned Imitation Learning over Unstructured Data](https://www.roboticsproceedings.org/rss17/p047.pdf)
* [IROS 2020] [Learning Visuomotor Policies for Aerial Navigation Using Cross-Modal Representations](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9341049&casa_token=z1V_OVjSYbYAAAAA:dDx2X6RLitFHfX_7xp7R2_a7J4KVZ3C2ZTP8eVRj0AQut8TKR9H_u9mmskFpp4Gy22jXltcf)
* [ArXiv 2019] [Trajectory VAE for multi-modal imitation](https://openreview.net/pdf?id=Byx1VnR9K7)
* [Neurips 2019] [Causal Confusion in Imitation Learning](https://proceedings.neurips.cc/paper_files/paper/2019/file/947018640bf36a2bb609d3557a285329-Paper.pdf)
* [IEEE CDC 2023] [Initial State Interventions for Deconfounded Imitation Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10383252&casa_token=ZJyKVnPGGN8AAAAA:4uV47CMW5MgsBGknbyk4sjnMlNcBNFhP80jvPjZMdvHPmiuPq56T9ov5IUqhW6hZX8JU94HU)
* [Neurips 2021] [Object-Aware Regularization for Addressing Causal Confusion in Imitation Learning](https://proceedings.neurips.cc/paper/2021/file/17a3120e4e5fbdc3cb5b5f946809b06a-Paper.pdf)
* [Neurips 2021] [An Empirical Investigation of Representation Learning for Imitation](https://openreview.net/pdf?id=kBNhgqXatI)
* [ICML 2020] [Intrinsic Reward Driven Imitation Learning via Generative Model](http://proceedings.mlr.press/v119/yu20d/yu20d.pdf)
* [ICCAS 2019] [Path Tracking Control Using Imitation Learning with Variational Auto-Encoder](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8971711&casa_token=jARtCQiMeeYAAAAA:onkkJlXxkmlIZwHbx1QjzhlWpm5KFsdiWyOac-n3MTd5NFO_nDZJI6oaiUaBFKjL-SP6y0nY)
* [ICRA 2018] [Vision-Based Multi-Task Manipulation for Inexpensive Robots Using End-To-End Learning from Demonstration](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8461076&casa_token=qXDKtEqT2-QAAAAA:PwL1ljHs_VxpLbCpv7QlV2nArsMifteUbgAcMVd82nFeC6BSmQfLfi-6BbSwRwuVzqzieovf)


##### 1.3 Offline Reinforcement Learning Papers
* [CoRL 2023] [Action-Quantized Offline Reinforcement Learning for Robotic Skill Learning](https://proceedings.mlr.press/v229/luo23a/luo23a.pdf)
* 