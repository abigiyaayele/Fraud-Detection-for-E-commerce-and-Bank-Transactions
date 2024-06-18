# Fraud Detection for E-commerce and Bank Transactions

## Project Summary
This project aims to improve the detection of fraud cases in e-commerce transactions and bank credit transactions using advanced machine learning models. By leveraging detailed data analysis, feature engineering, and geolocation analysis, we aim to create robust fraud detection models that can be deployed for real-time monitoring and reporting. This initiative will enhance transaction security, prevent financial losses, and build trust with customers and financial institutions.

## Overview
Adey Innovations Inc., a leading company in the financial technology sector, is committed to providing cutting-edge solutions for e-commerce and banking. This project focuses on developing and deploying machine learning models to detect fraudulent activities in transaction data. The models will be trained on two datasets: one containing e-commerce transactions and another containing bank credit transactions. The project also involves deploying these models using Flask and Docker to enable real-time fraud detection.

## Introduction
Fraud detection is critical for ensuring the security and integrity of financial transactions. E-commerce and banking sectors are particularly vulnerable to fraudulent activities, which can lead to significant financial losses and damage to customer trust. By developing sophisticated fraud detection systems, Adey Innovations Inc. aims to enhance the security of transactions and provide reliable protection against fraud.

## Objectives
- **Data Analysis and Preprocessing**: Analyze and preprocess transaction data to prepare it for model training.
- **Feature Engineering**: Create and engineer features that help in identifying fraud patterns.
- **Model Building and Training**: Build and train various machine learning models to detect fraud.
- **Model Evaluation**: Evaluate the performance of the models and make necessary improvements.
- **Model Explainability**: Use SHAP and LIME to interpret and explain the models' predictions.
- **Model Deployment**: Deploy the models for real-time fraud detection using Flask and Docker.
- **API Development**: Create REST APIs to serve the models and enable real-time prediction serving.

## Learning Outcomes
### Skills
- **Deploying machine learning models using Flask**
- **Containerizing applications using Docker**
- **Creating REST APIs for machine learning models**
- **Testing and validating APIs**
- **Developing end-to-end deployment pipelines**
- **Implementing scalable and portable machine-learning solutions**

### Knowledge
- **Principles of model deployment and serving**
- **Best practices for creating REST APIs**
- **Understanding of containerization and its benefits**
- **Techniques for real-time prediction serving**
- **Security considerations in API development**
- **Methods for monitoring and maintaining deployed models**

## Tasks and Steps

###  - Data Analysis and Preprocessing
1. **Handle Missing Values**
   - Impute or drop missing values.
2. **Data Cleaning**
   - Remove duplicates.
   - Correct data types.
3. **Exploratory Data Analysis (EDA)**
   - Univariate analysis.
   - Bivariate analysis.
4. **Merge Datasets for Geolocation Analysis**
   - Convert IP addresses to integer format.
   - Merge `Fraud_Data.csv` with `IpAddress_to_Country.csv`.
5. **Feature Engineering**
   - Transaction frequency and velocity for `Fraud_Data.csv`.
   - Time-based features for `Fraud_Data.csv` (e.g., hour_of_day, day_of_week).
6. **Normalization and Scaling**
7. **Encode Categorical Features**

### - Model Building and Training
1. **Data Preparation**
   - Feature and target separation [‘Class’ (creditcard), ‘class’ (Fraud_Data)].
   - Train-Test Split.
2. **Model Selection**
   - Compare performance of various models: Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, MLP, CNN, RNN, LSTM.
3. **Model Training and Evaluation**
   - Training models for both credit card and fraud-data datasets.
4. **MLOps Steps**
   - Versioning and Experiment Tracking using tools like MLflow.

###  - Model Explainability
1. **Using SHAP for Explainability**
   - Install SHAP: `pip install shap`.
   - Generate SHAP plots (Summary Plot, Force Plot, Dependence Plot).
2. **Using LIME for Explainability**
   - Install LIME: `pip install lime`.
   - Generate LIME plots (Feature Importance Plot).

### - Model Deployment and API Development
1. **Setting Up the Flask API**
   - Create the Flask application.
   - Define API endpoints.
   - Test the API.
2. **Dockerizing the Flask Application**
   - Create a Dockerfile.
     ```Dockerfile
     # Use an official Python runtime as a parent image
     FROM python:3.8-slim

     # Set the working directory in the container
     WORKDIR /app

## Author: Abigiya Ayele.
     

     # Copy the current directory contents into the container at /app
     COPY . .

     # Install any needed packages specified in requirements.txt
     RUN pip install -
