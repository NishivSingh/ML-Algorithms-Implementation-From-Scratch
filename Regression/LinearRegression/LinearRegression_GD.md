# 📘 Linear Regression (Gradient Descent Method)  

This document explains the **Linear Regression** algorithm implemented using the **Gradient Descent** method — an iterative optimization technique to find the optimal parameters.  

---

## 🧠 Overview  

Linear Regression models the relationship between features $X$ and a continuous target variable $y$ by fitting a linear function:  

$$
h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 x_2 + \dots + \theta_n x_n
$$  

Where $\theta$ are the model parameters.  

---

## 🔍 Objective  

We aim to minimize the **Mean Squared Error (MSE)** cost function:  

$$
J(\theta) = \frac{1}{2m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})^2
$$  

---

## ⚙️ Gradient Descent Solution  

Gradient Descent updates the parameters iteratively using:  

$$
\theta := \theta - \alpha \cdot \frac{\partial J(\theta)}{\partial \theta}
$$  

Where:  
- $\alpha$ = learning rate (controls step size)  
- $\frac{\partial J(\theta)}{\partial \theta}$ = gradient of the cost function w.r.t. parameters  

For Linear Regression, the gradient can be expressed as:  

$$
\frac{\partial J(\theta)}{\partial \theta} = \frac{1}{m} X^T (X\theta - y)
$$  

The algorithm steps:  
1. Initialize $\theta$ (usually zeros)  
2. Repeat until convergence or max iterations:  
   - Compute predictions  
   - Calculate gradients  
   - Update parameters  

---

## ✅ Advantages  

- Works well with large datasets where Normal Equation becomes slow  
- Can be applied to models without a closed-form solution  
- Easy to extend with regularization (L1, L2)  

---

## ❌ Limitations  

- Requires tuning of learning rate ($\alpha$)  
- May converge slowly or not at all if $\alpha$ is too large/small  
- Requires multiple iterations to reach optimal parameters  

---
