# 🐍 Snake Game AI — Reinforcement Learning Agent

> A Deep Reinforcement Learning-powered Snake Game built using Python and PyTorch. This project compares multiple RL algorithms (DQN, Double DQN, A2C, Dueling DQN, PPO, and PER) to train an agent that learns to survive and grow in a grid-based Snake environment.

<p align="center">
  <img src="https://img.shields.io/badge/Tech-PyTorch-red" />
  <img src="https://img.shields.io/badge/Model-DQN%2FA2C%2FPPO-green" />
  <img src="https://img.shields.io/badge/Type-Reinforcement_Learning-blue" />
</p>

## 🎥 Demo

Watch the AI in action:  
📺 [Click to Watch Demo Video](https://link-to-demo)

---

## 🚀 Project Overview

This project aims to train an agent to play the classic Snake game using **state-of-the-art reinforcement learning algorithms**. The game is rendered in a grid world where the snake must eat food while avoiding collisions with walls or itself.

### 🎯 Objective:
- Maximize score by consuming food
- Minimize collisions and survive longer
- Evaluate performance across multiple RL algorithms

---

## 🎮 Game Environment

| Feature            | Description                                                              |
|--------------------|--------------------------------------------------------------------------|
| **Grid-Based**     | Snake moves in 4 directions on a grid                                     |
| **State Space**    | Snake head + body, food position, distance to walls & self               |
| **Action Space**   | `['Up', 'Down', 'Left', 'Right']`                                        |
| **Reward System**  | +10 (food), -10 (collision)                                               |

---

## 🧠 Algorithms Used

| Algorithm         | Key Benefits                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **DQN**           | Stable for discrete action spaces                                            |
| **Double DQN**    | Reduces overestimation in Q-values                                           |
| **A2C**           | Actor-Critic structure enables smoother policy learning                     |
| **Dueling DQN**   | Separates value and advantage components for smarter decisions              |
| **PER**           | Prioritizes learning from high-impact experiences                           |
| **PPO**           | Enforces stable updates with clipping for controlled policy improvement     |

---

## 📊 Performance Summary

| Algorithm     | Highest Score | Avg. Lifespan (Steps) | Stability          |
|---------------|---------------|------------------------|--------------------|
| DQN           | 27            | 173                    | Medium (fluctuating)|
| Double DQN    | 28            | 150                    | Better than DQN     |
| A2C           | **70**        | **970**                | Most Stable         |
| Dueling DQN   | ~35           | 264                    | Improving steadily  |
| PER           | ~40           | 264                    | Fast learning phase |
| PPO           | ~20           | 322                    | Least effective     |

---

## 🧪 Installation & Setup

```bash
git clone https://github.com/yourusername/snake-game-ai.git
cd snake-game-ai
pip install -r requirements.txt
python train_dqn.py  # Replace with your script entry point
