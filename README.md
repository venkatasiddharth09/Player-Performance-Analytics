# Cricket Performance Prediction
This project applies Machine Learning techniques to predict cricket player performance, with a case study focused on Virat Kohli across all three international formats (T20I, ODI, Test).

# Project Overview
I collected match-by-match batting performance data of Virat Kohli (2010–2025) using Kaggle and used Excel/Python to clean, transform, and filter data.

Utilized feature engineering predictive features such as:
   Rolling averages of runs, strike rate, boundaries (4s/6s).
   Encoded opposition, venue (home/away), and match format.
   Batting position.
   
Built and compared three ML models:
   Linear Regression
   Random Forest Regressor
   XGBoost Regressor

Evaluated model efficiency and accuracy using MAE (Mean Absolute Error), MSE (Mean Squared Error), RMSE (Root Mean Squared Error), and R².

# Key Insights
   Rolling averages helped capture recent form and improved predictive stability of the statistics.
   Different formats showed unique patterns (e.g., Test form can vary heavily within a series).
   XGBoost and RandomForestRegressor generally gave the most stable results across formats.

# Tech Stack Utilized
   Python (pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn)
   Jupyter Notebook for experimentation and visualization

# Visualizations
   Predicted vs. Actual scatter plots for each model.
   Feature importance charts to highlight impactful predictors.
