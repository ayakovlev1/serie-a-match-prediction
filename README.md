# serie-a-match-prediction
Explainable Serie A Match Prediction

This project is a football analytics and machine learning project focused on predicting Serie A match outcomes using recent team form and interpretable statistical features.

The objective is not betting optimization or black-box prediction, but building a transparent football analytics pipeline using historical match data and rolling performance indicators.

The project predicts:
- Home Win (H)
- Draw (D)
- Away Win (A)

Main features include:
- average goals scored,
- average goals conceded,
- average points,
- shots,
- shots on target,
- recent home performance,
- recent away performance.

Rolling features are created only from previous matches in order to avoid data leakage.

Examples of engineered features:
- home_avg_goals_5
- away_avg_goals_5
- home_avg_points_5
- away_avg_points_5
- home_avg_shots_5
- away_avg_shots_5
- home_home_points_5
- away_away_points_5

The project currently uses Logistic Regression because it is simple, interpretable and appropriate for an educational football analytics project.

The dataset is split chronologically rather than randomly because football data is temporal and future matches should not influence past predictions.

Current model accuracy is approximately 44-45%, which is realistic for a simple football prediction model without betting odds, injuries or tactical information.

Project structure:

Serie_A_Forecast/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_feature_engineering.ipynb
│   ├── 02_model_training.ipynb
│   └── 03_match_predictions.ipynb
│
├── models/
│
├── outputs/
│
└── README.md

The project was developed and tested using Google Colab and Google Drive.

Main libraries:
- pandas
- numpy
- scikit-learn
- joblib

Data source:
https://www.football-data.co.uk/

This project is intended for educational and portfolio purposes only.

The model does not use:
- betting odds,
- injuries,
- lineups,
- tactical analysis,
- advanced tracking data.

Football is highly unpredictable and predictions should not be interpreted as betting advice.

Author:
Alexander Yakovlev
Applied Data Science Graduate
Football Analytics & Data Visualization Enthusiast
