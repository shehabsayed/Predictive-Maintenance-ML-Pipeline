# Predictive-Maintenance-ML-Pipeline

  This project implements a machine learning pipeline for predictive maintenance classification. It handles multiple leakage scenarios to evaluate model robustness.

- Overview

    - Goal: Predict machine failures using sensor data.

    - Models: Logistic Regression and XGBoost.

    - Scenarios:

          - No Leak – Only real features.

          - Failure Type Leak (FTL) – Includes a leaking feature.

          - Future Info Leak (FIL) – Simulates future data leakage.

- Features

  - Automatic data cleaning and preprocessing.

  - Handles numerical and categorical features.

  - SMOTETomek for class imbalance.

  - GroupKFold cross-validation to respect product groups.

  - Hyperparameter tuning with GridSearchCV.

  - Model evaluation using classification metrics, ROC curves, and confusion matrices.

  - SHAP feature importance analysis for model interpretability.

 - Data
 
    - Sensor measurements: Air temperature, Process temperature, Rotational speed, Torque, Tool wear.

    - Categorical feature: Type.

    - Target: Machine failure (0/1).

    - Product ID used for grouping.

- Results

  - Models are evaluated across all leakage scenarios.

  - Visualizations include class distributions, correlations, ROC curves, confusion matrices, and SHAP summaries.

  - Provides insights on feature importance and model robustness under different leakage scenarios.

