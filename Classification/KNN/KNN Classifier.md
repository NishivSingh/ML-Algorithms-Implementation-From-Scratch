# 📘 K-Nearest Neighbors (KNN) Classifier

This document explains the **K-Nearest Neighbors (KNN)** algorithm implemented from scratch in Python.

---

## **Overview**

**KNN** is a simple, non-parametric, instance-based learning algorithm used for **classification**.  
It predicts the class of a new data point based on the **majority class among its K nearest neighbors** in the training set.

- **Non-parametric:** No assumptions about data distribution.  
- **Instance-based:** Uses training data during prediction.  
- **Distance metrics:** Supports Euclidean, Manhattan, and Minkowski distances. 
  - **Euclidean:** √(Σ (xᵢ - yᵢ)²)  
  - **Manhattan:** Σ |xᵢ - yᵢ| 
  - **Minkowski:** (Σ |xᵢ - yᵢ|ᵏ)^(1/k) 

---

## **Algorithm Steps**

1. **Choose K and distance metric**  
2. **Compute distance** between test point and all training points.  
3. **Select K nearest neighbors** by sorting distances.  
4. **Majority vote:** Predict the label that appears most among K neighbors.  
5. **Return predicted label**.  

---

## **Evaluation Metrics**

- **Accuracy:** Fraction of correctly predicted labels.  
- **Confusion Matrix:** True vs predicted labels.  
- Optional: Precision, Recall, F1-score for multi-class problems.  

---

## **Advantages**

- Simple and easy to implement.  
- Works well on small datasets.  
- No training phase required (lazy learning).  

---

## **Limitations**

- Computationally expensive for large datasets.  
- Sensitive to irrelevant features and feature scaling.  
- Choice of K and distance metric affects performance.  
