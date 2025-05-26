# Predicting_House_Prices_Using_Boston_Housing_DataSet
This project demonstrates how to implement basic regression algorithms from scratch (without using libraries like `scikit-learn` for modeling) to predict house prices using the Boston Housing Dataset.

## Dataset

Used the Boston Housing Dataset from Kaggle (https://www.kaggle.com/datasets/altavish/boston-housing-dataset), which contains features related to housing and neighborhood characteristics in Boston, along with the median house value.

---

##  Project Steps

### 1. Data Preprocessing
- Loaded the dataset from CSV.
- Checked and renamed the target column to `median_house_value`.
- Handled missing values by dropping rows with NaNs.
- Scaled numerical features using `MinMaxScaler`.

### 2. Model Implementation (from scratch)
- Linear Regression
- Random Forest Regressor
- XGBoost-style Gradient Boosting Regressor

> Note: These models are implemented from scratch, using only NumPy.

### 3. Model Evaluation
- Used **RMSE (Root Mean Square Error)** and **R² (coefficient of determination)** as performance metrics.

### 4. Feature Importance
- For tree-based models (Random Forest & XGBoost), feature importance is computed based on how often features are used in splits.
- Bar plots are displayed for visualization.

---
# Observations
- Linear Regression performs decently but is outperformed by tree-based models in most cases.
- Random Forest is robust and generally yields better RMSE and R².
- XGBoost-style boosting reduces errors further by correcting previous predictions using residuals.
- Feature importance shows that variables like RM (average rooms per dwelling) and LSTAT (lower status of the population) have significant influence on price.

# Learnings
- Implementing models from scratch deepens understanding of their mechanics.
- Data preprocessing and normalization significantly affect model performance.
- Feature importance from ensemble models provides great insights into influential variables.
