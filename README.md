# loan-default-risk-optimization
# Loan Default Risk with Business Cost Optimization

## 📌 Project Overview
This project predicts the likelihood of loan default using the **Home Credit Default Risk Dataset**.  
The objective is not just classification but also **business cost optimization** — minimizing financial loss by adjusting the decision threshold.

## 🎯 Objectives
- Preprocess and clean the dataset  
- Train binary classification models:
  - Logistic Regression
  - CatBoost Classifier
- Define business cost values for false positives & false negatives  
- Adjust decision threshold to minimize total business cost  
- Analyze feature importance  

## 📊 Dataset
- **Source:** [Home Credit Default Risk Dataset (Kaggle)](https://www.kaggle.com/datasets/anggundwilestari/home-credit)  
- File used: `HC_application_train.csv`  
- Shape: **307,511 rows × 122 columns**

## ⚙️ Methodology
1. Data preprocessing (handling missing values, encoding categorical variables)  
2. Train/Test split (80/20)  
3. Logistic Regression & CatBoost training  
4. Evaluate using **AUC (ROC curve area)**  
5. Cost-sensitive threshold optimization  
6. Feature importance analysis (CatBoost)  

## 📈 Results
- **Logistic Regression AUC:** 0.7483  
- **CatBoost AUC:** 0.7620  

### ✅ Optimized Threshold
- Best Threshold: **0.18**  
- Minimum Business Cost: **2,064,700**

- 
- **Accuracy:** 87.8%  

### 🔝 Top 5 Features (CatBoost Importance)
1. EXT_SOURCE_3  
2. EXT_SOURCE_2  
3. DAYS_BIRTH  
4. EXT_SOURCE_1  
5. AMT_CREDIT  




### 🔢 Confusion Matrix at Optimal Threshold
