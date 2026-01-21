Supply Chain Spoilage Prediction Using Machine Learning
Project Overview

This project focuses on predicting product spoilage risk in supply chain transportation using supervised machine learning techniques. The objective is to build and evaluate classification models that can identify high-spoilage scenarios based on transportation, environmental, and operational factors.

The project follows a complete analytics lifecycle, including data preprocessing, exploratory data analysis, feature engineering, class imbalance handling, model training, evaluation, and interpretation.

Problem Statement

In supply chain logistics, spoilage leads to significant financial losses, especially for perishable goods. Factors such as transportation duration, temperature control, humidity, handling delays, and vehicle capacity directly influence spoilage risk.

Traditional rule-based monitoring systems fail to capture complex, non-linear relationships among these variables. This project addresses the problem by applying machine learning models to accurately classify spoilage risk and support proactive decision-making.

Objectives

Clean and preprocess real-world supply chain data

Perform exploratory data analysis to understand spoilage patterns

Handle class imbalance using resampling techniques

Build and compare multiple classification models

Evaluate models using robust performance metrics

Identify key features contributing to spoilage risk

Dataset Description

The dataset contains detailed transportation and logistics information related to product movement across the supply chain.

Key attributes include:

Product category and quantity

Transportation method

Vehicle type and capacity

Distance traveled

Delivery frequency and trip duration

Temperature and humidity maintenance

Storage and handling delays

Total delivery time and cost

Spoilage percentage (used to derive the target variable)

The target variable represents high spoilage risk, derived from spoilage percentage using a defined threshold.

Tools and Technologies

Python

Google Colab

Pandas and NumPy

Matplotlib and Seaborn

Scikit-learn

Imbalanced-learn (SMOTE)

Methodology
Data Preprocessing

Missing values handled using statistical imputation

Outliers assessed and managed where necessary

Categorical variables encoded using appropriate encoding techniques

Numerical features scaled using StandardScaler

Target variable created by binarizing spoilage percentage

Exploratory Data Analysis

Target distribution analysis to assess class imbalance

Descriptive statistics of numerical variables

Correlation analysis between operational variables and spoilage risk

Visual analysis of key features influencing spoilage

Class Imbalance Handling

The dataset exhibited significant class imbalance

Synthetic Minority Over-sampling Technique (SMOTE) was applied

Balanced training data improved model learning and recall for minority class

Models Implemented

The following classification models were trained and evaluated:

Logistic Regression

Support Vector Machine (SVM)

Decision Tree Classifier

K-Nearest Neighbors (KNN)

Random Forest Classifier

XGBoost Classifier

Each model was trained on scaled and balanced data for fair comparison.

Model Evaluation

Models were evaluated using multiple performance metrics:

Accuracy

Precision

Recall

F1-score

ROC-AUC score

Confusion Matrix

Cross-validation was also applied to assess model stability and generalization.

Key Insights

Tree-based models demonstrated superior performance on spoilage prediction

Random Forest and XGBoost achieved the highest accuracy and ROC-AUC scores

Environmental factors such as temperature maintenance and delivery duration were strong predictors of spoilage

SMOTE significantly improved recall for high-spoilage cases

Feature importance analysis highlighted operational delays as critical risk drivers

Business Implications

Enables early identification of high-risk spoilage shipments

Supports optimization of transportation planning and cold-chain management

Reduces financial losses by enabling proactive interventions

Applicable to food supply chains, pharmaceuticals, and perishable goods logistics

Limitations

Model performance depends on data quality and threshold selection

External factors such as weather conditions are not explicitly modeled

Real-time prediction would require system integration

Future Scope

Integration with real-time IoT sensor data

Deployment as a predictive monitoring dashboard

Cost-sensitive learning for spoilage risk prioritization

Expansion to multi-class spoilage severity prediction

Author

Parv
