# Cricket Performance Prediction using ML Models

**Machine Learning project** predicting Virat Kohli’s match-by-match batting performance across T20, ODI, and Test formats (2010–2025) using rolling averages, opposition, venue, and other key features. Compared Linear Regression, Random Forest, and XGBoost models to identify the most accurate predictor of runs scored and successfully predicted runs scored in future matches using testing data.

# 🔎 Project Overview

Collected and cleaned match-by-match batting data (2010–2025) using Kaggle and Python/Excel.

**Engineered predictive features** including rolling averages of runs, strike rate, boundaries (4s/6s), and encoded opposition, venue (home/away), and match format.

Built and compared **Linear Regression, Random Forest Regressor, and XGBoost Regressor** models.

Evaluated models using **MAE, MSE, RMSE, and R²** metrics.

# 📊 Key Insights

Rolling averages captured recent form, improving predictive stability.

Models performed well for **T20s and ODIs**; Test match predictions were less stable due to the format’s variability and fluctuating player form.

**XGBoost and Random Forest** generally produced the most consistent results across formats.

# 🛠️ Tech Stack

**Python** (pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn)

**Jupyter Notebook** for experimentation and visualization

# 🔧 Model Optimization

Used **GridSearchCV** to systematically search over parameter grids for Random Forest Regressor.

Tuned hyperparameters: **n_estimators, max_depth, min_samples_split, min_samples_leaf, learning_rate, etc.**

Implemented a custom manual function to tune hyperparameter combinations for XGBoost, ensuring robust model selection.

# 📈 Visualizations

Predicted vs. Actual scatter plots for each model.

Feature importance charts highlighting the most impactful predictors.

# 🔄 Retrospection

Initially used match format (T20, ODI, Test) as a single encoded feature to train the model. However, I found that this feature reduced model accuracy because player performance varied drastically across formats.

Adapted by splitting datasets by format and training separate models, leading to more interpretable and accurate results.

Key takeaway: Feature design and dataset organization are as important as model selection.

# 🚀 Future Work

Extend the framework to multiple players (bowlers, batters, all-rounders).

Incorporate additional contextual features like tournament stage, recent series outcomes, pitch type, bowling strength, match pressure.

Explore deep learning models for sequence-based predictions.
