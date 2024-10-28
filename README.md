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
├── results/                   # Stores results from the experiments
│   ├── CombineScaledRewards_plots # Plot for CombinedScaledRewards

├── notebooks/                 # Jupyter Notebooks for experiments and visualization
│   ├── dqn_agent.ipynb         # Notebook for analyzing performance
|   ├── dqn_agent.ipynb
|   ├── dqn_agent.ipynb
    ├── dqn_agent.ipynb
    ├── dqn_agent.ipynb 
│
├── README.md                  # This file
├── requirements.txt           # Python dependencies
