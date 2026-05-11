#  House Price Prediction using Machine Learning

##  Project Overview

This project focuses on building a Machine Learning model to predict house prices based on various property features such as size, quality, location, and construction year.

The goal is to demonstrate a complete data science pipeline, including:
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Machine Learning modeling
- Model evaluation and interpretation

---

## Dataset

The dataset comes from the Kaggle competition:

👉 House Prices: Advanced Regression Techniques  
https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques

### Target variable:
- SalePric` (house sale price)

### Features:
- Numerical and categorical variables describing houses (size, quality, rooms, etc.)

---

## 🧰 Technologies Used

- Python 
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Data Cleaning

The dataset required significant preprocessing:

- Removed columns with high percentage of missing values
- Handled missing values:
  - Numerical features → median imputation
  - Categorical features → "Missing" label
- Applied One-Hot Encoding to categorical variables

After preprocessing, the dataset was fully numerical and ready for machine learning.

---

##  Exploratory Data Analysis (EDA)

Key insights discovered:
- House price distribution is right-skewed
- Larger living area strongly correlates with higher price
- Overall quality is one of the strongest predictors of price

---

##  Machine Learning Model

### Model used:
- Random Forest Regressor

### Pipeline:
- Train/test split (80/20)
- Model training
- Prediction on test set

---

##  Model Evaluation

Performance metric used:
- Mean Absolute Error (MAE)

The model achieved a reasonable prediction error, showing good ability to estimate house prices based on input features.

---

##  Feature Importance

The most important features influencing house prices were:

- OverallQual (overall quality)
- GrLivArea (living area)
- GarageCars (garage capacity)
- YearBuilt (construction year)

This confirms that size and quality are key drivers of property value.

---

##  Model Improvement

An optimized version of the model was built using only the top important features.

Results:
- Reduced complexity
- Improved interpretability
- Comparable predictive performance

---

##  Results Summary

| Model Version | Performance (MAE) |
|--------------|------------------|
| Full Model   | 17615.393219178084                |
| Reduced Model | 18404.73551369863                |

---

##  Project Structure
