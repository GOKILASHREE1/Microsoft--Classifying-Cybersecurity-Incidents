
# Microsoft: Classifying Cybersecurity Incidents with Machine Learning
# Project Overview
This project focuses on developing a machine learning model to classify cybersecurity incidents as true positive (TP), benign positive (BP), or false positive (FP). By using historical data, the model aims to support Security Operation Centers (SOCs) by automating the triage process, thus improving efficiency and enhancing the security posture of enterprise environments. This classification tool helps SOC analysts prioritize incidents and provide actionable insights for guided responses.

# Skills Demonstrated
Data Preprocessing and Feature Engineering
Machine Learning Classification Techniques
Model Evaluation Metrics (Macro-F1 Score, Precision, Recall)
Cybersecurity Concepts (MITRE ATT&CK Framework)
Handling Imbalanced Datasets
Model Benchmarking and Optimization
# Domain
Cybersecurity
Machine Learning
# Problem Statement
As a data scientist at Microsoft, your task is to enhance the SOC’s efficiency by developing a model that can accurately predict the triage grade of cybersecurity incidents. Utilizing the GUIDE dataset, your objective is to create a robust classification model that categorizes incidents as TP, BP, or FP. This model will support SOC analysts by providing recommendations based on historical evidence and customer responses, ultimately streamlining incident management and response.

# Objective
Train the model using train.csv and evaluate it on test.csv with key metrics—macro-F1 score, precision, and recall—to ensure it performs well on unseen data, making it reliable for real-world applications.

# Business Use Cases
The model developed in this project can be deployed in various cybersecurity applications:

# Security Operation Centers (SOCs): Automate incident triage to help SOC analysts prioritize critical threats.
Incident Response Automation: Provide guided response recommendations for different incident types, reducing threat mitigation times.
Threat Intelligence: Enhance threat detection by incorporating historical data into the classification process, improving TP and FP identification.
Enterprise Security Management: Improve the security posture of organizations by reducing false positives and ensuring critical threats receive prompt attention.
# Approach
1. Data Exploration and Understanding
Initial Inspection: Load train.csv to inspect data structure, feature types, and target distribution (TP, BP, FP).
Exploratory Data Analysis (EDA): Visualize data and use statistical summaries to detect patterns, correlations, and imbalances.
2. Data Preprocessing
Handling Missing Data: Identify and handle missing values using imputation or removal.
Feature Engineering: Create or transform features to improve model accuracy, such as deriving features from timestamps or normalizing numerical variables.
Encoding Categorical Variables: Use techniques like one-hot or label encoding based on feature type and target relationship.
3. Data Splitting
Train-Validation Split: Split train.csv into training and validation sets for model tuning and evaluation.
Stratification: Ensure balanced class distribution using stratified sampling due to target imbalance.
4. Model Selection and Training
Baseline Model: Start with a simple model (e.g., logistic regression or decision tree) as a benchmark.
Advanced Models: Experiment with models such as:
Random Forest
Gradient Boosting Machines (e.g., XGBoost, LightGBM)
Neural Networks
Cross-Validation: Use k-fold cross-validation to evaluate model stability and reduce overfitting risks.
5. Model Evaluation and Tuning
Performance Metrics: Evaluate models using macro-F1 score, precision, and recall to ensure balanced performance.
Hyperparameter Tuning: Fine-tune models with Grid Search or Random Search for optimal performance.
Class Imbalance Handling: Use techniques like SMOTE or class weighting to address imbalanced target classes.
6. Model Interpretation
Feature Importance: Analyze the contribution of features to predictions using SHAP values, permutation importance, or model-specific methods.
Error Analysis: Identify common misclassifications to inform improvements in feature engineering or model complexity.
7. Final Evaluation on Test Set
Testing: Evaluate the final model on test.csv to report macro-F1 score, precision, and recall.
Baseline Comparison: Compare final results with baseline performance to confirm improvements.
8. Documentation and Reporting
Model Documentation: Document each step, including data preprocessing, model selection, and evaluation.
Recommendations: Provide insights on integrating the model into SOC workflows and future improvement areas.
# Results
By the end of the project, the model is expected to:

Accurately classify cybersecurity incidents (TP, BP, FP) with a high macro-F1 score, precision, and recall.
Provide insights into important features that impact classification, enhancing interpretability.
Include comprehensive documentation detailing the approach, challenges faced, and deployment considerations for real-world applications.
# Evaluation Metrics
Macro-F1 Score: Balanced metric considering all classes equally, critical for imbalanced data.
Precision: Ensures accuracy of positive predictions to minimize false positives.
Recall: Measures ability to correctly identify true positives, ensuring critical threats are not missed.
![image](https://github.com/user-attachments/assets/6de1bb3c-a7c7-4800-8cdc-0a42e322df59)
![image](https://github.com/user-attachments/assets/f01ee853-cd65-4107-af62-d475a13e8d42)
![image](https://github.com/user-attachments/assets/bd2fae46-cc1d-4423-a5cf-c5201b7b7e4d)
![image](https://github.com/user-attachments/assets/e79ee304-0b2b-4492-9eb1-b00609a87ed7)
![image](https://github.com/user-attachments/assets/fbe32231-70df-4400-aa14-1b6264c0aad1)
![image](https://github.com/user-attachments/assets/37b183fd-7003-4dd1-84ae-44f5f1d2c4dd)
![image](https://github.com/user-attachments/assets/2951d0dd-34f6-4b6e-94ac-11ea95088b67)
![image](https://github.com/user-attachments/assets/c7d657fd-2df7-471b-8c66-e4aaace722ec)
# Final Recommendations Summary for Cybersecurity:
Add more data to reduce false alarms: Use information like user behavior and device data to help the model make better decisions.
Combine different detection methods: Use multiple security checks to make sure real threats don’t get missed.
Automate low-risk alerts: For harmless activities that look suspicious, let the system handle them automatically so your security team can focus on real threats.
