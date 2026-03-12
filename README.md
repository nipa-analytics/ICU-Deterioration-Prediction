# ICU-Deterioration-Prediction
ICU Deterioration Risk Prediction using Machine Learning
Early identification of patients at risk of critical deterioration is essential for effective hospital resource management and improved patient outcomes.
This project develops a machine learning model to predict patients at higher risk of ICU utilization using historical hospital data. The model analyzes patient demographics and hospitalization patterns to identify factors associated with critical care needs.
The project also applies Explainable AI techniques, using SHAP, to interpret predictions from the machine learning model trained with XGBoost.

# Business Problem

Hospitals often struggle to anticipate ICU demand. Unexpected ICU admissions can lead to:

Delayed treatment for critically ill patients

Limited ICU bed availability

Increased healthcare costs

Overburdened medical staff

Using predictive analytics, hospitals can identify high-risk patients earlier and allocate resources more effectively.

# Project Objectives

The main goals of this project are:

Analyze hospital patient data to identify ICU utilization patterns

Develop a predictive model for ICU risk

Apply explainable AI techniques to understand model predictions

Provide insights that could support hospital decision-making

# Dataset

# The dataset contains summarized patient-level hospital information, including:

Feature	Description
subject_id	Unique patient identifier
gender	Patient gender
anchor_age	Patient age
total_admissions	Number of hospital admissions
avg_los_days	Average length of hospital stay
unique_diagnoses	Number of unique medical diagnoses
icu_visits	Historical ICU admissions

# A binary target variable icu_risk was created to classify patients with higher ICU utilization risk.

Technology Stack
Category	Tools Used
Programming	Python
Data Processing	Pandas
Database	PostgreSQL
Machine Learning	XGBoost
Explainable AI	SHAP
Visualization	Matplotlib
Machine Learning Workflow
Data Extraction

Patient data was extracted from a PostgreSQL database.

# Data Preparation

# Data cleaning and feature selection were performed to prepare inputs for modeling.

# Feature Engineering

# Relevant features representing patient health complexity and hospital utilization were selected.

# Model Training

A classification model was trained to predict ICU risk.

# Model Explainability

# SHAP values were used to understand feature contributions to predictions.

# Model Insights

# Explainable AI analysis revealed that several variables strongly influence ICU risk predictions:

Hospital Admission History
Patients with multiple hospital admissions tend to have higher ICU utilization.

Length of Stay
Longer hospitalization durations correlate with more severe medical conditions.

Medical Complexity
Patients with more diagnoses often have higher predicted ICU risk.

Age
Older patients generally show increased vulnerability to critical care needs.

Example Visualizations
Feature Importance (SHAP)

Shows which features most strongly influence ICU risk predictions.

# Example insights:

Total admissions strongly influence ICU risk

Longer hospital stays increase predicted risk

Patients with multiple diagnoses show higher ICU utilization

# Business Impact

# If deployed in a hospital environment, this model could help:

Identify high-risk patients earlier

Support ICU capacity planning

Improve patient monitoring strategies

Reduce emergency ICU admissions

# Predictive analytics can help clinicians make more proactive care decisions.

Limitations

# This project is a proof-of-concept model using simplified patient summary data.

# For real-world clinical implementation, additional data such as:

Vital signs

Laboratory results

Real-time patient monitoring .... would be required.
