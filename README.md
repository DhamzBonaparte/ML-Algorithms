# ML-algorithms

A collection of machine learning algorithms implemented from scratch in Python.  
This repository is intended for learning and demonstration purposes, showing how core ML techniques work under the hood without relying on high-level libraries.

---

## 📌 Currently Implemented
- **[Linear Regression](ca://s?q=Explain_Linear_Regression)**  
  A fundamental supervised learning algorithm used to model the relationship between input features and a continuous target variable.

- **[Multiple Linear Regression](ca://s?q=Explain_Multiple_Linear_Regression)**  
  An extension of linear regression that models the relationship between several input features and a continuous target variable. Implemented and tested using the **[Diabetes dataset](ca://s?q=Scikit_learn_diabetes_dataset)** from scikit-learn.

- **[Gradient Descent](ca://s?q=Explain_Gradient_Descent)**  
  Optimization algorithm used to minimize the cost function.  
  - First implemented with **only the intercept (b)** term.  
  - Extended to include both **intercept and slope** for parameter updates.

- **[Multiple Gradient Descent Regression](ca://s?q=Explain_Multiple_Gradient_Descent)**  
  A generalized gradient descent implementation for **multi‑feature regression**.  
  - Updates all coefficients simultaneously using vectorized operations.  
  - Handles intercept and multiple slopes efficiently.  
  - Demonstrates convergence behavior compared to closed‑form regression.

---

## ⚙️ Features
- Custom `LinearRegression`, `MultipleLinearRegression`, `GradientDescent`, and `MyMultipleGDRegressor` implementations with `fit()` and `predict()` methods
- Gradient-based parameter updates explained step by step
- Works with **pandas Series**, **NumPy arrays**, or scikit-learn datasets
- Clear mathematical derivations alongside code
- Demonstrates:
  - **Single-variable regression**
  - **Multi-variable regression**
  - **Gradient descent optimization**
  - **Multiple gradient descent regression**

---
