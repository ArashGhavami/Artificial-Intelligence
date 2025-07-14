# Artificial Intelligence Projects

This repository contains a collection of practical projects covering core algorithms and methods in Artificial Intelligence. Each notebook focuses on a specific AI paradigm such as search, constraint satisfaction, probabilistic reasoning, machine learning, or reinforcement learning. The aim is to build a foundational understanding of AI by implementing algorithms and applying them to real datasets like DNA sequences or structured logic problems.

---

## 📂 Repository Structure

| Folder | Description |
|--------|-------------|
| `Systematic Search` | Breadth-first search on logic puzzles like the Missionaries and Cannibals problem |
| `CSP-Adversarial Search` | Sudoku solving using Constraint Satisfaction, Othello game with Minimax/Alpha-Beta |
| `Bayesian Networks` | Probabilistic modeling and inference using DNA datasets |
| `Machine Learning` | Supervised classification of DNA samples using models like SVM, Random Forest, and KNN |
| `Reinforcement Learning` | Q-Learning agent trained on FrozenLake from OpenAI Gym |

---

## 🧠 Supported AI Algorithms

### 🔍 1. Systematic Search
Implemented: **Breadth-First Search (BFS)**  
Used to solve the classic **Missionaries and Cannibals** problem by exploring the full state space and enforcing safety constraints.

### ✅ 2. Constraint Satisfaction Problems (CSP)
Implemented on: **Sudoku**, **Cryptarithmetic Puzzles**  
- Backtracking Search  
- Forward Checking  
- Domain Reduction  
- Heuristics (MRV, Degree Heuristic)

### ⚔️ 3. Adversarial Search
Implemented on: **Othello (Reversi)**, **Kingdom Conflict: Eldora**  
- **Minimax Algorithm**  
- **Alpha-Beta Pruning**  
- Game tree modeling  
- Custom evaluation functions (e.g., mobility, stability, control)

### 📈 4. Machine Learning for Classification
Applied to: **DNA Classification**  
Models used:
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Decision Tree  
- Random Forest  
- Support Vector Machine (SVM)  

Each model was trained and evaluated using accuracy, confusion matrices, and relevant bioinformatics datasets.

### 📊 5. Bayesian Networks
Used for: **Probabilistic reasoning on DNA datasets**  
- Graph-based structure (DAG)  
- Conditional Probability Tables (CPTs)  
- Evidence-based inference  
Useful for predicting missing gene values or estimating likelihoods in biological systems.

### 🎮 6. Reinforcement Learning
Implemented: **Q-Learning**  
Applied to the **FrozenLake-v1** environment (OpenAI Gym) to train an agent that learns optimal actions in a slippery 4×4 grid world.  
Key components:
- Q-table learning
- ε-greedy exploration
- Performance tracking over episodes

---

## 📁 Example Notebooks

| Notebook | Topic |
|----------|-------|
| `systematic_search_missionaries_cannibals.ipynb` | BFS for logic puzzle |
| `sudoku_solver_csp.ipynb` | Solving Sudoku with CSP techniques |
| `othello_minimax_alpha_beta.ipynb` | Adversarial AI for Othello |
| `cryptarithmetic_csp.ipynb` | Digit-letter assignment via CSP |
| `kingdom_conflict_eldora.ipynb` | Strategy game with Minimax |
| `dna_classification_ml_models.ipynb` | ML models trained on DNA data |
| `bayes_net.ipynb` | Inference on genetic traits via Bayesian Network |
| `frozenlake_q_learning.ipynb` | Q-Learning agent for FrozenLake environment |

---

## 🛠 Requirements

Install dependencies using pip:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn pgmpy networkx gym
