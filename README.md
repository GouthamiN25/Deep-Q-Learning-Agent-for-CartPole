# Deep Q-Learning Agent for CartPole

This project demonstrates how to train a reinforcement learning agent using **Deep Q-Learning (DQN)** to solve the classic control problem **CartPole-v1** from OpenAI Gym. The agent learns to balance a pole on a moving cart using trial and error.

## Project Goal

Train an agent that learns the optimal policy to keep the pole balanced for as long as possible by interacting with the environment and improving over time using neural network approximations of Q-values.

## Key Features

-  Uses **Deep Q-Network (DQN)** with PyTorch
-  Implements **experience replay** using Python `deque`
-  Utilizes **ε-greedy policy** for exploration/exploitation
-  Tracks agent performance with reward curves
-  Includes model training and evaluation pipeline

## Technologies Used

- Python
- OpenAI Gym
- PyTorch
- NumPy
- Matplotlib

## How It Works

1. Initialize environment and model
2. For each step:
   - Choose action using ε-greedy strategy
   - Execute action in the environment
   - Store experience in replay buffer
   - Train the DQN using random samples from memory
3. Plot rewards to visualize learning progress

## Results

The agent gradually learns to improve its performance over episodes. A well-trained agent should consistently achieve near the maximum reward of 500 per episode.

## 📂 Project Structure

```
CartPole_RL_Project.ipynb     # Main notebook with code and results
README.md                     # This file
```

## Getting Started

Install required packages:
```bash
pip install gym numpy matplotlib torch
```

Run the notebook in Jupyter or Google Colab.
