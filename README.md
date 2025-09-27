Traffic Situation Prediction Using Machine Learning

This project implements and compares three machine learning algorithms — K-Nearest Neighbors (KNN), Decision Trees, and Random Forest — to predict traffic situations based on vehicle counts and temporal features.

📌 Project Overview

Traffic prediction plays a key role in smart city planning, congestion reduction, and efficient transportation management. In this project, we built a traffic situation classifier that predicts one of four classes — heavy, high, low, or normal traffic — using a dataset of 2,976 traffic records.

Our pipeline includes:

Data Cleaning: Duplicate removal, missing value handling, and correction of inconsistent records

Outlier Detection & Removal: Using the IQR method to improve data quality

Feature Engineering: Temporal feature extraction, quantile-based binning, total vehicle count feature

Class Imbalance Handling: SMOTE to generate synthetic samples for minority classes

Feature Scaling: Standardization for better model performance, particularly for KNN

🧠 Machine Learning Models

We implemented and compared three models:

KNN (k=5): Baseline model using majority vote of nearest neighbors

Decision Tree: Simple yet interpretable model with recursive feature-based splits

Random Forest (100 estimators): Ensemble approach for better accuracy and reduced overfitting

📊 Results
Model	Accuracy	Weighted Precision	Weighted Recall
KNN	82.93%	0.86	0.83
Decision Tree	85.34%	0.86	0.85
Random Forest	88.79%	0.89	0.89

Random Forest outperformed the other models, demonstrating the effectiveness of ensemble learning for traffic prediction tasks.

🚀 Future Work

Hyperparameter tuning for further performance gains

Integration of additional features (weather, events, road conditions)

Experimenting with deep learning models (e.g., LSTMs)

Building a real-time traffic prediction dashboard
