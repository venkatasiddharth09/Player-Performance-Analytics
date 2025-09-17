# Cricket Performance Prediction

Machine Learning project predicting Virat Kohli’s match-by-match batting performance across T20, ODI, and Test formats (from 2010–2025) using rolling averages of numerical data, opposition, venue, and other features. 
Compared Linear Regression, Random Forest, and XGBoost models to observe which model works the best in accurately predicting the runs scored.

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

# 🔧 Model Optimization

Used GridSearchCV to systematically search over parameter grids for Random Forest Regressor.

Tuned key hyperparameters such as n_estimators, max_depth, min_samples_split, min_samples_leaf, and learning_rate.

Implemented a custom manual function to test specific parameter combinations for XGBoost Regression Model and compare RMSE, ensuring robustness in model selection.

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
