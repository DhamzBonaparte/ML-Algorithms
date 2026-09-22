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

- **[Stochastic Gradient Descent (SGD)](ca://s?q=Explain_Stochastic_Gradient_Descent)**  
  Variant of gradient descent where parameters are updated using **one randomly chosen sample** at a time.  
  - Faster updates, introduces noise that can help escape local minima.  
  - Demonstrates trade‑off between convergence speed and stability.

- **[Mini‑Batch Gradient Descent](ca://s?q=Explain_Mini_Batch_Gradient_Descent)**  
  Hybrid approach between batch and stochastic gradient descent.  
  - Updates parameters using **small batches of samples**.  
  - Balances efficiency and stability.  
  - Commonly used in deep learning training.

- **[Ridge Regression](ca://s?q=Explain_Ridge_Regression)**  
  A regularized version of linear regression that adds a penalty term to shrink coefficients.  
  - Helps prevent overfitting when features are highly correlated.  
  - Implemented with closed‑form solution.  

- **[Multiple Ridge Regression](ca://s?q=Explain_Multiple_Ridge_Regression)**  
  Extension of ridge regression for multi‑feature datasets.  
  - Handles intercept and multiple slopes with regularization.  
  - Demonstrates stability compared to ordinary least squares when multicollinearity exists.

- **[Gradient Descent Ridge Regression](ca://s?q=Explain_Gradient_Descent_Ridge_Regression)**  
  Extension of gradient descent applied to ridge regression.  
  - Uses iterative updates to minimize the **ridge cost function**  
    where the gradient includes both the error term and the regularization penalty.  
  - Demonstrates how ridge regression can be solved not only with closed‑form solutions but also with **iterative optimization**, making it scalable for large datasets.  
  - Highlights the trade‑off between bias and variance controlled by the regularization parameter.


- **[Perceptron Trick](ca://s?q=Explain_Perceptron_Algorithm)**  
  A foundational binary classifier that inspired logistic regression.  
  - Works by finding a separating line (or hyperplane) between classes.  
  - Stops once it finds *any* viable separating line.  
  - Limitation: does not continue searching for the **optimal solution**, unlike logistic regression which optimizes using maximum likelihood.

- **[Sigmoid Logistic Regression](ca://s?q=Explain_Logistic_Regression)**  
  A probabilistic classifier that improves upon the perceptron.  
  - Uses the **sigmoid function** to map linear combinations of inputs into probabilities between 0 and 1.  
  - Decision boundary occurs at probability = 0.5 → corresponds to \(w^T x + b = 0\).  
  - Unlike the perceptron, logistic regression continues optimizing the boundary using maximum likelihood, ensuring the **best fit** rather than just any separating line.

- **[Logistic Regression with Cross‑Entropy Loss](ca://s?q=Explain_Cross_Entropy_Loss_in_Logistic_Regression)**  
  A full implementation of logistic regression using the **cross‑entropy cost function**
  - Gradient descent is applied to minimize this loss.  
  - Ensures the model finds the **optimal separating boundary** by maximizing likelihood.  
  - Demonstrates the difference between perceptron’s hard cutoff and logistic regression’s smooth probability optimization.

- **[K‑Nearest Neighbors (KNN) Classifier](ca://s?q=Explain_KNN_Classifier)**  
  A non‑parametric supervised learning algorithm used for classification.  
  - Predicts the class of a sample by looking at the **majority vote** among its *k* nearest neighbors in feature space.  
  - Distance metrics (e.g., Euclidean, Manhattan) determine closeness.  
  - Sensitive to feature scaling → preprocessing with normalization/standardization is essential.  
  - Demonstrates how instance‑based learning differs from parametric models like logistic regression.

- **[K‑Means Clustering](ca://s?q=Explain_K_Means_Clustering)**  
  An unsupervised machine learning algorithm used to partition a dataset into $k$ distinct, non-overlapping clusters.  
  - Iteratively assigns data points to the nearest cluster centroid and recalculates centroids based on the mean of assigned points.  
  - Uses distance metrics (such as Euclidean distance) to measure similarity.  
  - Demonstrates how unsupervised learning discovers hidden patterns and groupings in unlabeled data, unlike supervised classifiers like KNN.
---

## ⚙️ Features
- Custom `LinearRegression`, `MultipleLinearRegression`, `GradientDescent`, `MyMultipleGDRegressor`, `StochasticGDRegressor`, `MiniBatchGDRegressor`, `RidgeRegressor`, `MultipleRidgeRegressor`, `Perceptron`, `LogisticRegressionSigmoid`,`LogisticRegressionCrossEntropy` and `KMeans` implementations with `fit()` and `predict()` methods
- Gradient-based and closed‑form parameter updates explained step by step
- Works with **pandas Series**, **NumPy arrays**, or scikit-learn datasets
- Clear mathematical derivations alongside code
- Demonstrates: 
  - **Single-variable regression**
  - **Multi-variable regression**
  - **Gradient descent optimization**
  - **Multiple gradient descent regression** 
  - **Stochastic gradient descent**
  - **Mini‑batch gradient descent**
  - **Ridge regression**
  - **Multiple ridge regression**
  - **Perceptron classification**
  - **Logistic regression with sigmoid**
  - **Logistic regression with cross‑entropy loss**
  - **KNN Classifier**
  - **KMeans Classifier**

## 📌 Demo Implementations (using scikit‑learn)

These are **demo usage examples** included to show how popular ML algorithms can be applied quickly with scikit‑learn.  
Unlike the from‑scratch implementations above, these demos rely on scikit‑learn’s built‑in classes.

- **AdaBoost**  
  - Demo of `AdaBoostClassifier`. 
  - Shows how boosting reweights samples to focus on hard cases.

- **GradientBoostingRegressor**  
  - Demo using scikit‑learn’s gradient boosting for regression tasks.  
  - Highlights how weak learners are added iteratively to minimize residuals.

- **Naive Bayes**  
  - Demo of Naive Bayes.
  - Illustrates probabilistic classification based on Bayes’ theorem.

