# Financial Risk Prediction

This project focuses on predicting **financial risk levels** of individuals using decision tree models.  
The dataset contains demographic, financial, and credit-related attributes, with the goal of classifying people into **Low**, **Medium**, or **High** risk categories.

📂 Dataset can be downloaded from the following link:  
[Download dataset (Google Drive)](https://drive.google.com/drive/folders/1wIU5vF7iNSqh5gnrZuwHoWDU5kDnBiZ8?usp=sharing)

The notebook: **`financial-risk-prediction.ipynb`**

---

## Project Overview
The project is divided into two main parts:

- **Part I: Implementing Decision Tree (ID3)**
  - Handle missing values using custom preprocessing.
  - Encode categorical attributes manually (without external preprocessing libraries).
  - Split dataset into **train (70%)**, **test (15%)**, and **validation (15%)**.
  - Train a decision tree using the **ID3 algorithm**.
  - Evaluate with multiple metrics and generate rules (root-to-leaf paths).
  - Analyze misclassified samples and provide commentary.

- **Part II: Decision Tree Pruning**
  - Apply pruning to reduce overfitting and improve generalization.
  - Iteratively remove low-information branches.
  - Compare **pre-pruning** and **post-pruning** performance.
  - Report pruned features and reasoning behind them.

---

## Dataset
The dataset contains **15,000 samples** with **19 attributes**.  
Key features include:

- Age, Gender, Education Level, Marital Status  
- Income, Credit Score, Loan Amount, Loan Purpose  
- Employment Status, Years at Current Job  
- Payment History, Debt-to-Income Ratio, Assets Value  
- Number of Dependents, City, State, Country  
- Previous Defaults, Marital Status Change  
- **Risk Rating (target): Low / Medium / High**

---

## Methods and Models
- **Algorithm:** Decision Tree (ID3, implemented from scratch)  
- **Pruning:** Post-pruning based on Information Gain and validation accuracy  
- **Metrics:**  
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
  - Confusion Matrix  

---

## Installation
```bash
# Python 3.9+ recommended
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate
pip install -U pip
pip install -r requirements.txt
