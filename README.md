# Reinforcement Learning for Kaggle ConnectX Challenge

**Python, PyTorch, Reinforcement Learning (DQN, DDQN, A2C)**

## Introduction

This project implements reinforcement learning agents for the Kaggle ConnectX competition using Deep Q-Learning (DQN), Double DQN (DDQN), and Actor-Critic (A2C) methods. The goal is to build an agent that learns optimal strategies for playing ConnectX by interacting with the environment.

## Project Overview

The project includes the implementation of three major RL algorithms for solving ConnectX:

- **Deep Q-Learning (DQN)**
- **Double DQN (DDQN)**
- **Actor-Critic (A2C)**

These models are compared based on their performance in terms of win rates and training efficiency.

## Key Features

- **Modeling Different Architectures**: Implementing DQN, DDQN, and Actor-Critic methods to compare effectiveness.
- **Replay Buffer**: Storing and sampling experiences to improve learning stability.
- **Action Selection**: Using Epsilon-Greedy for balancing exploration and exploitation.
- **Training & Evaluation**: Training agents and evaluating their performance against a random opponent.
- **Model Comparison**: Comparing DQN, DDQN, and A2C based on win rates.
- **Hyperparameter Tuning**: Experimenting with different hyperparameters for optimal performance.

## Why I Chose DQN, DDQN, and A2C

- **DQN**: A classic deep reinforcement learning model that learns a policy using a neural network to approximate the Q-value function. This provides a simple and effective method for solving ConnectX.
- **DDQN**: An improvement over DQN, designed to address Q-value overestimation by using a target network. It helps stabilize training and enhances performance.
- **A2C**: An extension of the Actor-Critic method that uses two networks: an Actor to select actions and a Critic to evaluate them. This method ensures better stability and faster convergence.

## Summary Report

The goal of this project was to create a reinforcement learning agent capable of playing ConnectX. We leveraged DQN, DDQN, and A2C models to build a competitive agent and achieved promising results.

### Key Components:

- **DQN and DDQN**: 
  - DQN used a fully connected neural network with ReLU activation to approximate Q-values.
  - DDQN improved upon DQN by separating action selection and Q-value estimation with a target network, reducing overestimation bias.
  
- **Actor-Critic (A2C)**:
  - A2C used two networks (Actor and Critic) to select actions and evaluate the current state, optimizing both networks using the advantage function.

- **Experience Replay**: 
  - A replay buffer was used to store state-action-reward-next state transitions, enabling the agent to learn from a diverse set of experiences.

- **Epsilon-Greedy Strategy**:
  - The agent used epsilon-greedy for action selection, initially exploring random actions and gradually exploiting learned strategies.

- **Training & Evaluation**:
  - Models were trained for 1,000 episodes. Evaluation showed a win rate of 86.4% for the A2C model against random opponents.
  
- **Hyperparameter Tuning**:
  - Hyperparameters like learning rate, epsilon decay, and batch size were tuned to optimize performance.

## Conclusion

This project successfully demonstrated the effectiveness of A2C, DQN, and DDQN in solving the ConnectX challenge. The results showed that A2C performed best, achieving a win rate of 86.4%, followed by DQN/DDQN with a win rate of 77.2%.

## Future Work

- Explore advanced RL techniques like Proximal Policy Optimization (PPO).
- Further optimize hyperparameters for better stability and performance.
- Test the agent against more sophisticated models to further improve its strategy.
