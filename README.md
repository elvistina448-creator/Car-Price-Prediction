# Car Price Prediction Using Multiple Linear Regression & CatBoost 

## Table of Contents 

- [Project Evaluation](#project-evaluation) 
- [Data Preprocessing](#data-preprocessing) 
- [Models Included](#models-included) 
- [Model Evaluation](#model-evaluation) 
- [Key Skills Demonstrated](#key-skills-demonstrated) 
- [Future Improvements](#future-improvements) 

## Project Evaluation 

This project predicts car prices using two machine learning models, Multiple Linear Regression (MLR) as the main project model, and CatBoost as an additional advanced model to improve accuracy and compare performance. 

The dataset includes various car attributes such as engine size, fuel type, horsepower, car brand, and body type. The goal was to build an interpretable baseline model (MLR) and then test with a different model to see if I could reduce prediction error. 

## Data Preprocessing 

- Data had no missing values 
- Encoded categorical variables using one-hot encoding 
- Created separate datasets for training models (df for MLR, df2 for CatBoost) 

## Models Included 

### 1. Multiple Linear Regression (Main Project Model) 

- Provides a simple and explainable baseline 
- Helps understand how each feature influences car price 
- Trained on df (after cleaning and encoding) 

### 2. CatBoost Regressor (Advanced Model for Comparison) 

- Automatically handles categorical variables 
- Achieved lower prediction error 
- Trained on df2 

## Model Evaluation 

| Model | RMSE | MAE | R² |
|-------|------|-----|----|
| Multiple Linear Regression | 6446 | 4177 | 0.5 |
| CatBoost Regressor | 2297 | 1548 | 0.9 |

*CatBoost performed better than MLR* 

### Feature Importance (CatBoost) 

Bar chart showing how each car feature affects predicted price  
<img width="3000" height="1800" alt="catboost_feature_importance" src="https://github.com/user-attachments/assets/0f0b1671-2543-475b-bd9e-f5b785e481aa" />

## Key Skills Demonstrated 

1. Data cleaning & preprocessing 
2. Handling categorical variables 
3. Building and comparing ML models 
4. Model persistence using joblib 
5. Creating reusable training datasets 
6. Experimenting with modern ML boosting algorithms 

## Future Improvements 

1. Hyperparameter tuning 
2. Feature engineering 
3. Model evaluation dashboard 
4. Deployment using Streamlit or FastAPI
