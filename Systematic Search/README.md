# Systematic Search

This notebook demonstrates a **Systematic Search** approach for solving a defined problem in Artificial Intelligence. Systematic search refers to methods that explore the problem space in a structured and exhaustive way, often used in pathfinding, constraint satisfaction, and decision-making tasks.

## 🔍 Algorithm: Systematic Search

Systematic search explores the problem space methodically, often by generating and expanding nodes based on a clear set of rules. Common forms include:

- **Breadth-First Search (BFS)**
- **Depth-First Search (DFS)**
- **Uniform Cost Search**
- **Iterative Deepening**
- **Backtracking for CSPs**

These algorithms are designed to find a solution (or prove none exists) while guaranteeing completeness, and in some cases, optimality.

The notebook includes:
- State representation
- Successor function
- Goal checking
- Frontier and explored set management

## 🗂 Dataset / Problem Setup

This particular implementation applies the search algorithm to a predefined problem (e.g., puzzle-solving, state transition space, or logical deduction). The dataset or problem setup is simple and structured to emphasize the logic of the search rather than the scale or complexity of data.

## 🛠 Requirements

```bash
pip install numpy matplotlib

