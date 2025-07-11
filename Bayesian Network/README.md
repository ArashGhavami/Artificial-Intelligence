# Bayesian Network for DNA Data Inference

This notebook demonstrates the use of a **Bayesian Network (Bayes Net)** to model and reason about uncertainty in a DNA-based dataset. The focus is on building a probabilistic graphical model to represent the dependencies between genetic variables and performing inference over this structure.

---

## 📊 What is a Bayesian Network?

A **Bayesian Network** is a probabilistic graphical model that represents a set of variables and their conditional dependencies using a directed acyclic graph (DAG). Each node corresponds to a random variable, and each edge represents a direct probabilistic dependency.

### Key Components:
- **Nodes**: Represent variables (e.g., gene presence, mutation status)
- **Edges**: Represent conditional dependencies between variables
- **CPTs (Conditional Probability Tables)**: Quantify the relationship between a node and its parents

Bayesian networks enable efficient **joint probability modeling** and **inference** (e.g., calculating the probability of one event given evidence about another).

---

## 🧬 Application: DNA Dataset

In this notebook, a DNA dataset is used to model genetic relationships and infer properties such as:

- The probability of a specific gene or marker being present given other observed markers
- The likelihood of genetic traits or mutations based on probabilistic dependencies
- Inference tasks under partial observability (e.g., using known gene values to estimate missing ones)

The model helps explore how evidence in one part of the genome may probabilistically influence outcomes in other regions.

---

## ✅ Features of the Notebook

- Construction of a Bayesian Network graph based on biological assumptions or data patterns
- Definition of conditional probability tables (CPTs) for each node
- Probabilistic inference using evidence variables
- Analysis of how specific gene markers affect outcomes
- Useful for educational and bioinformatics applications

---

## 🛠 Requirements

To run this notebook, install the required packages:

```bash
pip install pgmpy pandas networkx matplotlib

