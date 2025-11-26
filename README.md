# Big Data Customer Churn Prediction Using PySpark

This project uses PySpark to analyze telecom customer churn and build a churn prediction model. The workflow includes data preprocessing, exploratory analysis, and a logistic regression model using Spark MLlib. All steps were executed in Google Colab.

## Dataset
- ~7,000 customer records
- 21 numerical features
- Target column: Churn (0 = No, 1 = Yes)

## Project Goals
- Load and preprocess the dataset using PySpark
- Perform large-scale churn analysis
- Train a logistic regression churn model
- Evaluate model performance
- Identify key factors that influence churn

## Key Insights
- Contract type is the strongest churn indicator:
  - Month-to-month: 42.7% churn
  - One-year: 11%
  - Two-year: 2.8%
- Tenure has a strong loyalty effect:
  - 0–12 months: 48% churn
  - 48+ months: 9.6%
- Streaming and internet-heavy customers churn more
- Customers with TechSupport, OnlineSecurity, and PhoneService churn less

## Model Performance
- Accuracy: 0.807
- ROC-AUC: 0.855

## Feature Importance
Features that increase churn:
- InternetService
- StreamingMovies
- StreamingTV
- PaperlessBilling
- MultipleLines

Features that reduce churn:
- Contract
- PhoneService
- OnlineSecurity
- TechSupport
- Dependents

## Tech Stack
- PySpark
- Spark SQL
- Spark MLlib
- Google Colab
- Python

## How to Run
1. Open the notebook in Google Colab
2. Install PySpark:
```
!pip install pyspark
```
3. Run the notebook cells in order
4. Dataset downloads automatically with wget


