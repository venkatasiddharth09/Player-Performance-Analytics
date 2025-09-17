# Cricket Performance Prediction
This project applies Machine Learning techniques to predict cricket player performance, with a case study focused on Virat Kohli across all three international formats (T20I, ODI, Test).

# 🔎 Project Overview

Collected and cleaned match-by-match batting data (2010–2025) using Kaggle and Excel/Python.

**Utilized feature engineering predictive features such as** caluclating rolling averages of runs, strike rate, boundaries (4s/6s), and encoding opposition, venue (home/away), and match format.

**Built and compared three ML models:** Linear Regression, Random Forest Regressor, XGBoost Regressor

Evaluated models using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R².

# 📊 Key Insights

Rolling averages helped capture recent form of the player and improved predictive stability.

The model was efficient in predicting results or scores in T20s and ODIs, while it had a hard time predicting close to the runs for Tests. This is because Tests format is extremely versatile and the player statistics show that he has been on and off in his batting form throughout his career within this format.

**XGBoost and RandomForest** Regressor generally gave the most stable results across formats.

# 🛠️ Tech Stack

Python (pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn)

Jupyter Notebook for experimentation and visualization of models.

# 📈 Visualizations

Predicted vs. Actual scatter plots for each model.

Feature importance charts to highlight impactful predictors.

# 🔄 Retrospection

Initially included match format (T20, ODI, Test) as a single encoded feature in the dataset.

After experimentation, I found that the formats had partially reduced model accuracy since player performance varied drastically across formats.

Therefore, I adapted by splitting the dataset by format in Excel and training separate models for each dataset, leading to better insights and more interpretable results.

Key takeaway: feature design and dataset organization are as important as model selection.

# 🚀 Future Work/Steps

Extend the framework to multiple players (e.g., bowlers, batters, all-rounders).

Add other contextual features such as tournament stage, recent series outcomes, pitch type, bowling strength, match pressure, etc. for better predictivity and model training.

Explore deep learning models for sequence-based predictions.
