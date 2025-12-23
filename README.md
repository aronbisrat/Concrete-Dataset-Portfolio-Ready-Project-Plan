# Concrete Compressive Strength Prediction

## Overview
This project predicts the compressive strength of concrete using machine learning models trained on mixture composition and curing age.

The work demonstrates:
- Exploratory Data Analysis (EDA)
- Domain-informed feature engineering
- Model comparison and evaluation using cross-validation
- Hyperparameter tuning with XGBoost

## Dataset
- Source: UCI Concrete Compressive Strength Dataset
- Samples: 1,030
- Features: Cement, aggregates, water, additives, age

## Feature Engineering
Key engineered features include:
- Water–Cement Ratio
- Aggregate–Cement Ratio
- Fine–Coarse Aggregate Ratio
- Age squared (nonlinear aging effect)

These features are grounded in civil engineering domain knowledge.

## Models Used
- Random Forest Regressor (baseline)
- XGBoost Regressor
- Tuned XGBoost with GridSearchCV

## Evaluation Metric
- Mean Absolute Error (MAE)
- Cross-validation (5-fold)

**Best MAE:** ~8 MPa

## Results & Insights
- Water–Cement ratio is the strongest predictor
- Engineered ratios improved model performance
- XGBoost outperformed Random Forest after tuning

## Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

## How to Run
1. Clone the repository
2. Open the notebook
3. Run all cells (no GPU required)

## Author
Aron Bisrat  
