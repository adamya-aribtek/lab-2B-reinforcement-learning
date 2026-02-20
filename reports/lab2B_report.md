# LAB 2B Report — Reinforcement Learning with CartPole

## 1. Objective
The objective of this lab is to implement and compare tabular and deep
reinforcement learning methods in a classic control environment. The lab focuses
on learning dynamics, stability, and practical limitations of each approach.

---

## 2. Environment
- Environment: CartPole-v1 (Gymnasium)
- State space: Continuous, 4-dimensional
- Action space: Discrete, 2 actions
- Reward: +1 per timestep until failure

---

## 3. Methods

### Tabular Q-Learning
The continuous state space was discretized into coarse bins to enable tabular
Q-learning. An ε-greedy exploration strategy was used, and Q-values were updated
using the standard Bellman equation.

### Deep Q-Network (DQN)
A DQN was implemented using a neural network to approximate the action–value
function. Experience replay and a target network were employed to improve
training stability.

---

## 4. Results
Tabular Q-learning demonstrated limited performance due to discretization and
lack of generalization. In contrast, the DQN achieved significantly higher
episode rewards and learned a stabilizing policy more efficiently.

---

## 5. Stability and Divergence Analysis
Training instability was observed in the DQN, characterized by sudden drops in
episode reward after high-performing episodes. This behavior arises from the
interaction of function approximation, bootstrapping, non-stationary targets,
and stochastic exploration. Despite this, overall learning trends indicate
successful policy improvement.

---

## 6. Model Artifacts
For reproducibility, the learned Q-table and DQN network weights were saved.
Unlike supervised learning, reinforcement learning does not rely on fixed
datasets; saved artifacts primarily support inspection and reuse rather than
offline evaluation.

---

## 7. Conclusion
This lab demonstrates the limitations of tabular reinforcement learning in
continuous environments and highlights the effectiveness of deep reinforcement
learning methods. While DQN introduces training instability, it provides superior
performance and scalability, making it suitable for more complex control tasks.