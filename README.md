# 📊 Numerical & Categorical Data Preprocessing in Machine Learning
> **"A strong Machine Learning model always starts with well-prepared data."**
## 📖 Overview
Data Preprocessing is one of the most important stages in the Machine Learning workflow. Real-world data is often incomplete, inconsistent, and unstructured. Before training a model, data must be cleaned, transformed, and prepared so that algorithms can learn meaningful patterns effectively.

This repository provides a comprehensive guide to Numerical and Categorical Data Preprocessing techniques used in Machine Learning.

---

## 🚀 Core Preprocessing Techniques
### 1️⃣ Data Cleaning & Missing Values
* **Cleaning:** Removing duplicates, fixing incorrect data types, and standardizing text formats (e.g., `MALE`, `male` ➔ `Male`).
* **Missing Values:** Handled via Mean, Median, Mode imputation or predictive modeling.

### 2️⃣ Numerical Data Preprocessing
* **Feature Scaling:** 
  * *Min-Max (Normalization):* Scales data between 0 and 1.
  * *StandardScaler (Z-Score):* Centers data (Mean=0, Std=1).
  * *RobustScaler:* Best for datasets with heavy outliers.
* **Outlier Treatment:** Detection using Box Plots, Z-Score, and IQR.
* **Feature Transformation:** Reshaping skewed data using Log, Box-Cox, and Yeo-Johnson transformations.

### 3️⃣ Categorical Data Encoding
Algorithms need numbers, not text.
* **Label / Ordinal Encoding:** For categories with a natural order (e.g., *High School = 1, Graduate = 2*).
* **One-Hot Encoding:** Creates binary (`0`/`1`) columns for nominal data (e.g., *Red, Blue, Green*).
* **Rare Categories:** Grouping low-frequency labels into an "Other" bucket to improve model efficiency.

---

## ⚠️ Common Mistakes to Avoid (Crucial)
❌ **Data Leakage:** Never scale your data *before* splitting. **Always `train_test_split` first**, fit the scaler on the training data, and then transform both train and test data.
❌ **Blindly Removing Outliers:** Investigate outliers first; they might hold vital business insights (like fraud detection).
❌ **Label Encoding on Nominal Data:** This forces algorithms to assume fake mathematical relationships.

---

## 🔄 Standard Preprocessing Pipeline
`Raw Data` ➔ `Clean Text & Duplicates` ➔ `Handle Missing Values` ➔ `Treat Outliers` ➔ `Encode Categories` ➔ `Scale Features` ➔ `Model Training`

---
## 🛠️ Technologies Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

---
## 🤝 Connect With Me
Let's connect and talk about Machine Learning, Data Science, and AI!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sujit-padhan-5024053ab)
[![Medium](https://img.shields.io/badge/Medium-Read_Article-black?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@sujit-padhan)
## 👨‍💻 Author
---
**Sujit Kumar Padhan**

If you found this repository helpful, consider giving it a ⭐
