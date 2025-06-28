# snake-rl-agent
A Deep Q-Learning agent trained to play the classic Snake game using PyTorch and Pygame. This project demonstrates fundamental reinforcement learning concepts including experience replay, epsilon-greedy strategy, and Q-value updates using a simple feedforward neural network.

# Snake Game AI using Deep Q-Learning

This project demonstrates how to train an artificial agent to play the classic Snake game using **Deep Q-Learning (DQN)**, a reinforcement learning algorithm. The agent learns to survive and grow longer by eating food while avoiding collisions.

---

## 📌 Features

- ✅ Trains a neural network to play Snake using PyTorch
- ✅ Uses Deep Q-Learning (DQN) with experience replay
- ✅ Epsilon-greedy strategy for exploration vs. exploitation
- ✅ Saves and loads trained models
- ✅ Play mode to watch the trained agent in action
- ✅ Visual training performance plot using `matplotlib`

---

## 🧠 Algorithm: Deep Q-Learning

This project implements a **value-based, off-policy** reinforcement learning algorithm called **DQN**:

- **State Space**: 11 features (danger ahead, direction, food location)
- **Action Space**: `[Straight, Right Turn, Left Turn]`
- **Reward Function**:
  - `+10` for eating food 🍎
  - `-10` for dying ☠️
  - `0` for a regular move (or small penalty if you add one)
- **Learning Method**:
  - Neural network estimates `Q(state, action)`
  - Experience replay using a memory buffer
  - Bellman equation for Q-value updates
