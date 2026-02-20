# LAB 2B — Reinforcement Learning with CartPole

This lab explores reinforcement learning algorithms in a classic control setting
using the CartPole environment. The objective is to compare tabular and deep
reinforcement learning approaches and analyze learning stability.

Two methods are implemented:
1. Tabular Q-learning with discretized state space
2. Deep Q-Network (DQN) using neural network function approximation

The lab emphasizes correct algorithmic implementation, reproducibility, and
learning behavior analysis rather than exhaustive hyperparameter tuning.

---

## Environment
- Environment: CartPole-v1
- Framework: Gymnasium
- Action space: Discrete (left / right)
- State space: Continuous (4-dimensional)

---

## Methods
- **Tabular Q-learning**
  - Coarse discretization of continuous state space
  - ε-greedy exploration
- **Deep Q-Network (DQN)**
  - Neural network function approximation
  - Experience replay
  - Target network for stabilization

---

## Results
- Tabular Q-learning shows gradual learning but unstable and capped performance
- DQN learns faster, achieves higher rewards, and generalizes better
- Training instability is observed and analyzed

---

## Reproducibility
- All random seeds fixed
- Models trained from scratch in notebook
- Learned Q-table and DQN weights saved for reference

---

