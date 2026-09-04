# Ml-algorithms

A collection of machine learning algorithms implemented from scratch in Python.  
This repository is intended for learning and demonstration purposes — showing how core ML techniques work under the hood without relying on high-level libraries.

---

## 📌 Currently Implemented
- **[Linear Regression](ca://s?q=Explain_Linear_Regression)**  
  A fundamental supervised learning algorithm used to model the relationship between input features and a continuous target variable.

---

## ⚙️ Features
- Custom `LinearRegression` class with `fit()` and `predict()` methods
- Gradient-based parameter updates explained step by step
- Works with **pandas Series** or **NumPy arrays**
- Clear mathematical derivations alongside code

---

## 🚀 Usage Example
```python
import pandas as pd
from linear_regression import LinearRegression

# Sample training data
xTrain = pd.Series([1, 2, 3, 4, 5])
yTrain = pd.Series([2, 4, 6, 8, 10])

# Train model
lr = LinearRegression()
lr.fit(xTrain, yTrain)

# Predict
xTest = pd.Series([6, 7, 8])
y_pred = lr.predict(xTest)

print("Predictions:", y_pred)
