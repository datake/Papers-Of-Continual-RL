# Papers-Continual-RL
I am constantly collecting papers on Continual Reinforcement Learning published on high-profile ML conferences or journals. Although there are too many challenges in continual RL, e.g., less formal definition and incomplete foundations, it is still a valuable research field that helps to address the challenges in the **non-stationary environments** in RL. Please feel free to let us know if you feel we have missed some important papers.

**Contact** : [Ke Sun](https://sites.google.com/view/kesun), ksun6@ualberta.ca



## 2025


* [Continual Knowledge Adaptation for Reinforcement Learning](https://neurips.cc/virtual/2025/poster/118130) (NeurIPS 2025)


* [Tackling Continual Offline RL through Selective Weights Activation on Aligned Spaces](https://arxiv.org/abs/2410.15698) (NeurIPS 2025)

> This paper leverages vector quantization to align the different state and action spaces of various tasks by selective weight activations. The experiments are on CW10, Mujoco, and D4RL.

* [Knowledge Retention for Continual Model-Based Reinforcement Learning](https://arxiv.org/abs/2503.04256) (ICML 2025)
> This paper uses VAE to continually learn a generative model by freezing the previous one to replay past experience. At the same time, to facilitate plasticity, a new learner is encouraged to explore the new state and action pairs beyond the state-action scope of the generative/world model, i.e., the past knowledge, leading to exploration of new knowledge in the new environment.

* [Continual Reinforcement Learning by Planning with Online World Models](https://openreview.net/forum?id=mQeZEsdODh) (ICML 2025)

> This paper learns an online world model and act by planning via model prediction control to construct a unified world dynamics to handle the catastrophic forgetting issue. An online agent is also developed to evaluate on a proposed continual bench environment.

* [Mitigating Plasticity Loss in Continual Reinforcement Learning by Reducing Churn](https://openreview.net/forum?id=EkoFXfSauv) (ICML 2025)

> This paper follows Fast TRAC (NeurIPS 2024), focusing on plasticity loss with mostly same experimental settup: gym control, procgen, and MinAtar. The novelty of this paper is that it establishes the connection between plasticity and the churn via NTK matrix. 


* [Position: Lifetime tuning is incompatible with continual reinforcement learning](https://openreview.net/pdf?id=JMoWFkwnvv) (ICML 2025)

> This position paper emphasizes the importance of evaluation of the algorithm's performance in the context of continual RL. They propose k-percent turning to promote a fairer evaluation, called lifetime tuning.

* [Prevalence of Negative Transfer in Continual Reinforcement Learning: Analyses and a Simple Baseline](https://openreview.net/forum?id=KAIqwkB3dT) (ICLR 2025)
> This paper highlights the prevalence of negative transfer within the loss of plasticity (even for fine-tune algorithms without considering the catastrophic forgetting) through extensive experiments on Metaworld, DMC control, and Atar games. To address this issue, the dual actor networks are used, with one periodically resetting the learn the current task, and the other distilling all knowledge from the large replay buffer via behavior cloning.

## 2024





* [Fast TRAC: A Parameter-Free Optimizer for Lifelong Reinforcement Learning](https://openreview.net/pdf?id=QEaHE4TUgc) (NeurIPS 2024)
> The authors bring the idea from parameter-free online convex optimization to design a new advanced optimizer (based on SGD, Adam) to address the loss of plasiticity issue in continual RL. Experiments include Procgen, Atari, and Gym Control environments, which are more flexible.


* [Parseval Regularization for Continual Reinforcement Learning](https://openreview.net/pdf?id=RB1F2h5YEx) (NeurIPS 2024)
> This paper focuses on the loss of plasticity of continual RL from the perspective of optimization, one of the important aspects of continual RL. The authors propose to use Parseval regularization, which maintains orthogonality of weight matrix and thus enhances the optimization in the presence of new tasks.



* [Self-composing policies for scalable continual RL](https://github.com/mikelma/componet) (ICML 2024)
> Like PackNet, this paper designs a growing NN that uses the attention module to integrate the output from previous policies and the current policy. The growing NN is thus deployed for the new task and empirically achieves great performance in terms of bot plasticity (forward transfer and learning curve) and catastrophic forgetting (average performance) in Metaworld and Atari games.





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
> The paper proposes sparse prompting to address continual RL problems, which learns overcomplete dictionaries to produce sparse masks as prompts, extracting a sub-network for each task from a meta-policy network.


* [Task-Agnostic Continual Reinforcement Learning: Gaining Insights and Overcoming Challenges](https://arxiv.org/abs/2205.14495) (CoLLAs 2023)
> The paper considers continual RL from the perspective of POMDP, and it also involves some insightful discussions.

* [Loss of Plasticity in Continual Deep Reinforcement Learning](https://proceedings.mlr.press/v232/abbas23a/abbas23a.pdf) (CoLLAs 2023)
> This paper studies the continual learning of value-based RL in Atari games, (1) standard setting: 10 games * 20M * repeat 5times (2) milder setting: mode change within one game. Then they find the loss of plasticity and the catastrophic interference often occur with the weight diminishing. Therefore, they propose to use concatenated ReLu (ReLu(x), ReLu(-x)) to help propagate the gradient to reduce the loss of plasticity.


## 2022 and Before 



* [CoMPS: Continual Meta Policy Search](https://arxiv.org/pdf/2112.04467) (ICLR 2022)
> This paper studies continual RL from the perspective of meta-learning.


* [Lifelong Robotic Reinforcement Learning by Retaining Experiences](https://proceedings.mlr.press/v199/xie22a/xie22a.pdf) (CoLLAs 2022)
> As an early attempt, this paper focuses on the loss of plasticity only while assuming the previous data are stored and the previous reward functions are given. However, the interesting idea is that the importance weight is introduced, estimated by a learned classifier and in the progressively increasing replay buffer. Experiments are on a suite of simulated robotics environments.



* [Disentangling Transfer in Continual Reinforcement Learning](https://arxiv.org/abs/2209.13900) (NeurIPS 2022)
> This paper empirically investigates the impact of different components in SAC on continual RL, and proposes the behavior cloning method to combine improvements.

* [Towards Evaluating Adaptivity of Model-Based Reinforcement Learning Methods](https://arxiv.org/pdf/2204.11464) (ICML 2022)
> This paper investigates the adaptive power of model-based RL to local reward changes and reveals 4 failure modes. It finds that a large replay buffer from old data hurts the adaptivity/plasticity, while a small one tends to lead to catastraphic forgetting, suggesting a trade-off between them to achieve more ambitious continual RL problems.

* [Continual World: A Robotic Benchmark For Continual Reinforcement Learning](https://arxiv.org/abs/2105.10919) (NeurIPS 2021)
> Benchmark: Continual World, 10 manipulation tasks from MetaWorld

* [Towards Continual Reinforcement Learning: A Review and Perspectives](https://arxiv.org/abs/2105.10919) (Journal of Artificial Intelligence Research (JAIR)) 2020
> The first review of continual RL, however, most of the related papers are about continual learning instead of RL.

* [Policy Consolidation for Continual Reinforcement Learning](https://arxiv.org/abs/1902.00255) (ICML 2019）
> The authors proposed to use the policy consolidation method, in which the policy network interacts with a series of hidden networks in different time-scales to mitigate catastrophic forgetting.

* [Continual Reinforcement Learning with Complex Synapses](https://arxiv.org/abs/1802.07239) (ICML 2018)
> This paper incorporates a synaptic model in RL agents to mitigate catastrophic forgetting in continual RL. This study is inspired by neuroscience, but its experiments are restricted on tabular experiments.

* [State Abstractions for Lifelong Reinforcement Learning](https://proceedings.mlr.press/v80/abel18a/abel18a.pdf) (ICML 2018)
> This paper brings state abstraction to lifelong RL and provides a theoretical analysis.



**Remark**. There are also a few papers before 2022 collected in https://github.com/ContinualAI/continual-learning-papers#continual-reinforcement-learning.

