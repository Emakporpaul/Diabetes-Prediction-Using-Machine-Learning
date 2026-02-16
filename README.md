# Diabetes-Prediction-Using-Machine-Learning

🧠 Diabetes Prediction using Machine Learning

This project builds a machine learning model to predict the likelihood of diabetes based on clinical health indicators such as glucose level, BMI, age, and insulin.

The goal is to support early risk screening and preventive healthcare decisions.

📊 Problem Statement

Diabetes is a chronic disease that often goes undiagnosed until complications appear. Early identification of high-risk individuals can enable timely lifestyle changes and medical intervention.

This project applies supervised machine learning to predict diabetes risk from patient health measurements.

📁 Dataset

The dataset contains medical diagnostic variables for female patients, including:

Pregnancies

Glucose

Blood Pressure

Skin Thickness

Insulin

BMI

Diabetes Pedigree Function

Age

Outcome (0 = Non-diabetic, 1 = Diabetic)

⚙️ Feature Engineering

Additional categorical health risk features were created:

BMI categories (Underweight, Overweight, Obesity levels)

Glucose risk levels

Insulin score classification

Missing values in medical variables were imputed using class-wise medians.

🤖 Model

Algorithm: XGBoost Classifier

Reasons for selection:

Handles nonlinear relationships

Robust to feature interactions

High performance on tabular medical data

📈 Model Performance

Metrics used:

Accuracy

Precision

Recall

F1-score

The model demonstrates strong ability to identify diabetic patients, making it suitable for early-screening support tools.

🔍 Feature Importance

The most influential predictors include:

Glucose

BMI

Age

Insulin

These align with established medical risk factors for diabetes.
