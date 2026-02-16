# Diabetes-Prediction-Using-Machine-Learning

This project builds a machine learning model to predict the likelihood of diabetes based on clinical health indicators, including glucose levels, BMI, age, and insulin levels.

The goal is to support early risk screening and preventive healthcare decisions.

# Problem Statement

Diabetes is a chronic disease that often goes undiagnosed until complications appear. Early identification of high-risk individuals can enable timely lifestyle changes and medical intervention.

This project applies supervised machine learning to predict diabetes risk from patient health measurements.

# Dataset

The dataset contains medical diagnostic variables for female patients, including:

1. Pregnancies
2. Glucose
3. Blood Pressure
4. Skin Thickness
5. Insulin
6. BMI
7. Diabetes Pedigree Function
8. Age
9. Outcome (0 = Non-diabetic, 1 = Diabetic)

# Feature Engineering

Some categorical health risk features were created:

1. BMI categories (Underweight, Overweight, Obesity levels)
2. Glucose risk levels
3. Insulin score classification

Missing values in medical variables were imputed using class-wise medians.

# Model

#### Algorithm: XGBoost Classifier

#### Reasons for selection:

i. Handles nonlinear relationships
ii. Robust to feature interactions
iii. High performance on tabular medical data

# Model Performance

Metrics used:

1. Accuracy
2. Precision
3. Recall
4. F1-score

The model demonstrates a strong ability to identify diabetic patients, making it suitable for early screening support tools.

# Feature Importance

The most influential predictors are:

1. Glucose
2. BMI
3. Age
4. Insulin

These align with established medical risk factors for diabetes.

# Example of My Prediction

#### Input patient data:
Pregnancies: 2  
Glucose: 150  
BloodPressure: 80  
SkinThickness: 30  
Insulin: 130  
BMI: 33.5  
DPF: 0.45  
Age: 52

#### Model Output:
Prediction: Diabetic
Risk Probability: 0.88





from xgboost import plot_importance
import matplotlib.pyplot as plt

plot_importance(xgb)
plt.savefig("images/feature_importance.png")
plt.show()
