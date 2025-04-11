## Overview
This project focuses on forecasting game outcomes for the 2025 NCAA Men’s Basketball Tournament by predicting win probabilities for all possible team matchups. Historical game data, advanced basketball metrics, and machine learning techniques were used to build a model capable of evaluating each team’s performance. The work included data preparation, feature engineering, model training, and generating a formatted prediction file for tournament evaluation.

## Objectives
The main objectives of this project were to:

Predict the win probability for any potential matchup in the 2025 NCAA Men’s Tournament.

Engineer key game-level features such as efficiency, shooting accuracy, and turnovers.

Analyze the impact of historical performance, seeding, and head-to-head records.

Evaluate model performance using appropriate metrics and submit predictions.

Tools and Technologies Used
Python: Used for data cleaning, feature engineering, modeling, and evaluation.

Pandas & NumPy: Employed for data manipulation and statistical calculations.

Scikit-learn & XGBoost: Used to build and evaluate machine learning models.

SHAP: Applied for model interpretability and feature importance analysis.

Matplotlib & Seaborn: Utilized for visualizing distributions and outliers.

## Key Features Engineered
True Shooting Percentage (TS%): Captures overall shooting efficiency.

Effective FG% and Turnover %: Key predictors for offensive and defensive strength.

Rebounding % and Net Efficiency: Evaluated team dominance across the court.

Seed Difference: Reflects expected advantage based on seeding.

Head-to-Head Win % (with Laplace Smoothing): Captures matchup history.

Rolling Averages (5 & 20 games): Represent recent team form.

Project Workflow
Data Collection & Cleaning: Loaded NCAA datasets, checked consistency, and merged historical records.

Feature Engineering: Computed advanced basketball metrics and handled outliers.

Matchup Generation: Created all possible 2025 tournament matchups using team combinations.

Model Training: Trained XGBoost and Random Forest classifiers; evaluated using Brier Score, AUC, and accuracy.

Model Interpretation: Used SHAP to analyze feature impact on prediction results.

Prediction Generation: Predicted win probabilities for all matchups and formatted results for submission.

## Results
The final model generated win probabilities for over 1,000 possible matchups in the 2025 NCAA Men’s Tournament. Key findings included:

Teams with stronger rolling averages in Net Efficiency and TS% had higher win probabilities.

Seed Difference and historical head-to-head performance significantly influenced outcomes.

The model showed strong performance with competitive Brier Score and AUC values, indicating reliable probability estimates.

## Conclusion
This project demonstrates the application of machine learning in sports analytics, combining statistical metrics with real-world game data. It highlights how predictive modeling and feature engineering can offer valuable insights into team performance and tournament outcomes. The final output supports data-driven decision-making for analysts, fans, and tournament stakeholders.

