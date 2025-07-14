# Q-Learning on FrozenLake (Reinforcement Learning)

This notebook implements **Q-learning**, a foundational reinforcement learning algorithm, to solve the **FrozenLake** environment from OpenAI Gym. The agent learns how to navigate a slippery 4×4 grid from a start point to a goal while avoiding holes.

---

## 🤖 What is Reinforcement Learning?

Reinforcement Learning (RL) is an area of machine learning where an agent learns to make decisions by interacting with an environment. It receives feedback in the form of **rewards** and uses this to learn an optimal **policy** — a mapping from states to actions.

Key Concepts:
- **Agent**: The learner or decision-maker
- **Environment**: Where the agent operates (FrozenLake in this case)
- **State**: Current position of the agent
- **Action**: Move left, right, up, or down
- **Reward**: Feedback from the environment (1 for reaching the goal, 0 or -1 otherwise)
- **Q-table**: A lookup table the agent builds to estimate the value of state-action pairs

---

## ❄️ Environment: FrozenLake-v1

- Grid-based 4×4 map with four possible actions: {Left, Down, Right, Up}
- Goal: Reach the terminal state safely
- Challenges: Slippery surface causes stochastic transitions
- Termination: Reaching the goal (success) or falling into a hole (failure)

---

## 🧠 Algorithm: Q-Learning

Q-Learning is a model-free RL algorithm that estimates the **optimal action-value function (Q*)** using the Bellman equation. The agent updates its Q-table as it explores.

### Q-Update Rule:

Q(s, a) ← Q(s, a) + α * [r + γ * max(Q(s’, a’)) - Q(s, a)]

- **α**: Learning rate
- **γ**: Discount factor
- **r**: Immediate reward
- **s'**: Next state

The agent uses an **ε-greedy policy** during training to balance exploration (trying new actions) and exploitation (using known good actions).

---

## 📈 What the Notebook Does

- Initializes Q-table for all state-action pairs
- Trains the agent over thousands of episodes
- Tracks reward trends and success rate
- Plots performance metrics (e.g., reward vs. episodes)
- Demonstrates learned policy on test runs

---

## 🛠 Requirements

To run the notebook, install:

```bash
pip install gym numpy matplotlib

