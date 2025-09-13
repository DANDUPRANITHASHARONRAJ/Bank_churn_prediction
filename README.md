# 🏦 Bank Churn Prediction (Ensemble)

## 🎯 Objective
Build a binary classification model to predict whether a bank customer will **churn (Exited = 1)** or **stay (Exited = 0)**. The project aims to demonstrate best practices in **data preparation, feature engineering, model building, and interpretability**.

---

## 🛠️ Tech Stack
- **Languages:** Python  
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, xgboost, lightgbm, catboost  
- **Tools:** Jupyter Notebook, Kaggle  

---

## 📂 Dataset
- Source: Kaggle Playground Series (synthetic) + Original Bank Churn dataset  
- Records: ~10,000 customers  
- Features: Demographic, financial, and behavioral attributes (e.g., Age, Credit Score, Balance, Geography, Gender, Tenure, Products, etc.)  

---

## 🔑 Key Steps & Workflow

### 1. Data Preparation
- Combined synthetic and original datasets for more robust training  
- Handled missing values, scaling (RobustScaler), and encoding (OneHot)  

### 2. Feature Engineering
- **Binning:** Age categories, Credit Score ranges  
- **Ratios:** Balance-to-Salary Ratio  
- **Interactions:** Geography × Gender, Total Products Used  
- **Text Features:** TF-IDF + SVD on Surnames (5 latent features)  

### 3. Exploratory Data Analysis
- Identified **class imbalance** (~80% non-churn vs 20% churn)  
- Visualized distributions of key features (Age, Balance, Products, etc.)  

### 4. Modeling
- Models used: **XGBoost, LightGBM, CatBoost, MLP**  
- Optimized hyperparameters using GridSearchCV / Optuna  
- Final prediction: **Ensemble of XGBoost + LightGBM + CatBoost**  

### 5. Evaluation
- Metric: Accuracy, F1-score, ROC-AUC  
- Achieved **~85% accuracy** and **12% reduction in false negatives**  
- Feature importance analysis for model interpretability  

---

## 📊 Results
- Delivered a strong ensemble solution 
- Key drivers of churn: **Age, Number of Products, IsActiveMember, Geography, Credit Score**  
- Actionable outcome: Enables banks to **identify high-risk customers** and design **targeted retention strategies**  

---
