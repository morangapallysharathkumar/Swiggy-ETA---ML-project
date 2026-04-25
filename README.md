# Swiggy-ETA---ML-project

Swiggy Delivery Time (ETA) Prediction

Project Overview
As one of India's largest food delivery platforms, Swiggy handles millions of daily orders. Providing an accurate Estimated Time of Arrival (ETA) is critical for customer satisfaction and operational efficiency. This project utilizes machine learning to predict delivery times based on various real-world factors such as distance, traffic, weather, and rider conditions.

Business Problem
Inaccurate ETA predictions lead to:
Order cancellations 
Customer dissatisfaction 
Increased operational costs 


Objective

The primary goal is to build a robust regression model to predict delivery time (in minutes) accurately. By optimizing ETA, the project aims to reduce cancellations and enhance the overall user experience.

Dataset Summary
Total Records: 45,502
Total Features: 26 (including Rider Age, Ratings, Weather, Traffic, Latitude/Longitude, etc.)
Target Variable: Delivery Time (minutes) 

Methodology: CRISP-ML(Q)
The project follows the CRISP-ML(Q) framework to ensure a structured machine learning lifecycle:

Business & Data Understanding: Defining KPIs and verifying data feasibility.
Data Engineering: Cleaning, transforming, and preparing raw data.
Model Building: Algorithm selection and hyperparameter tuning.
Model Evaluation: Validating performance against business goals.
Model Deployment: Integrating the model into a production environment.
Monitoring & Maintenance: Tracking performance and detecting drift.

Data Preprocessing Pipeline:
To prepare the data for modeling, the following steps were implemented:
Missing Values: Handled using SimpleImputer.
Categorical Encoding: One-Hot Encoding for nominal data and Ordinal Encoding for ranked data.
Feature Scaling: Applied StandardScaler to numerical features.
Data Split: 80/20 train-test split.

Model Building & Evaluation
Several regression algorithms were tested to find the most accurate predictor:
Linear Regression
KNN Regressor 
Decision Tree
Random Forest 
Gradient Boosting 
SVR 
XGBoost Regressor (Best Performer) 

Performance Metrics (XGBoost):
After GridSearchCV hyperparameter tuning and 5-Fold Cross Validation, the final model achieved:
R² Score: 0.8161 
RMSE: 4.043 
MAE: 3.219

Deployment:

The final model is deployed as a web application using Streamlit and is hosted on Hugging Face Spaces.
Live Demo: Link to Hugging Face Space 

Future Applications
The insights and models from this project can be extended to:
E-commerce delivery tracking (Amazon, Flipkart).
Emergency services (Ambulance arrival time).
Urban transportation planning and traffic pattern analysis.

Author 
M. Sharath Kumar

LinkedIn: [https://www.linkedin.com/feed/update/urn:li:activity:7453692647094976512/]
