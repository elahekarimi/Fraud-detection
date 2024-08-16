# Fraud Detection Using XGBoost

## Overview

This repository contains a machine learning project aimed at detecting fraudulent transactions using XGBoost. The project involves data preprocessing, model training, evaluation, and visualization of performance metrics. The goal is to build a robust model that can effectively identify fraudulent activities based on various features.

## Table of Contents

1.  [dataset](#dataset)
2.  [Project Description](#project-description)
3. [Features](#features)
4. [Setup and Installation](#setup-and-installation)
5. [Usage](#usage)
6. [Data](#data)
7. [Model Evaluation](#model-evaluation)
8. [Visualizations](#visualizations)
9. [Contributing](#contributing)
10. [License](#license)


## Dataset
The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise
## Project Description

This project utilizes the XGBoost algorithm to classify transactions as fraudulent or regular. It includes the following steps:
- Data preprocessing: Handling missing values, outlier removal, and feature selection.
- Model training: Building and training an XGBoost classifier.
- Model evaluation: Assessing model performance using metrics such as accuracy, precision, recall, and AUC.
- Visualization: Plotting performance metrics and distribution of features.

## Features

- **Data Preprocessing**: Includes outlier detection and handling, missing value imputation.
- **Model Training**: XGBoost classifier for fraud detection.
- **Evaluation Metrics**: Accuracy, precision, recall, ROC AUC, and precision-recall curves.
- **Visualizations**: Boxplots, distribution plots, confusion matrix.

## Setup and Installation

To get started with this project, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/fraud-detection-xgboost.git
   cd fraud-detection-xgboost


Model Evaluation
The model is evaluated using several metrics:

Accuracy: Proportion of correctly classified instances.
Precision and Recall: Performance measures for the positive class.
AUC-ROC Curve: Performance measure for binary classification.
Confusion Matrix: Visualization of true vs. predicted labels.
Visualizations
This project includes various visualizations to understand model performance and data distributions:

Boxplots: Visualize the distribution of features.
Distribution Plots: Show the distribution of transaction amounts and other features.
Confusion Matrix: Assess the number of true positives, false positives, true negatives, and false negatives.
