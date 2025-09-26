# Credit Card Fraud Detection

## Dataset

This project uses the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

1. Download the dataset from Kaggle.
2. Place the file inside the `data/` folder with the name `creditcard.csv`.

## What is Fraud?

Fraud refers to any intentional act of deception carried out to gain an unfair or unlawful advantage. In financial systems, this can include:

- **Credit card fraud**
- **Identity theft**
- **Fake transactions**
- **Money laundering**
- **Insurance or loan fraud**

Fraud not only causes **financial losses** but also damages **trust** in businesses, banks, and digital platforms.

---

## Why is Fraud Detection Important?

- 💰 **Financial Protection** – Prevents monetary losses for individuals, banks, and companies.  
- 🔒 **Security & Trust** – Builds confidence among users in digital payment systems.  
- ⚖️ **Regulatory Compliance** – Helps organizations meet government and financial regulations.  
- ⚡ **Early Intervention** – Detecting fraud in real-time can stop large-scale damage before it spreads.

---

## 📊 Evaluation Metrics  

Fraud detection is an **imbalanced classification problem**, so metrics beyond accuracy are critical. Below are the key metrics we use and their target thresholds:  

- **Precision (≥ 90%)**  
  - Ensures that the majority of transactions flagged as fraud are truly fraudulent.  
  - Reduces false alarms and improves user trust.  

- **Recall (≥ 80%)**  
  - Ensures that most fraudulent transactions are caught.  
  - Prevents fraudsters from slipping through undetected.  

- **F1-Score (≥ 85%)**  
  - Harmonic mean of precision and recall.  
  - Balances catching fraud with minimizing false positives.  

- **ROC-AUC (≥ 0.90)**  
  - Evaluates the model’s ability to distinguish between fraud and non-fraud.  
  - Higher AUC = better overall performance.  

- **Latency (≤ 200ms per transaction)**  
  - The pipeline should flag fraud in near **real-time**.  
  - Critical for production deployment in financial systems.  

⚠️ **Note:** Accuracy is not emphasized here because fraud datasets are highly imbalanced (e.g., 99% genuine vs. 1% fraud). A model predicting “no fraud” for everything would show 99% accuracy but be useless in practice.  

