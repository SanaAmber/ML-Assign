 🌍 Mastering Gradient Boosting: A World Happiness Tutorial

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange?style=flat-square&logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![University](https://img.shields.io/badge/University-Hertfordshire-purple?style=flat-square)

---

## 📖 About This Project

This repository contains a **comprehensive machine learning tutorial** on **Gradient Boosting**, submitted as part of the Machine Learning module at the University of Hertfordshire.

The tutorial teaches Gradient Boosting from the ground up — from the core intuition of *learning from mistakes*, through the mathematics of gradient descent in function space, to hands-on hyperparameter tuning and model interpretability using SHAP values. Everything is demonstrated on a **World Happiness dataset**, predicting a country's Life Ladder (happiness) score from six real-world indicators.

| Detail | Info |
|---|---|
| **Author** | Sana Amber |
| **Student ID** | 24140806 |
| **Module** | Machine Learning |
| **Module Leader** | Dr Darshan Kakkad |
| **Institution** | University of Hertfordshire |
| **Submission Date** | 27 March 2026 |

---

## 🎯 What You Will Learn

By working through this tutorial, you will be able to:

- Explain how Gradient Boosting works sequentially — building each tree to correct the errors of the last
- Compare Gradient Boosting against Linear Regression, Decision Trees, Random Forest, and AdaBoost
- Tune the three key hyperparameters (learning rate, max depth, number of estimators) using Grid Search and cross-validation
- Interpret model predictions using **SHAP (SHapley Additive exPlanations)** values
- Recognise common pitfalls and apply best practices in real-world projects

---

## 🚀 Getting Started

### Prerequisites

Make sure you have **Python 3.8 or higher** installed. You can check with:

```bash
python --version
```

### 1. Clone the Repository

```bash
git clone https://github.com/[your-username]/gradient-boosting-tutorial.git
cd gradient-boosting-tutorial
```

### 2. Install Required Libraries

Install all dependencies with a single command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn shap jupyter
```

Or if you prefer using a requirements file:

```bash
pip install -r requirements.txt
```

### 3. Launch the Notebook

```bash
jupyter notebook world_happiness_tutorial.ipynb
```

Then run all cells from top to bottom using **Cell > Run All**.

> **Note:** Running the full notebook takes approximately 2–4 minutes due to Grid Search cross-validation.

---

## 📊 Dataset

The tutorial uses a **synthetic World Happiness dataset** with 250 observations, constructed using realistic feature ranges from the [World Happiness Report](https://worldhappiness.report/).

The dataset includes the following features:

| Feature | Range | Relationship to Happiness |
|---|---|---|
| GDP per Capita | 0.3 – 1.8 | Strong positive (+3.5) |
| Social Support | 0.2 – 1.0 | Strong positive (+2.8) |
| Health Expectancy | 40 – 80 yrs | Mild positive (+0.04) |
| Freedom | 0.1 – 0.95 | Positive (+2.2) |
| Generosity | 0.0 – 0.60 | Positive (+1.8) |
| Corruption | 0.0 – 0.70 | Negative (−1.8) |

The target variable — **Life Ladder** — is generated using a known formula, which allows us to verify that Gradient Boosting correctly learns the true relationships.

---

## 🗂️ Tutorial Sections

The notebook is divided into **9 teaching sections**:

| # | Section | What It Covers |
|---|---|---|
| 1 | What Is Gradient Boosting? | Theory, intuition, kitchen analogy, mathematical framework, history |
| 2 | Setup & Data Preparation | Libraries, dataset creation, feature engineering |
| 3 | Algorithm Comparison | GB vs Linear Regression, Decision Tree, Random Forest, AdaBoost |
| 4 | Hyperparameter: Learning Rate | Effect of shrinkage on model accuracy |
| 5 | Hyperparameter: Max Depth | Controlling tree complexity |
| 6 | Hyperparameter: N Estimators | Number of boosting rounds |
| 7 | Grid Search & Cross-Validation | Systematic hyperparameter optimisation |
| 8 | Feature Importance & SHAP | Interpreting the model with impurity scores and SHAP values |
| 9 | Best Practices & Summary | Pitfalls, decision guide, key takeaways |

---

## 📈 Key Results

After tuning with Grid Search + 5-fold cross-validation, the optimised Gradient Boosting model achieves:

| Metric | Value |
|---|---|
| R² Score | > 0.85 |
| RMSE | < 0.12 |
| MAE | < 0.09 |
| Mean Residual | ≈ 0.00 (no systematic bias) |

The model correctly identifies **GDP per Capita** as the strongest happiness driver and **Health Expectancy** as the weakest — exactly matching the known data-generating formula.

---

## ♿ Accessibility

This tutorial was designed with accessibility in mind:

- All plots use **Paul Tol's colourblind-safe palette** (`#0173B2`, `#029E73`, `#DE8F05`, `#CC78BC`, `#D55E00`)
- Every figure includes a descriptive **alt-text caption** in the report
- The written report uses **structured headings** compatible with screen readers
- Code cells include clear **comments** explaining each step

---
