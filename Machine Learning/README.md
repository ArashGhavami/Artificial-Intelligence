# DNA Classification using Machine Learning

This notebook applies various supervised machine learning (ML) algorithms to classify samples in a DNA dataset. The goal is to learn patterns from gene expression or sequence-based features and accurately predict the associated genetic category or label.

---

## 🧠 Machine Learning Algorithms Used

Several ML models were trained and evaluated in this project:

### 1. Logistic Regression
A linear classifier that models the probability of class membership using the logistic function. It's a good baseline for binary or multiclass classification.

### 2. K-Nearest Neighbors (KNN)
A non-parametric algorithm that classifies a sample based on the majority class among its k closest neighbors in feature space. It works well with small datasets and can adapt to complex boundaries.

### 3. Decision Tree Classifier
A tree-based model that learns decision rules inferred from the features. It can capture non-linear relationships and provides interpretability through its tree structure.

### 4. Random Forest Classifier
An ensemble method that combines multiple decision trees (via bagging) to improve accuracy and reduce overfitting. It's robust and often achieves high performance across many domains.

### 5. Support Vector Machine (SVM)
A powerful classifier that finds the optimal hyperplane that maximizes margin between classes. It is effective in high-dimensional spaces, such as those common in genomic data.

Each model was trained, tested, and evaluated using metrics such as **accuracy**, **precision**, **recall**, and **confusion matrix**.

---

## 🧬 Application: DNA Dataset

The dataset consists of numerical features extracted from DNA samples. These could represent gene expression levels, nucleotide frequencies, or other molecular measurements.

**Task:**  
Predict the class label of each DNA sample using its feature vector. This could correspond to:
- Classifying genetic conditions or traits
- Detecting mutations or anomalies
- Grouping organisms based on genetic similarity

The project uses **supervised learning**: known labels are used during training to help the models learn to distinguish between genetic classes.

---

## ✅ Key Notebook Features

- Data loading and preprocessing (standardization, splitting)
- Training of 5 different ML classifiers
- Visualization of performance metrics (e.g., confusion matrices)
- Comparison of model accuracies and generalization behavior
- Discussion on model selection and suitability for genetic data

---

## 🛠 Requirements

Install required packages:

```bash
pip install numpy pandas matplotlib scikit-learn seaborn

