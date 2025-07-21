# 🏠 Ames Housing Price Prediction

This project was created to predict home prices using the **Ames Housing dataset**, a well-known alternative to the Boston Housing dataset for regression modeling. It demonstrates the end-to-end pipeline of data preprocessing, feature engineering, model training, and prediction.

## 📊 Dataset

The Ames Housing dataset contains 79 explanatory variables describing various aspects of residential homes in Ames, Iowa. The target variable is `SalePrice`.

- Source: [Kaggle Competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
- Goal: Predict the final price of each home in the test dataset

## 🧪 Project Workflow

1. **Get to know the data**
   - Read in train and test data
   - Explore the distribution of the target variable: examine its normality, etc.
   - Explore the distribution of covariates: Look for missing data, outliers, etc.
   - Examine the bi-variate association
  
2. **Data Cleaning**
   - Handle missing values
   - Impute or remove uninformative variables
   - Outlier removal based on domain-specific thresholds

3. **Feature Engineering**
   - Log-transform skewed variables
   - One-hot encode categorical variables
   - Normalize numeric features with `RobustScaler`

4. **Modeling**
   - Train individual models: Lasso, ElasticNet, XGBoost, LightGBM
   - Combine them with a stacked ensemble model

5. **Evaluation**
   - Metric: Root Mean Squared Log Error (RMSLE)

## 🚀 Getting Started

### 📦 Prerequisites

- Python 3.7+
- Required packages:
  - `pandas`, `numpy`, `scikit-learn`
  - `xgboost`, `lightgbm`, `seaborn`, `matplotlib`

