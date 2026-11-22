CompareClassifier

Comparing the performance of four classification models (K-Nearest Neighbors, Support Vector Machine, Decision Tree and Logistic Regression) on marketing data from a Portuguese bank.

Overview

This repository analyzes data a Portuguese banking institution collected during its direct marketing campaigns for term (fixed) deposits. The goal is to predict whether a client will subscribe to a term deposit, and to find out which classification model does this best.

The project follows the full CRISP-DM (Cross-Industry Standard Process for Data Mining) lifecycle, from understanding the business problem to evaluating the final models.

Dataset
Source: UCI Machine Learning Repository: Bank Marketing
Content: Client attributes (age, job, marital status, education and so on), details of the last contact in the current campaign, results of previous campaigns, and social and economic indicators.
Target variable: y, which records whether the client subscribed to a term deposit (yes / no).
Methodology: CRISP-DM
Business Understanding: Define the goal of predicting which clients are likely to subscribe, so the bank can target its marketing more efficiently.
Data Understanding: Explore the dataset, its features, distributions, missing or "unknown" values, and the class imbalance in the target.
Data Preparation: Clean the data, encode categorical features, scale numerical features and split the data into training and test sets.
Modeling: Train and tune the four classifiers listed below.
Evaluation: Measure and compare how well each model performs.
Deployment / Recommendations: Summarize the findings and recommend a model and next steps.
Models Used
Model	Description
K-Nearest Neighbors (KNN)	Classifies a client by the majority class of the most similar clients
Support Vector Machine (SVM)	Finds the boundary that best separates the two classes
Decision Tree	Learns a set of if/then rules from the features
Logistic Regression	Models the probability that a client subscribes
Evaluation

Each model is evaluated and compared on:

Training time
Training and test accuracy
Precision, Recall and F1-score
Confusion matrix
ROC curve and AUC
Visualizations

The project includes visualizations to support both the data exploration and the model comparison, such as:

Feature distributions and the balance of the target classes
Correlation heatmap
Confusion matrices for each model
ROC curves comparing all models
Bar charts comparing model accuracy and training time
Repository Structure
CompareClassifier/
├── data/                  # Bank marketing dataset
├── images/                # Saved charts and plots
├── CompareClassifier.ipynb  # Main Jupyter notebook
└── README.md
Getting Started
Prerequisites
Python 3.x
Jupyter Notebook
pandas, numpy, matplotlib, seaborn, scikit-learn
Acknowledgments

The dataset is from: [Moro et al., 2014] S. Moro, P. Cortez. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014.
