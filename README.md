# Papers-Continual-RL
I am constantly collecting papers on Continual Reinforcement Learning published on high-profile ML conferences or journals. Although there are too many challenges in continual RL, e.g., less formal definition and incomplete foundations, it is still a valuable research field that helps to address the challenges in the **non-stationary environments** in RL. Please feel free to let us know if you feel we have missed some important papers.

**Contact** : [Ke Sun](https://sites.google.com/view/kesun), ksun6@ualberta.ca

## 2025

* [Prevalence of Negative Transfer in Continual Reinforcement Learning: Analyses and a Simple Baseline](https://openreview.net/forum?id=KAIqwkB3dT) (ICLR 2025)
>

## 2024





* [Fast TRAC: A Parameter-Free Optimizer for Lifelong Reinforcement Learning](https://openreview.net/pdf?id=QEaHE4TUgc) (NeurIPS 2024)
> The authors bring the idea from parameter-free online convex optimization to design a new advanced optimizer (based on SGD, Adam) to address the loss of plasiticity issue in continual RL.


* [Parseval Regularization for Continual Reinforcement Learning](https://openreview.net/pdf?id=RB1F2h5YEx) (NeurIPS 2024)
> This paper focuses on the loss of plasticity of continual RL from the perspective of optimization, one of the important aspects of continual RL. The authors propose to use Parseval regularization, which maintains orthogonality of weight matrice and thus enhances the optimization in the presence of new tasks.



* [Self-composing policies for scalable continual RL](https://github.com/mikelma/componet) (ICML 2024)
> Like PackNet, this paper designs a growing NN that uses the attention module to integrate the output from previous policies and current policy. The growing NN is thus deployed for the new task and empirically achieve great performance in terms of bot plasticity (forward transfer and learning curve) and catastrophic forgetting (average performance) in Metaworld and Atari games.



* [CPPO: Continual Learning for Reinforcement Learning with Human Feedback](https://openreview.net/forum?id=86zAUE80pP) (ICLR 2024)
> This paper is the first to consider the continual RLHF with dynamic preference learning, by using the sample-wise reweighting method based on the performance and variance.

* [Loss of plasticity in deep continual learning](https://www.nature.com/articles/s41586-024-07711-7) (Nature 2024)
> This paper empirically studies the loss of plasticity issue from supervised learning to reinforcement learning and proposes the continual propogation algorithm to mitigate the loss of plasticity issue partially.



## 2023

* [Replay-enhanced Continual Reinforcement Learning](https://openreview.net/forum?id=91hfMEUukm) (TMLR 2023)
> This paper incorporates normalized Q function and policy distillation (KL regularization) in SAC to address the reward scaling and catastrophic forgetting issues in continual RL. Experiments include several common baselines and are conducted in Continual World.

* [Building a Subspace of Policies for Scalable Continual Learning](https://arxiv.org/abs/2211.10445) (ICLR 2023)
> This paper incrementally expands the subspace of policies to balance the agent's size and performance in continual RL. Although the result is very reasonable, it may suffer from the high computation, and increasing the agent's size may not be admissible in practice.

* [A Definition of Continual Reinforcement Learning](https://arxiv.org/abs/2307.11046) (NeurIPS 2023)
> The authors are the first to provide a conceptual definition of continual RL, but unfortunately, no practical algorithms are proposed.


* [Prediction and Control in Continual Reinforcement Learning](https://arxiv.org/abs/2312.11669) (NeurIPS 2023)
> This paper studies the value-based continual RL in both prediction and control settings, and proposes to decompose the value function into two components that are updated in different time-scaling, which mirror the function of neocortex and hippocampus

* [COOM: A Game Benchmark for Continual Reinforcement Learning](https://openreview.net/pdf?id=qmCxdPkNsa) (NeurIPS 2023)
> Benchmark on Images: Tensorflow

* [Continual Task Allocation in Meta-Policy Network via Sparse Prompting](https://arxiv.org/abs/2305.18444) (ICML 2023)
> The paper proposes sparse prompting to address continual RL problems, which learns over-complete dictionaries to produce sparse masks as prompts extracting a sub-network for each task from a meta-policy network.


* [Task-Agnostic Continual Reinforcement Learning: Gaining Insights and Overcoming Challenges](https://arxiv.org/abs/2205.14495) (CoLLAs 2023)
> The paper considers continual RL from the perspective of POMDP, and it also involves some insightful discussions.


## 2022 and Before 

* [Lifelong Robotic Reinforcement Learning by Retaining Experiences](https://proceedings.mlr.press/v199/xie22a/xie22a.pdf) (CoLLAs 2022)
> 



* [Disentangling Transfer in Continual Reinforcement Learning](https://arxiv.org/abs/2209.13900) (NeurIPS 2022)
> This paper empirically investigates the impact of different components in SAC on continual RL, and proposes the behavior cloning method to combine improvements.

* [Towards Evaluating Adaptivity of Model-Based Reinforcement Learning Methods](https://arxiv.org/pdf/2204.11464) (ICML 2022)
> This paper investigates the adaptive power of model-based RL to local reward changes and reveals 4 failure modes. It finds that a large replay buffer from old data hurts the adaptivity/plasticity, while a small one tends to lead to catastraphic forgetting, suggesting a trade-off between them to achieve more ambitious continual RL problems.

* [Continual World: A Robotic Benchmark For Continual Reinforcement Learning](https://arxiv.org/abs/2105.10919) (NeurIPS 2021)
> Benchmark: Continual World, 10 manipulation tasks from MetaWorld

* [Towards Continual Reinforcement Learning: A Review and Perspectives](https://arxiv.org/abs/2105.10919) (Journal of Artificial Intelligence Research (JAIR)) 2020
> The first review of continual RL, however, most of the related papers are about continual learning instead of RL.

* [Policy Consolidation for Continual Reinforcement Learning](https://arxiv.org/abs/1902.00255) (ICML 2019）
> The authors proposed to use policy consolidation method, in which the policy network interacts with a series of hidden networks in different time-scales to mitigate catastrophic forgetting.

* [Continual Reinforcement Learning with Complex Synapses](https://arxiv.org/abs/1802.07239) (ICML 2018)
> This paper incorporates a synaptic model in RL agents to mitigate catastrophic forgetting in continual RL. This study is inspired by neuroscience, but its experiments are restricted on tabular experiments.

* [State Abstractions for Lifelong Reinforcement Learning](https://proceedings.mlr.press/v80/abel18a/abel18a.pdf) (ICML 2018)
> This paper brings state abstraction to lifelong RL and provides a theoretical analysis.



**Remark**. There are also a few papers before 2022 collected in https://github.com/ContinualAI/continual-learning-papers#continual-reinforcement-learning.

