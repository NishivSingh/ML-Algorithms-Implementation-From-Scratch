# 📘 Linear Regression (Normal Equation Method)

This document explains the **Linear Regression** algorithm implemented using the **Normal Equation** — a direct, closed-form solution to find the optimal parameters without iterative methods.

---

## 🧠 Overview

Linear Regression models the relationship between features \( X \) and a continuous target variable \( y \) by fitting a linear function:

\[
h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 x_2 + \dots + \theta_n x_n
\]

Where \( \theta \) are the model parameters.

---

## 🔍 Objective

We aim to minimize the **Mean Squared Error (MSE)** cost function:

\[
J(\theta) = \frac{1}{2m} \sum_{i=1}^m (h_\theta(x^{(i)}) - y^{(i)})^2
\]

---

## ⚙️ Normal Equation Solution

The Normal Equation provides a closed-form solution for \( \theta \):

$$
\mathbf{\theta} = \left( \mathbf{X}^T \mathbf{X} \right)^{-1} \mathbf{X}^T \mathbf{y}
$$

- \( X \) is the design matrix with a bias term column (ones)
- \( y \) is the vector of target values
- \( \theta \) is the parameter vector (including intercept)

No need to tune hyperparameters like learning rate or iterate multiple times.

---
