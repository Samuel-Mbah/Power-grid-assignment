# Grid2Op Reinforcement Learning Agents: DQN and Successive Representation

This project explores reinforcement learning techniques applied to power grid management using the Grid2Op environment. The agents are trained to ensure the stability and reliability of a power grid by optimizing both `L2RPNReward` and `N1Reward`. Two algorithms are implemented and iteratively improved:
- **Deep Q-Network (DQN)**
- **Successive Representation Agent**

## Project Overview

The goal of this project is to develop, evaluate, and iteratively improve reinforcement learning agents for the task of power grid management. The focus is on the reliability of electricity flow across the network, with the ability to withstand individual component failures (N-1 reliability). 

## Installation

### Requirements

- Python 3.8 or above
- `gymnasium`
- `Grid2Op` library
- `Stable-Baselines3` (optional, if using for comparison purposes)
- `matplotlib` for visualizations
- `PyTorch` for DQN implementation
- `lightsim2grid` for backend simulation

### Steps to Install

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-repo-url.git]
    cd [your-repo-url](https://github.com/Samuel-Mbah/Power-grid-assignment.git)
    ```

2. **Set up a virtual environment (optional but recommended):**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up the Grid2Op environment:**
    Follow the installation instructions on the [Grid2Op Documentation](https://grid2op.readthedocs.io/en/latest/).

5. **Install LightSim2Grid:**
    ```bash
    pip install lightsim2grid
    ```

## Directory Structure

```markdown
├── main/                                 # Main codebase and baseline files
│   ├── Baseline.ipynb                    # Baseline implementation notebook
│   ├── baseline.zip                      # Compressed baseline agent files
│   ├── CombinedScaledRewards.png         # Reward plot for baseline agent
│
├── DQN-with-new-exploration-strategy/    # Experiment with new exploration strategy (Boltzmann)
│   ├── boltzmann_strategy.ipynb          # Notebook implementing Boltzmann exploration
│   ├── dqn_boltzmann_agent.zip           # Compressed files for the Boltzmann DQN agent
│   ├── CombinedRewards.png               # Reward plot for Boltzmann exploration DQN
│
├── DQN-with-UCB/                         # Experiment with Upper Confidence Bound (UCB)
│   ├── dqn_ucb.ipynb                     # Notebook implementing UCB strategy
│   ├── ucb_dqn_agent.zip                 # Compressed files for the UCB DQN agent
│   ├── CombinedScaledRewards.png         # Reward plot for UCB DQN
│
├── Reward-Shaping/                       # Experiment with reward shaping for DQN
│   ├── reward_shaping.ipynb              # Notebook with reward shaping strategy
│   ├── dqn_grid2op_agent.zip             # Compressed files for reward-shaped DQN agent
│   ├── CombinedScaledRewards.png         # Reward plot for reward-shaped DQN
│
├── DQN-with-Seeds-for-reproducibility/   # Experiment with seed-based reproducibility
│   ├── DQN_seeds.ipynb                   # Notebook setting seeds for reproducibility
│   ├── dqn_grid2op_agent.zip             # Compressed files for reproducible DQN agent
│   ├── CombinedScaledRewards.png         # Reward plot for reproducible DQN
│
├── minimize-observations/                # Experiment minimizing observation space
│   ├── Grid_op_assignment.ipynb          # Notebook for observation space reduction
│   ├── dqn_grid2op_agent.zip             # Compressed files for minimized observation DQN agent
│   ├── CombinedScaledRewards.png         # Reward plot for minimized observation DQN
│
├── Successive-Representation/            # Successive Representation agent implementation
│   ├── SR_baseline.ipynb                 # Baseline implementation of SR agent
│   ├── final-sr-w-o-hyperparameters.ipynb# Final SR agent without hyperparameter tuning
│
├── Final-code/                           # Final selected code and models
│   ├── final_dqn_agent.ipynb             # Notebook for final DQN agent
│   ├── dqn_grid2op_agent.zip             # Compressed final DQN agent files
│   ├── dqn_boltzmann_agent.zip           # Compressed final Boltzmann exploration DQN agent
│
├── README.md                             # Project README file
├── requirements.txt                      # Python dependencies

```

## Experimentation & Improvements
This repository contains different branches for various improvements and experiments conducted during the project:

- `main`: The main branch with the core implementations.
- `DQN-with-new-exploration-strategy`: Implements a new exploration strategy (Boltzmann) for the DQN agent.
- `DQN-with-UCB`: A variant of DQN with Upper Confidence Bound (UCB) for enhanced exploration.
- `Reward-Shaping`: Custom reward shaping is introduced to guide DQN behaviour.
- `DQN-with-Seeds-for-reproducibility`: Adds seeds for reproducibility in DQN experiments.
- `minimize-observations`: Reduces the observation space to critical features for efficiency.
- `Successive-Representation`: Contains experiments with a successive representation approach.



## Version Control
This project uses Git for version control, with multiple branches for different features and experiments. Use the following commands to check the available branches and switch between them:

1. **List all branches:**
    ```bash
    git branch -a
    ```
2. **Switch to a specific branch:**
    ```bash
    git checkout <branch-name>
    ```


