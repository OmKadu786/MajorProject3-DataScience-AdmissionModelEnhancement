📘 Overview

This project extends the Admission Prediction Problem (previously implemented with Logistic Regression) by applying advanced modeling and optimization techniques to improve predictive accuracy.
The goal is to predict whether a student will be admitted to a university based on features such as GRE score, GPA, and rank, while exploring polynomial regression and ensemble learning for accuracy improvement.

🎯 Objective

To enhance the accuracy and reliability of the admission prediction model using advanced machine learning techniques such as Polynomial Regression, Random Forest Regressor, and Gradient Boosting Regressor.

🧩 Dataset

File: College_admission.csv
Target Variable: admit (1 = Admitted, 0 = Not Admitted)
Key Features
| Feature | Description                                           |
  | ------- | ----------------------------------------------------- |
  | `GRE`   | Graduate Record Examination score                     |
  | `GPA`   | Grade Point Average                                   |
  | `Rank`  | Prestige of the applicant’s undergraduate institution |
  | `Admit` | Admission decision (target)                           |

⚙️ Workflow
1. Data Loading & Exploration
  Load dataset using pandas and examine structure.
  Check for missing values and data types.
  Display summary statistics using describe().
  Visualize data distribution with:
  Countplots for admission rates.
  Pairplots for feature interactions.
  Correlation Heatmap to identify relationships.

2. Baseline Model — Logistic Regression
  Train a Logistic Regression model for binary classification.
  Evaluate performance using:
  Accuracy
  Confusion Matrix
  Classification Report
  Cross-validation accuracy
  Measure baseline metrics:
  RMSE, MAPE, and R²

🚀 Model Enhancement Techniques

A. Polynomial Regression (Degree = 3)
  Generate higher-degree polynomial features to capture non-linear relationships.
  Apply feature scaling using StandardScaler.
  Fit and evaluate the model to check improvement in predictive accuracy.

B. Random Forest Regressor
  Apply ensemble learning using multiple Decision Trees.
  Parameters used:
    n_estimators = 180
    max_features = 'sqrt'
    random_state = 42
    Aggregates predictions to improve accuracy and reduce overfitting.

C. Gradient Boosting Regressor
  Sequentially builds trees to correct previous errors.
  Parameters:
    n_estimators = 250
    learning_rate = 0.05
    subsample = 0.8
    Excellent at capturing complex feature interactions.
