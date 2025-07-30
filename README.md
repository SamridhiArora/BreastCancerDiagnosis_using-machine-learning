🧠 Machine Learning-Based Diagnosis of Breast Cancer Using Feature Optimization
A comprehensive machine learning project implementing and comparing 11 classification algorithms for early and accurate detection of breast cancer using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset. The approach replicates and extends the methodology from the research paper:
📄 "Machine learning-based diagnosis of breast cancer utilizing feature optimization technique" by Uddin et al. (2023).

📊 Project Overview
Breast cancer is a leading cause of mortality among women. Early detection is critical. This project explores the use of ML models to classify tumors as benign or malignant based on clinical measurements derived from biopsy samples.

Key steps:

Dataset Cleaning & Visualization

Feature Optimization using PCA

Model Building with GridSearchCV & Cross-Validation

Evaluation (Accuracy, Precision, Recall, F1-Score)

ROC Curve Analysis

Final Deployment using Gradio

🧬 Dataset
Source: UCI Machine Learning Repository

Samples: 569 breast tumor records

Features: 30 real-valued numeric features

Target: Diagnosis (M for Malignant, B for Benign) — encoded to binary 0 and 1.

⚙️ Methodology
Two parallel pipelines were implemented:

Raw Model Pipeline — Models trained on original dataset.

Optimized Pipeline — Models trained on PCA-reduced data (16 components) after StandardScaler normalization.

PCA retained 98.7% of the variance with just 16 components.

🤖 Models Implemented
The following 11 machine learning models were tuned and evaluated:

Logistic Regression

Support Vector Machine (SVM)

K-Nearest Neighbors (KNN)

Decision Tree

Random Forest

Naive Bayes

AdaBoost

Gradient Boosting

Multi-Layer Perceptron (MLP)

Nearest Centroid

Voting Classifier (SVM + Logistic Regression)

🧪 Model Evaluation
All models were tuned using GridSearchCV with 10-fold cross-validation, optimized for F1 Score.

Metrics used:

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

ROC Curve & AUC

✅ The Voting Classifier demonstrated the best performance with ~98.6% accuracy.

🌐 Deployment
The Voting Classifier was deployed using Gradio to create an interactive web app that predicts diagnosis based on 15 tumor features.
