# Experiment Log — LAB 2B (Reinforcement Learning)

This document tracks experimental configurations and observations for the
CartPole reinforcement learning task.

---

## Experiment 1 — Tabular Q-Learning
- Algorithm: Q-learning with discretized state space
- Discretization: 6 bins per state dimension
- Exploration: ε-greedy with decay
- Episodes: 500
- Observations:
  - Gradual increase in reward
  - High variance across episodes
  - Performance plateaus at moderate reward values

---

## Experiment 2 — Deep Q-Network (DQN)
- Algorithm: DQN with MLP function approximation
- Network: 2 hidden layers (128 units each)
- Replay buffer: Enabled
- Target network: Periodically updated
- Episodes: 600
- Observations:
  - Faster learning than tabular method
  - Achieves near-maximum rewards
  - Intermittent instability and reward drops observed

---

## Final Notes
- DQN significantly outperforms tabular Q-learning
- Instability is expected due to function approximation and bootstrapping
- Results are consistent with standard RL behavior on CartPole