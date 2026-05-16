# 📢 Awesome Continual Reinforcement Learning (CRL) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)



This repository collects important papers in the field of **Continual Reinforcement Learning (CRL)** and **Lifelong Reinforcement Learning (LRL)**, aiming to provide a comprehensive and up-to-date resource for researchers. The goal of CRL is to enable autonomous agents to learn sequentially across multiple tasks or in **non-stationary environments** while accumulating knowledge, mitigating **catastrophic forgetting**, and preventing **loss of plasticity.**

**Contributions and suggestions for missing important works are always welcome.**



## 🤝 Contributing
We aim to keep this repository up-to-date with the latest research on CRL and LRL. We are continuously improving and expanding this repository to make it a more comprehensive and well-organized resource for the Continual and Lifelong RL community.

Feel free to contribute either with a PR or by opening an issue.

- [📢 Awesome Continual Reinforcement Learning (CRL) ](#-awesome-continual-reinforcement-learning-crl-)
  - [🤝 Contributing](#-contributing)
  - [📝 Survey](#-survey)
  - [📖 Research Papers](#-research-papers)
    - [2026](#2026)
    - [2025](#2025)
    - [2024](#2024)
    - [2023](#2023)
    - [2022](#2022)
    - [2021](#2021)
    - [2019](#2019)
    - [2018](#2018)
    - [arXiv](#arxiv)
  - [🌎 Benchmarks](#-benchmarks)
  - [🔗 Related Repositories](#-related-repositories)


## 📝 Survey
- Mai Z, Jeon S, Huang Z, et al. **A Survey of Continual Learning for Robotics in the Foundation Model Era**[J].[[Paper]](https://www.techrxiv.org/doi/full/10.36227/techrxiv.176972367.76460794/v3)[[Code]](https://github.com/OSU-MLB/awesome-continual-learning-robotics-embodied-ai)

    >TL;DR: This survey provides unified task formulations across Continual manipulation, navigation, and planning in the foundation model era. It summarizes widely used benchmarks and organizes existing methods into a technique taxonomy spanning architecture- replay-, and optimization-based methods. I believe that CRL represents a highly significant scenario within the field of robotics.

- Zuffer A, Burke M, Harandi M. **Advancements and Challenges in Continual Reinforcement Learning: A Comprehensive Review**[J]. arXiv preprint arXiv:2506.21899, 2025.[[Paper]](https://arxiv.org/abs/2506.21899)

    >TL;DR: This paper serves as a comprehensive and systematic survey about CL and CRL. While it offers a solid and accessible entry point for newcomers to the field, the classification of CRL approaches is relatively limited and does not cover some of the most recent advancements. 


- Pan C, Yang X, Li Y, et al. **A Survey of Continual Reinforcement Learning**[J]. arXiv preprint arXiv:2506.21872, 2025.[[Paper]](https://arxiv.org/abs/2506.21872)

    >TL;DR: This paper provides an up-to-date and comprehensive survey of CRL. It introduces a new taxonomy that categorizes methods into four types: policy-focused, experience-focused, dynamics-focused, and reward-focused, from the perspective of knowledge storage and transfer.  


- Khetarpal K, Riemer M, Rish I, et al. **Towards continual reinforcement learning: A review and perspectives**[J]. Journal of Artificial Intelligence Research, 2022, 75: 1401-1476.[[Paper]](https://arxiv.org/abs/2012.13490)


- Klein T, Miklautz L, Sidak K, et al. **Plasticity loss in deep reinforcement learning: A survey**[J]. arXiv preprint arXiv:2411.04832, 2024.[[Paper]](https://arxiv.org/abs/2411.04832)[[Code]](https://github.com/Probabilistic-and-Interactive-ML/awesome-plasticity-loss)

## 📖 Research Papers

### 2026
#### ICLR 2026
- Sun K, Zhang H, Jin J, et al. **Principled Fast and Meta Knowledge Learners for Continual Reinforcement Learning**[J]. 2025.[[Paper]](https://arxiv.org/abs/2603.00903)[[Code]](https://github.com/datake/FAME)

    >TL;DR: This paper proposes FAME, a dual-learner framework where a fast learner adapts to new tasks and a meta learner incrementally consolidates past knowledge. Using principled measures of MDP difference and forgetting, FAME enables adaptive knowledge transfer and stable integration, improving forward transfer and reducing catastrophic forgetting in CRL.

- Wu Z, Tang H, Ma Y, et al. **The Rank and Gradient Lost in Non-stationarity: Sample Weight Decay for Mitigating Plasticity Loss in Reinforcement Learning**[J]. arXiv preprint arXiv:2604.01913, 2026.[[Paper]](https://arxiv.org/abs/2604.01913)[[Code]](https://github.com/wzhhasadream/CleanRL-JAX)

    >TL;DR: This paper identifies $\theta(1/k)$ gradient magnitude decay as a primary theoretical driver of plasticity loss in non-stationary RL. To address this, the authors propose Sample Weight Decay (SWD), a lightweight experience replay strategy that prioritizes recent data to restore gradient signals, effectively mitigating plasticity loss and improving learning stability across various RL benchmarks.

- Han I, Park S, Oh S, et al. **FIRE: Frobenius-Isometry Reinitialization for Balancing the Stability-Plasticity Tradeoff** (Oral)[J]. arXiv preprint arXiv:2602.08040, 2026.[[Paper]](https://openreview.net/forum?id=CfZLxT3zIZ)[[Code]](https://isaac7778.github.io/fire/) 

    >TL;DR: FIRE optimizes the stability–plasticity tradeoff by framing reinitialization as a constrained geometric projection. It minimizes the Squared Frobenius Error (to preserve past knowledge) while enforcing Dynamical Isometry (to restore learning capacity). This principled reinitialization, efficiently implemented via Newton–Schulz iteration, consistently outperforms standard reset methods across computer vision, language modeling, and reinforcement learning. 

### 2025
#### RLC 2025
- Elelimy E, Szepesvari D, White M, et al. **Rethinking the foundations for continual reinforcement learning**[J]. arXiv preprint arXiv:2504.08161, 2025.[[Paper]](https://arxiv.org/abs/2504.08161)

    >TL;DR: This paper argues that key assumptions of standard RL, such as MDP formulations, optimal policy focus, and episodic evaluation, are misaligned with the goals of CRL. It proposes a new paradigm tailored to CRL based on the history process, providing a more appropriate foundation for lifelong learning. 


#### ICML 2025
- Liu Z, Fu G, Du C, et al. **Continual Reinforcement Learning by Planning with Online World Models** (Spotlight)[J]. arXiv preprint arXiv:2507.09177, 2025.[[Paper]](https://icml.cc/virtual/2025/poster/44151)

    >TL;DR: This paper shows that CRL should learn a unified dynamics rather than training policies. It introduces an Online Agent (OA) that selects actions via MPC with CEM instead of training policies, and plans using a Follow-The-Leader shallow world model that updates incrementally with no-regret guarantees against forgetting. Evaluation is performed on their custom-designed Continual Bench.

- Sun Y, Fu H, Littman M, et al. **Knowledge Retention for Continual Model-Based Reinforcement Learning**[J]. arXiv preprint arXiv:2503.04256, 2025.[[Paper]](https://arxiv.org/abs/2503.04256)[[Code]](https://github.com/YixiangSun/drago)

     >TL;DR: This paper introduces DRAGO, a model-based CRL framework built upon the TDMPC method. It aims to preserve dynamics knowledge across sequential tasks without storing past data. DRAGO achieves this by generating synthetic experiences from previous tasks and employing an intrinsic reward to guide exploration towards revisiting familiar states, thereby mitigating catastrophic forgetting and promoting effective knowledge transfer.   

- Tang H, Obando-Ceron J, Castro P S, et al. **Mitigating Plasticity Loss in Continual Reinforcement Learning by Reducing Churn**[J]. arXiv preprint arXiv:2506.00592, 2025.[[Paper]](https://arxiv.org/abs/2506.00592)[[Code]](https://github.com/bluecontra/C-CHAIN)

    >TL;DR: This paper links plasticity loss in CRL to increased "churn" (network output variability for out-of-batch data), showing it's exacerbated by Neural Tangent Kernel (NTK) rank decrease. The authors propose C-CHAIN, a method to reduce churn, which prevents NTK rank collapse and adaptively adjusts gradients. C-CHAIN significantly improves learning performance across diverse benchmarks.

- Mesbahi G, Panahi P M, Mastikhina O, et al. **Position: Lifetime tuning is incompatible with continual reinforcement learning**[C]//Forty-second International Conference on Machine Learning Position Paper Track.[[Paper]](https://openreview.net/forum?id=JMoWFkwnvv)

    >TL;DR: Standard lifetime tuning optimizes hyperparameters by repeatedly evaluating agents over a fixed, known interaction lifetime, which leads to overfitting to this specific lifespan and misleads continual RL evaluation. This paper proposes k percent tuning, which tunes on only a fraction of the agent’s lifetime to more accurately reveal the advantages of true continual learning algorithms.

#### NeurIPS 2025
- Lee D, Lee D, Kwack T Y, et al. **Policy Compatible Skill Incremental Learning via Lazy Learning Interface**(Spotlight)[J]. arXiv preprint arXiv:2509.20612, 2025.[[Paper]](https://arxiv.org/abs/2509.20612)[[Code]](https://github.com/L2dulgi/SIL-C)

    >TL;DR: This paper presents SIL-C, a skill incremental learning framework that resolves evolving skill–policy incompatibility. It uses a bilateral lazy-learning interface that aligns policy subtasks with updated skills via trajectory similarity, enabling backward and forward compatibility without retraining and supporting efficient continual skill expansion.

- Hu J, Lian Z H, Wen Z, et al. **Continual Knowledge Adaptation for Reinforcement Learning**[C]//The Thirty-ninth Annual Conference on Neural Information Processing Systems.[[Paper]](https://openreview.net/forum?id=QRlVickNdN)[[Code]](https://github.com/Fhujinwu/CKA-RL)

    >TL;DR: CKA-RL addresses catastrophic forgetting and scalability in CRL. It uses a dynamic pool of task-specific knowledge vectors to adapt historical knowledge for new tasks, and an adaptive merging mechanism to consolidate similar vectors. This approach significantly improves performance and knowledge transfer.

- Hu J, Huang S, Shen L, et al. **Tackling Continual Offline RL through Selective Weights Activation on Aligned Spaces**[C]//The Thirty-ninth Annual Conference on Neural Information Processing Systems. 2025.[[Paper]](https://openreview.net/forum?id=KfRfTAJpjh)

    >TL;DR: This paper introduces VQ-CD, a continual offline RL method that aligns heterogeneous task spaces with vector quantization and mitigates forgetting through selective weight activation using task masks. By unifying representations and isolating task-specific parameters, it enables robust continual learning across diverse task sequences.



#### ICLR 2025
- Ahn H, Hyeon J, Oh Y, et al. **Prevalence of negative transfer in continual reinforcement learning: Analyses and a simple baseline**[C]//The Thirteenth International Conference on Learning Representations. 2025.[[Paper]](https://openreview.net/forum?id=KAIqwkB3dT)[[Code]](https://github.com/hongjoon0805/Reset-Distill)

    >TL;DR: This paper demonstrates that negative transfer is prevalent in CRL. Reset & Distill (R&D) tackles this with a dual-learner approach: an online network resets its parameters for each new task to eliminate negative transfer and efficiently learn, while an offline network sequentially distills knowledge from the online actor and previous expert policies to prevent catastrophic forgetting.  

- Choi W, Park J, Ahn S, et al. **NeSyC: A Neuro-symbolic Continual Learner For Complex Embodied Tasks In Open Domains**[C]//The Thirteenth International Conference on Learning Representations.[[Paper]](https://openreview.net/forum?id=VoayJihXra)


- Choi J, Seo S W. **Dynamic Contrastive Skill Learning with State-Transition Based Skill Clustering and Dynamic Length Adjustment**[C]//The Thirteenth International Conference on Learning Representations.[[Paper]](https://openreview.net/forum?id=8egnwady4b)

#### ICRA 2025
- Roy K, Dissanayakc A, Tidd B, et al. **M2distill: Multi-modal distillation for lifelong imitation learning**[C]//2025 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2025: 1429-1435.[[Paper]](https://ieeexplore.ieee.org/abstract/document/11128857/)
  
    >TL;DR: This paper proposes a multi-modal distillation-based lifelong imitation learning approach, which imposes constraints on the alterations in latent representations and action distributions. Experimental results on the LIBERO benchmark show superior performance in retaining old skills while learning new tasks.

#### NMI 2025
- Meng Y, Bing Z, Yao X, et al. **Preserving and combining knowledge in robotic lifelong reinforcement learning**[J]. Nature Machine Intelligence, 2025: 1-14.[[Paper]](https://www.nature.com/articles/s42256-025-00983-2)[[Code]](https://github.com/Ghiara/LEGION)

    >TL;DR: This paper presents LEGION, a robotic lifelong reinforcement learning framework that continually preserves and recombines knowledge across tasks. Leveraging a Bayesian non-parametric knowledge space and language embeddings, it integrates an upstream task inference module with a downstream single policy conditioned on latent task representations, enabling efficient transfer and long-horizon task execution.  

### 2024
#### Nature 2024
- Dohare S, Hernandez-Garcia J F, Lan Q, et al. **Loss of plasticity in deep continual learning**[J]. Nature, 2024, 632(8026): 768-774.[[Paper]](https://www.nature.com/articles/s41586-024-07711-7)[[Code]](https://github.com/shibhansh/loss-of-plasticity)

    >TL;DR: This paper systematically demonstrates that both supervised and reinforcement learning methods based on backpropagation suffer from loss of plasticity in continual learning tasks, and proposes Continual Backpropagation, which maintains long-term learning ability by continually and randomly reinitializing a small fraction of less-used units.

#### NeurIPS 2024
- Chung W, Cherif L, Meger D, et al. **Parseval regularization for continual reinforcement learning**[J]. Advances in Neural Information Processing Systems, 2024, 37: 127937-127967.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/e6df4efa20adf8ef9acb80e94072a429-Paper-Conference.pdf)[[Code]](https://github.com/wechu/parseval_reg)

    >TL;DR: This paper introduces Parseval regularization to mitigate plasticity loss in CRL. It adds a term to the objective function to maintain the orthogonality of weight matrices, applied to both the policy and value networks across all layers except the last, thereby preserving optimization properties and improving the agent’s ability to learn new tasks.

- Muppidi A, Zhang Z, Yang H. **Fast trac: A parameter-free optimizer for lifelong reinforcement learning**[J]. Advances in Neural Information Processing Systems, 2024, 37: 51169-51195.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/5b76d77e7095c6480ed827b85f0c2878-Abstract-Conference.html)[[Code]](https://computationalrobotics.seas.harvard.edu/TRAC/)

    >TL;DR: TRAC is a parameter-free optimizer for LRL, derived from Online Convex Optimization. It adaptively regularizes learning by keeping policy weights near a reference point, which can be seen as a parameter-free L2 regularization. This prevents plasticity loss and enables rapid adaptation to new, diverse tasks without any hyperparameter tuning, outperforming baselines across Procgen, Atari, and control tasks.

- Lee D, Yoo M, Kim W K, et al.**Incremental learning of retrievable skills for efficient continual task adaptation**[J]. Advances in Neural Information Processing Systems, 2024, 37: 17286-17312.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/1f0832859514e53a0e4f229fc9b3a4a2-Abstract-Conference.html)[[Code]](https://github.com/L2dulgi/IsCiL)

    >TL;DR: IsCiL introduces an adapter-based Continual Imitation Learning (CiL) framework that enhances knowledge sharing. It achieves this by incrementally learning and retrieving shareable skills through prototype-based memory, enabling sample-efficient and robust task adaptation in non-stationary environments.

#### ICML 2024
- Malagón M, Ceberio J, Lozano J A. **Self-Composing Policies for Scalable Continual Reinforcement Learning**[J].[[Paper]](https://arxiv.org/pdf/2506.14811)[[Code]](https://github.com/mikelma/componet)

    >TL;DR: CompoNet is a modular architecture for CRL that prevents forgetting by freezing past policies and adding new modules. Utilize attention to dynamically combine historical outputs with an internal policy, enabling efficient transfer. Unlike Progressive Networks, CompoNet scales linearly, ensuring superior scalability and speed while maintaining high plasticity.

#### Entropy 2024
- Gai S, Lyu S, **Zhang H, et al. Continual reinforcement learning for quadruped robot locomotion**[J]. Entropy, 2024, 26(1).[[Paper]](https://www.mdpi.com/1099-4300/26/1/93)

    >TL;DR: This paper introduces a CRL approach for quadruped robot to overcome catastrophic forgetting and plasticity loss. It uses a modified Piggyback dynamic network that protects learned parameters and enhances exploration via re-initialization and entropy regularization, outperforming baselines on complex locomotion tasks.  

### 2023
#### ICML 2023
- Sokar G, Agarwal R, Castro P S, et al. **The dormant neuron phenomenon in deep reinforcement learning**[C]//International Conference on Machine Learning. PMLR, 2023: 32145-32168.[[Paper]](https://proceedings.mlr.press/v202/sokar23a/sokar23a.pdf)[[Code]](https://github.com/timoklein/redo)

    >TL;DR: This paper attributes the reduced expressivity of reinforcement learning networks to the dormant neuron phenomenon, showing through extensive experiments that the proportion of inactive neurons increases during training. It introduces ReDo, a simple yet effective method that periodically reinitializes inactive neurons based on their activation statistics to restore network expressivity.

#### ICLR 2023
- Gaya J B, Doan T, Caccia L, et al. **Building a subspace of policies for scalable continual learning**[J]. arXiv preprint arXiv:2211.10445, 2022.[[Paper]](https://arxiv.org/abs/2211.10445)[[Code]](https://github.com/facebookresearch/salina/tree/main/salina_cl)

    >TL;DR: This paper introduces Continual Subspace of Policies (CSP), a scalable continual reinforcement learning method that incrementally builds a subspace of policies to balance performance and model size, achieving sublinear growth, no forgetting, and strong transfer on Brax and Continual World benchmarks.

#### CoLLAs 2023
- Abbas Z, Zhao R, Modayil J, et al. **Loss of plasticity in continual deep reinforcement learning**[C]//Conference on lifelong learning agents. PMLR, 2023: 620-636.[[Paper]](https://proceedings.mlr.press/v232/abbas23a/abbas23a.pdf)[[Code]](https://github.com/timoklein/crelu-pytorch)

    >TL;DR: This paper investigates plasticity loss in CRL by tracking the evolution of weights, gradients, and activations. The authors observe activation collapse, where only a few neurons remain active in non-stationary environments, leading to vanishing gradients and stagnant network weights. Replacing ReLU with CReLU activations mitigates loss of plasticity and sustains learning over time.

- Kessler S, Ostaszewski M, Bortkiewicz M P, et al. **The effectiveness of world models for continual reinforcement learning**[C]//Conference on Lifelong Learning Agents. PMLR, 2023: 184-204.[[Paper]](https://proceedings.mlr.press/v232/kessler23a.html)[[Code]](https://github.com/skezle/continual-dreamer)
    
    >TL;DR: This paper shows the effectiveness of world models in CRL. Continual-Dreamer utilizes reservoir sampling for experience replay, employs world model prediction uncertainty as an intrinsic reward for task-agnostic exploration, mitigating forgetting and enabling transfer, outperforming existing methods.  

### 2022
#### NeurIPS 2022
- Wolczyk M, Zając M, Pascanu R, et al. **Disentangling transfer in continual reinforcement learning**[J]. Advances in Neural Information Processing Systems, 2022, 35: 6304-6317.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/2938ad0434a6506b125d8adaff084a4a-Abstract-Conference.html)
    
    >TL;DR: This paper empirically investigates how SAC components impact transfer in CRL, highlighting the critic's paramount role and providing key design recommendations. Based on experimental observations, it proposes ClonEx-SAC, leveraging behavioral cloning and exploration strategy to significantly boost performance and forward transfer on Continual World.  

- Schöpf P, Auddy S, Hollenstein J, et al. **Hypernetwork-ppo for continual reinforcement learning**[C]//Deep Reinforcement Learning Workshop NeurIPS 2022. 2022.[[Paper]](https://openreview.net/forum?id=s9wY71poI25)

    >TL;DR: This paper proposes HyperNetwork-PPO (HN-PPO), where a shared hypernetwork generates task-specific actor–critic parameters from task embeddings. Regularized hypernetwork updates prevent drastic changes to prior policies, enabling continual adaptation without forgetting.

#### ICLR 2022
- Lyle C, Rowland M, Dabney W. **Understanding and preventing capacity loss in reinforcement learning**[J]. arXiv preprint arXiv:2204.09560, 2022.[[Paper]](https://openreview.net/forum?id=ZkC8wKoLbQ7)[[Code]](https://github.com/timoklein/infer)

    >TL;DR: This paper investigates capacity loss in RL, where networks gradually lose the ability to fit new targets. Using feature rank to quantify representational capacity, the authors propose Initial Feature Regularization (InFeR), which constrains a subspace of features to stay close to initial values, preserving feature rank and mitigating capacity loss across diverse RL settings.  

### 2021
#### ICLR 2021
- Kumar A, Agarwal R, Ghosh D, et al. **Implicit Under-Parameterization Inhibits Data-Efficient Deep Reinforcement Learning**[C]//International Conference on Learning Representations.[[Paper]](https://openreview.net/forum?id=O9bnihsFfXU)[[Code]](https://github.com/timoklein/implicit_underparameterization)

### 2019
#### NeurIPS 2019

- Traoré R, Caselles-Dupré H, Lesort T, et al. **DISCORL: Continual reinforcement learning via policy distillation**[C]//NeurIPS workshop on Deep Reinforcement Learning. 2019.[[Paper]](https://arxiv.org/abs/1907.05855)[[Code]](https://github.com/anonymous-authors-2018/DisCoRL)

    >TL;DR: This paper presents DisCoRL, a CRL framework that combines state representation learning and policy distillation to sequentially learn multiple tasks without catastrophic forgetting or task labels. The method distills previously learned policies into a single network using stored soft-labeled data, enabling a robot to automatically infer and perform all tasks in both simulation and real-world settings.

- Rolnick D, Ahuja A, Schwarz J, et al. **Experience replay for continual learning**[J]. Advances in neural information processing systems, 2019, 32.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2019/hash/fa7cdfad1a5aaf8370ebeda47a1ff1c3-Abstract.html)

    >TL;DR: This paper introduces CLEAR, a simple replay-based method for CRL that mixes on-policy learning from new experience with off-policy learning and behavioral cloning from replay buffers. CLEAR greatly reduces catastrophic forgetting without requiring task labels or complex architectural changes, outperforming methods like EWC and P&C.

### 2018
#### ICML 2018
- Schwarz J, Czarnecki W, Luketina J, et al. **Progress & compress: A scalable framework for continual learning**[C]//International conference on machine learning. PMLR, 2018: 4528-4537.[[Paper]](https://proceedings.mlr.press/v80/schwarz18a.html?ref=https://githubhelp.com)

    >TL;DR: This paper introduces Progress & Compress (P&C), a scalable continual learning framework with online EWC for robust knowledge retention. An active column learns new tasks in the progress phase, while a knowledge base consolidates them via distillation in the compress phase. Experiments on handwritten alphabet classification, Atari, and 3D maze navigation validate the effectiveness of P&C.


### arXiv
- Hu J, Shim J, Tang C, et al. **Simple Recipe Works: Vision-Language-Action Models are Natural Continual Learners with Reinforcement Learning**[J]. arXiv preprint arXiv:2603.11653, 2026.[[Paper]](https://arxiv.org/abs/2603.11653)[[Code]](https://github.com/UT-Austin-RobIn/continual-vla-rl)
  
    >TL;DR: The authors introduce CRL to the VLA domain, employing GRPO and LoRA to attain both stability against forgetting and high adaptation plasticity, while further augmenting the model's zero-shot transferability. Through systematic validation, they demonstrate that such robustness emerges from the synergy between large pre-trained backbones, parameter-efficient fine-tuning, and the stable dynamics of on-policy RL.

- Li Y, He Q, Yuan M, et al. **Continual Policy Distillation from Distributed Reinforcement Learning Teachers**[J]. arXiv preprint arXiv:2601.22475, 2026.[[Paper]](https://arxiv.org/abs/2601.22475)[[Code]](https://github.com/biolbe1230/Continual-Policy-Distillation-from-Distributed-Reinforcement-Learning-Teachers)

    >TL;DR: This paper frames CRL as a continual Multi-Task Distillation problem by distilling distributed single-task experts into an incrementally expanding MoE Transformer. By synergizing Contrastive Task Embeddings, DPP-based Replay, and Parameter Masking, the framework transforms unstable sequential learning into a scalable supervised process, recovering over 85% of expert performance with minimal forgetting.  

- Xue Yang, Michael Schukat, Junlin Lu, et al. **Demonstration-Guided Continual Reinforcement Learning in Dynamic Environments**[J]. arXiv preprint arXiv:2512.18670, 2025.[[Paper]](https://arxiv.org/abs/2512.18670)[[Code]](https://github.com/XueYang0130/DGCRL.git)

    >TL;DR: Unlike traditional CRL where past knowledge indirectly influences optimization, DGCRL uses a self-evolving external demonstration repository to directly guide agent behavior via curriculum learning. This approach, together with an effective actor–critic resetting mechanism, significantly improves performance and knowledge transfer while mitigating forgetting in dynamic environments.

    
- Fernando C, Banarse D, Blundell C, et al. **Pathnet: Evolution channels gradient descent in super neural networks**[J]. arXiv preprint arXiv:1701.08734, 2017.[[Paper]](https://arxiv.org/pdf/1701.08734)

    >TL;DR: PathNet can be viewed as an evolutionary-masked neural network that uses a genetic algorithm to select and train task-specific parameter paths, freezing them afterward to avoid catastrophic forgetting; by reusing high-fitness modules while isolating irrelevant ones, it achieves faster and more reliable transfer than fine-tuning or learning from scratch across both supervised and RL tasks.  

- Rusu A A, Rabinowitz N C, Desjardins G, et al. **Progressive neural networks**[J]. arXiv preprint arXiv:1606.04671, 2016.[[Paper]](https://arxiv.org/abs/1606.04671)
  
    >TL;DR: This paper introduces Progressive Neural Networks, which add a new neural network (a column) for each task and freeze earlier ones to avoid catastrophic forgetting. Lateral connections enable effective feature reuse, and experiments on Atari, Pong variants, and 3D mazes show consistent positive transfer beyond standard finetuning in deep RL.  





## 🌎 Benchmarks
#### arXiv
- Yuan M, Wang Q, Ma G, et al. Plasticine: Accelerating research in plasticity-motivated deep reinforcement learning[J]. arXiv preprint arXiv:2504.17490, 2025.[[Paper]](https://arxiv.org/pdf/2504.17490)[[Code]](https://github.com/RLE-Foundation/Plasticine)

    >TL;DR: Plasticine is the first open-source benchmark for plasticity loss in deep RL, providing a unified framework with 13 mitigation methods, 6 evaluation metrics, and progressive non-stationary environments to accelerate research into lifelong learning agents. 

#### ICML 2025
- Liu Z, Fu G, Du C, et al. **Continual Bench: Continual Reinforcement Learning by Planning with Online World Models** (Spotlight)[J]. arXiv preprint arXiv:2507.09177, 2025.[[Paper]](https://arxiv.org/abs/2507.09177)[[Code]](https://github.com/sail-sg/ContinualBench)

    >TL;DR: Continual Bench is a CRL benchmark with six Meta-World manipulation tasks that share a unified state/action space and identical environment dynamics. Unlike prior benchmarks with unrealistic physics and conflicting task dynamics, it spatially arranges tasks rather than concatenating them temporally, ensuring consistent world dynamics. Task switches are induced solely by reward changes, enabling controlled evaluation of both adaptation and forgetting.

#### NeurIPS 2023
- Liu B, Zhu Y, Gao C, et al. **Libero: Benchmarking knowledge transfer for lifelong robot learning**[J]. Advances in Neural Information Processing Systems, 2023, 36: 44776-44791.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract-Datasets_and_Benchmarks.html)[[Code]](https://libero-project.github.io/)

    >TL;DR: This paper presents LIBERO, a new benchmark for Lifelong Learning in Decision-Making (LLDM) in robot manipulation, comprising 130 multi-modal tasks across four suites. It investigates five major research topics in lifelong learning, focusing on declarative and procedural knowledge transfer across visual, state, and language modalities.  

- Tomilin T, Fang M, Zhang Y, et al. **COOM: A game benchmark for continual reinforcement learning**[J]. Advances in Neural Information Processing Systems, 2023, 36: 67794-67832.[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d61d9f4fe4357296cb658795fd7999f0-Abstract-Datasets_and_Benchmarks.html)[[Code]](https://github.com/hyintell/COOM)

#### CoLLAs 2022
- Powers S, Xing E, Kolve E, et al. **CORA: Benchmarks, baselines, and metrics as a platform for continual reinforcement learning agents**[C]//Conference on Lifelong Learning Agents. PMLR, 2022: 705-743.[[Paper]](https://proceedings.mlr.press/v199/powers22b.html)[[Code]](https://github.com/AGI-Labs/continual_rl)


#### NeurIPS 2021
- Wołczyk M, Zając M, Pascanu R, et al. **Continual world: A robotic benchmark for continual reinforcement learning**[J]. Advances in Neural Information Processing Systems, 2021, 34: 28496-28510.[[Paper]](https://proceedings.neurips.cc/paper/2021/hash/ef8446f35513a8d6aa2308357a268a7e-Abstract.html)[[Code]](https://github.com/awarelab/continual_world)

    >TL;DR: This paper proposes Continual World, a new benchmark for CRL built on Meta-World. It empirically evaluates seven CL methods on Continual World and finds that existing CL methods effectively mitigate forgetting but largely fail to achieve positive forward transfer, reflecting an inefficient utilization of previously learned knowledge.

#### ICML 2020
- Cobbe K, Hesse C, Hilton J, et al. **Procgen:Leveraging procedural generation to benchmark reinforcement learning**[C]//International conference on machine learning. PMLR, 2020: 2048-2056.[[Paper]](https://proceedings.mlr.press/v119/cobbe20a.html)[[Code]](https://github.com/openai/procgen)

#### CoRL 2019
- Yu T, Quillen D, He Z, et al. **Meta-world: A benchmark and evaluation for multi-task and meta reinforcement learning**[C]//Conference on robot learning. PMLR, 2020: 1094-1100. [[Paper]](http://proceedings.mlr.press/v100/yu20a)[[Code]](https://github.com/Farama-Foundation/Metaworld)

     >TL;DR: This paper proposes Meta-World, a benchmark for meta-reinforcement learning and multi-task learning consisting of 50 distinct robotic manipulation tasks. It evaluates seven meta-RL and multi-task learning algorithms, including MTSAC, to assess generalization across diverse tasks. Meta-World has become a widely used benchmark in CRL research.



## 🔗 Related Repositories

| Repository | URL |
|:--------------------------------------|:-------------------------------------------------------------|
| **Papers-Of-Continual-RL** | [Link](https://github.com/datake/Papers-Of-Continual-RL) |
| **Awesome-Robotics-Manipulation** | [Link](https://github.com/BaiShuanghao/Awesome-Robotics-Manipulation/blob/main/contents/bottlenecks.md?tab=readme-ov-file#lifelongcontinualincremental-learning) |
| **Awesome-Continual-Learning** | [Link](https://github.com/lywang3081/Awesome-Continual-Learning) |
| **continual-learning-papers** | [Link](https://github.com/ContinualAI/continual-learning-papers?tab=readme-ov-file#continual-reinforcement-learning) |
| **awesome-plasticity-loss** | [Link](https://github.com/Probabilistic-and-Interactive-ML/awesome-plasticity-loss) |
| **awesome-continual-learning-robotics-embodied-ai** | [Link](https://github.com/OSU-MLB/awesome-continual-learning-robotics-embodied-ai) |


