# Constraint Satisfaction Problems (CSP) & Adversarial Search

This directory contains implementations and examples related to two core topics in Artificial Intelligence: **Constraint Satisfaction Problems (CSPs)** and **Adversarial Search**. These represent two different AI problem-solving paradigms — one focuses on satisfying constraints, and the other on competing agents in games or decision-making environments.

---

## 1. Constraint Satisfaction Problems (CSP)

CSPs involve finding values for a set of variables that satisfy a series of constraints. Examples include:

- Sudoku
- Map coloring
- Scheduling problems
- Logic puzzles

### Core Concepts:
- **Variables**: Elements to assign values to (e.g., Sudoku cells)
- **Domains**: Possible values for each variable
- **Constraints**: Conditions that restrict valid combinations (e.g., no duplicate numbers in a row)

### Algorithms:
- **Backtracking Search**
- **Forward Checking**
- **Constraint Propagation** (e.g., AC-3)
- **Heuristics** like MRV (Minimum Remaining Values) and LCV (Least Constraining Value)

---

## 2. Adversarial Search

Adversarial Search deals with decision-making in **competitive environments** (usually two-player games). Each agent attempts to **maximize its utility while minimizing the opponent’s advantage**.

### Common Domains:
- Chess, Tic-Tac-Toe, Checkers
- Othello (Reversi)
- Strategic board games and planning

### Key Algorithms:
- **Minimax**: Recursive strategy for perfect play in deterministic, turn-based games
- **Alpha-Beta Pruning**: Optimization of Minimax to skip evaluating unnecessary branches
- **Expectimax**: For stochastic games (e.g., dice rolls)
- **Game Trees**: Representation of all possible future game states

---

## Othello Implementation Details

The `othello_minimax_alpha_beta.ipynb` notebook applies **Adversarial Search** to the game of **Othello** (also known as Reversi). Key highlights:

- **Board Representation**: 8×8 grid with pieces represented as 1 (Black), -1 (White), and 0 (Empty).
- **Move Generation**: Legal move identification by checking for flippable opponent disks in all eight directions.
- **Evaluation Function**: Combines disk difference, mobility (number of legal moves), and positional stability (corner occupancy and edge disks).
- **Minimax with Alpha-Beta Pruning**:
  - Depth-limited search (e.g., depth = 4)
  - Alpha and Beta bounds to prune branches and reduce computation
- **Performance**:
  - Average branching factor reduced by ~30% with pruning
  - Search completion time under 2 seconds for depth 4 on a standard CPU

---

## Cryptarithmetic Puzzle (CSP)

Cryptarithmetic problems involve assigning digits to letters such that a given arithmetic expression holds true (e.g., SEND + MORE = MONEY). They are a classic form of CSP, featuring:

- **Variables**: Unique letters in the equation
- **Domains**: Digits 0–9 (no repetition allowed)
- **Constraints**:
  - All letters map to unique digits
  - No leading zeroes
  - Arithmetic operation must be valid digit-wise

This implementation uses backtracking with forward checking to prune inconsistent assignments early. It demonstrates how symbolic reasoning and digit-carrying arithmetic can be handled in a CSP framework.

---

## Kingdom Conflict: Eldora (Adversarial Search)

The "Kingdom Conflict: Eldora" is a custom strategic turn-based game implemented to demonstrate **Adversarial Search** in a richer state space. Each player controls a faction aiming to capture territory and outmaneuver the opponent.

### Features:
- **Game Map**: A graph-based representation of regions
- **Actions**: Move, attack, defend, expand
- **Game Tree**: Explored using Minimax with Alpha-Beta pruning
- **Evaluation Function**: Weights control over regions, troop strength, and threat zones

This implementation emphasizes how complex multi-factor heuristics can be embedded into a search algorithm to yield smart, tactical gameplay decisions.

---

## 🔧 Requirements

Typical notebooks in this directory may require:

```bash
pip install numpy matplotlib

