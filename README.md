# Cricket Performance Prediction
This project applies Machine Learning techniques to predict cricket player performance, with a case study focused on Virat Kohli across all three international formats (T20I, ODI, Test).

# 🔎 Project Overview

Collected and cleaned match-by-match batting data (2010–2025).

Utilized feature engineering predictive features such as:

Rolling averages of runs, strike rate, boundaries.

Encoded opposition, venue (home/away), and match format.

Batting position.

Built and compared three ML models:

Linear Regression

Random Forest Regressor

XGBoost Regressor

Evaluated models using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R².

# 📊 Key Insights

Rolling averages helped capture recent form and improved predictive stability.

Different formats showed unique patterns (e.g., Test form can vary heavily within a series).

XGBoost generally gave the most stable results across formats.

# 🛠️ Tech Stack

Python (pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn)

Jupyter Notebook for experimentation and visualization

# 📈 Visualizations

Predicted vs. Actual scatter plots for each model.

Feature importance charts to highlight impactful predictors.

# 🔄 Retrospection & Learning

Initially included match format (T20, ODI, Test) as a single encoded feature in the dataset.

After experimentation, found this reduced model accuracy since player performance varies drastically across formats.

Adapted by splitting the dataset by format and training separate models, leading to better insights and more interpretable results.

Key takeaway: feature design and dataset organization are as important as model selection.

# 🚀 Future Work

Extend the framework to multiple players (e.g., bowlers).

Add contextual features such as tournament stage or recent series outcomes.

Explore deep learning models for sequence-based predictions.
