
# Optimal Energy System Scheduling Using A Constraint-Aware Reinforcement Learning Algorithm

This code accompanies the paper Hou Shengren, Pedro P. Vergara, Edgar Mauricio Salazar Duque, Peter Palensky, "Optimal energy system scheduling using a constraint-aware reinforcement learning algorithm", International Journal of Electrical Power & Energy Systems,
Volume 152, 2023, 109230, ISSN 0142-0615, https://doi.org/10.1016/j.ijepes.2023.109230.

# Abstract 
The massive integration of renewable-based distributed energy resources (DERs) inherently increases the energy system's complexity, especially when it comes to defining its operational schedule. Deep reinforcement learning (DRL) algorithms arise as a promising solution due to their data-driven and model-free features. However, current DRL algorithms fail to enforce rigorous operational constraints (e.g., power balance, ramping up or down constraints) limiting their implementation in real systems. To overcome this, in this paper, a DRL algorithm (namely MIP-DQN) is proposed, capable of \textit{strictly} enforcing all operational constraints in the action space, ensuring the feasibility of the defined schedule in real-time operation. This is done by leveraging recent optimization advances for deep neural networks (DNNs) that allow their representation as a MIP formulation, enabling further consideration of any action space constraints. Comprehensive numerical simulations show that the proposed algorithm outperforms existing state-of-the-art DRL algorithms, obtaining a lower error when compared with the optimal global solution (upper boundary) obtained after solving a mathematical programming formulation with perfect forecast information; while strictly enforcing all operational constraints (even in unseen test days).

# Organization
* Folder "Data" -- Historical and processed data.
* script "Parameters"-- General parameters for batteries and other energy units.
* script "MIP_DQN"-- The implementation of the proposed MIP-DQN algorithm.
* script "random_generator_battery" -- The energy system environment
* script "random_generator_more_battery" -- The energy system environment with multi-batteries. 
* Run scripts after installing all packages. 

# Dependencies
This code requires installation of the following libraries: ```PYOMO```,```pandas 1.1.4```, ```numpy 1.20.1```, ```matplotlib 3.3.4```, ```pytorch 1.11.0```,  ```OMLT```,```wandb```. I used wandb to monitor the changes during the training. you can find more information [at this page](https://arxiv.org/abs/2305.05484).

# Recommended citation
Hou Shengren, Pedro P. Vergara, Edgar Mauricio Salazar Duque, Peter Palensky, "Optimal energy system scheduling using a constraint-aware reinforcement learning algorithm", International Journal of Electrical Power & Energy Systems,
Volume 152, 2023, 109230, ISSN 0142-0615, https://doi.org/10.1016/j.ijepes.2023.109230.

A preprint is available, and you can check this paper for more details  [Link of the paper](https://arxiv.org/abs/2305.05484).
