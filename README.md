# Anomaly Detection System in Blockchain

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0.2-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5.1-orange)
![Numpy](https://img.shields.io/badge/Numpy-1.22.0-yellow)

## Prototype Statement
This project focuses on developing an **Anomaly Detection System** for Blockchain networks, specifically targeting the detection of **51% attacks** in real-time. The system leverages machine learning models such as **Support Vector Machine (SVM)** and **Random Forest Classifier** to identify malicious activities in Bitcoin transaction data.

---

## Abstract / Introduction
With the growing adoption of Blockchain technologies, ensuring the integrity and security of decentralized systems like Bitcoin has become critical. This project proposes an efficient method to identify malicious activity within the Blockchain by analyzing transaction data using machine learning techniques. The solution involves injecting artificial anomalies into a Bitcoin dataset and building machine learning models to detect those anomalies.

---

## Functional Requirements
The system is designed to fulfill the following functional requirements:

1. **Data Loading and Processing**:
   - Load the Bitcoin Blockchain dataset containing transaction data and relevant block information.
   - Preprocess the dataset by cleaning, transforming, and handling missing values or inconsistencies.

2. **Anomaly Injection**:
   - Inject artificial anomalies mimicking a 51% attack into the dataset.
   - Anomalies will affect key features such as:
     - Confirmations: Set anomalous blocks to have zero or unusually low confirmations.
     - Height: Duplicate or irregular block heights.
     - Number of Transactions: Set anomalously high or low transaction volumes in certain blocks.
     - Difficulty: Simulate reduced difficulty in attack scenarios.
     - Timestamps: Create irregular or overlapping timestamps for the blocks.

3. **Anomaly Labeling**:
   - Label the dataset with a binary indicator (`Anomaly` column), where `1` represents an anomalous block and `0` indicates normal blocks.

4. **Machine Learning Model Building**:
   - Implement four machine learning algorithms for anomaly detection:
     - Support Vector Machine (SVM)
     - Random Forest Classifier
     - AdaBoost Classifier
     - XGBoost Classifier
   - Train these models to identify patterns associated with a 51% attack.

5. **Model Evaluation**:
   - Evaluate each model using performance metrics such as:
     - Accuracy
     - Precision
     - Recall
     - F1-score
   - Generate confusion matrices for each model to visualize the distribution of true positives, true negatives, false positives, and false negatives.

6. **Comparison of Models**:
   - Compare the performance of the models and identify the best algorithm based on the evaluation metrics.
   - Visualize the results using bar plots showing the performance metrics for each model.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**:
  - Scikit-learn
  - Matplotlib
  - Numpy
- **Development Environment**: Kaggle, Jupyter Notebook, or Google Colab

---

## Dataset
The dataset used for this project is available on Kaggle:
[Bitcoin Historical On-Chain Data (2014-2024)](https://www.kaggle.com/datasets/arthurgomesbubolz/bitcoin-historical-on-chain-data-2014-2024/data)

---
