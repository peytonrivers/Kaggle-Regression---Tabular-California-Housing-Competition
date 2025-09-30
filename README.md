# Kaggle-Regression---Tabular-California-Housing-Competition
🏡 California Housing Price Prediction (Kaggle Competition)
📌 Overview

This repository contains my solution for the Regression - Tabular California Housing Kaggle competition.
The goal of the competition is to predict median house values using the classic California Housing dataset.

👉 In my first Kaggle competition ever, I achieved 2nd place on the public leaderboard 🥈 with an RMSE of 0.56779.

🚀 Approach
1. Exploratory Data Analysis (EDA)

Explored distributions of key features: MedInc, HouseAge, AveRooms, AveBedrms, Population, AveOccup, Latitude, Longitude.

Engineered new features such as:

rooms_per_person

bedrooms_per_room

pop_per_household

Centered latitude & longitude features

Distance-from-center measures

2. Model Development

I experimented with several machine learning models:

Linear Regression

Random Forest Regressor

XGBoost Regressor

CatBoost Regressor

LightGBM Regressor ✅

After benchmarking, the LightGBM Regressor consistently delivered the best accuracy (lowest RMSE).

3. Final Model

The final model was built with LightGBM Regressor and tuned hyperparameters, including:

Learning rate

Number of leaves

Number of estimators

Subsample and colsample ratios

I also tested feature engineering strategies, target transformations, and cross-validation setups to improve generalization.

🏆 Results

Public Leaderboard: 2nd place 🥈 (RMSE: 0.56779)

Outperformed many other approaches by focusing on:

Strong feature engineering

Cross-validation for stability

Model tuning with LightGBM

🔑 Key Learnings

Feature engineering can matter as much as the model choice.

Cross-validation is critical when Kaggle evaluates on hidden test data.

Ensembling and tuning often bring marginal but important improvements.

LightGBM shines in tabular data competitions.

📈 Next Steps

Try blending LightGBM with CatBoost/XGBoost for additional stability.

Explore spatial clustering features (KMeans on lat/lon).

Build a reproducible pipeline for deployment.

🙌 Acknowledgements

Huge thanks to Kaggle and the competition organizers for providing the dataset. This competition was my first step into the Kaggle world — and achieving 2nd place is just the beginning!
