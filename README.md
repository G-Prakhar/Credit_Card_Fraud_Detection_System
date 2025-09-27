# 🛡️ Fraud Detection System

---

### 🔍 What is Fraud?
Fraud refers to **unauthorized or deceptive financial transactions** that cause monetary loss to businesses or customers.  
Examples include stolen credit cards, fake accounts, and abnormal purchases.

---

### ⚠️ Why is Fraud Detection Important?
- Fraud cases are **rare but costly**, making them hard to spot.  
- A fraud detection model that isn’t accurate can lead to:
  - Missed frauds → huge financial loss.  
  - Too many false alarms → frustrated customers.  
- Detecting fraud quickly helps save money, protect trust, and keep systems secure.

---

### 📊 What Metrics Matter (and Why)?
Accuracy alone isn’t enough. In fraud detection, the following metrics matter most:

- **Recall (True Positive Rate)** → Must be high, because missing a fraud is very expensive.  
- **Precision** → Important to reduce false alarms.  
- **F1-score** → Balances recall and precision.  
- **ROC-AUC** → Evaluates how well the model separates fraud vs. non-fraud.  

✅ Focus will be on **Recall and F1-score**.

---

### 📥 Dataset Features & Target

| **Feature Name** | **Type**     | **Description**                          |
|------------------|--------------|------------------------------------------|
| `Time`           | Numeric      | Seconds elapsed between each transaction |
| `Amount`         | Numeric      | Value of the transaction                 |
| `V1 … V28`       | Numeric      | Anonymized PCA-transformed features      |
| `Class` (Target) | Categorical  | 0 = Legitimate, 1 = Fraudulent           |

---

### 🎯 Target Metrics & Thresholds
To consider the project successful:
- **Recall ≥ 0.80** (catch at least 80% of frauds)  
- **F1-score ≥ 0.85** (balance precision & recall)  

---

### ⚡ Constraints & Assumptions
- Dataset is **highly imbalanced** (fraud cases ~0.17%).  
- Fraud patterns evolve → model must be updated over time.  
- In the real world, the system needs **real-time predictions**.  
- For this project, we assume access to the Kaggle Credit Card Fraud Detection dataset.  

---

### 🧾 Problem Statement
> Build a machine learning system that detects fraudulent credit card transactions.  
> The system should prioritize **high recall** to minimize missed frauds, while keeping false positives under control.  
> The solution should be scalable and capable of real-time prediction.

---
