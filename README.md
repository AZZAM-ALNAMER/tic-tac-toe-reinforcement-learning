# Tic-Tac-Toe Deep Q-Learning From Scratch

## Project Overview
This project implements a **Deep Q-Network (DQN)** agent from scratch to learn optimal strategies for playing **Tic-Tac-Toe**. The goal is to demonstrate a first-principles understanding of **Reinforcement Learning (RL)** and **Neural Networks**, without relying on high-level machine learning frameworks.

The project was deliberately chosen because Tic-Tac-Toe provides a simple yet well-defined environment that allows full control over the learning process while still requiring key RL concepts such as value approximation, exploration–exploitation tradeoff, and temporal-difference learning.

---

## Why Tic-Tac-Toe?
Tic-Tac-Toe offers an ideal environment to:
- Implement reinforcement learning from scratch
- Understand how agents learn from interaction rather than labeled data
- Apply forward and backward propagation manually
- Study value-based learning in a controlled setting

This aligns with the objective of deeply understanding how learning emerges through gradient-based updates driven by environment interaction.

---

## Problem Definition
- **Task Type:** Reinforcement Learning (Value-Based)
- **Algorithm:** Deep Q-Network (DQN)
- **State Space:** Tic-Tac-Toe board (9-dimensional vector)
- **Action Space:** 9 possible board positions
- **Reward Signal:**
  - Win: +1.0  
  - Loss: −1.0  
  - Draw: +0.5  
  - Non-terminal step: 0.0  

---

## System Pipeline
The complete pipeline is implemented in **pure Python**, using:
- NumPy for numerical computation
- random for stochastic exploration
- matplotlib for training visualization

No external ML libraries (e.g., TensorFlow or PyTorch) are used.

The pipeline consists of:
1. Environment definition
2. Neural network architecture
3. Forward and backward propagation
4. Experience replay buffer
5. Target network
6. Training loop
7. Evaluation and visualization

---

## Environment Design
- Board represented as a 1D array of length 9
- State encoding:
  - `+1` → agent move (X)
  - `-1` → opponent move (O)
  - `0` → empty cell
- Legal actions dynamically determined
- Terminal states: win, loss, draw

---

## Neural Network Architecture
A Multi-Layer Perceptron (MLP) approximates the Q-function:

## 🎥 Project Demo
A full video demonstration of the training process and agent behavior is available here:  
👉 [Watch the demo on YouTube](
https://www.youtube.com/watch?v=UQ8TXct-5ko)


