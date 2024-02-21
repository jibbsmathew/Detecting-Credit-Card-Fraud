# Detecting-Credit-Card-Fraud

## Credit Card Fraud Detection

This repository contains code for detecting fraudulent credit card transactions using machine learning models. The models are built using a public dataset obtained from Kaggle, which can be found [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

### Data Overview

The dataset comprises 284,807 transactions, each characterized by 30 numeric features. These features are PCA transformed to maintain confidentiality. Additionally, there's a target class indicating whether a transaction is fraudulent or not.

It's important to note that the dataset is highly imbalanced, with only 0.17% of transactions labeled as fraudulent. For privacy reasons, no detailed feature information is provided, except for the 'Time' and 'Amount' columns, which remain untouched.

### Analysis Steps

The analysis involves the following key steps:

1. **Data Exploration**: Understanding the distributions, correlations, and identifying anomalies.
   
2. **Handling Class Imbalance**: Employing techniques like undersampling and oversampling to address the class imbalance issue.

3. **Modeling**: Utilizing various algorithms including Logistic Regression, Random Forest, and XGBoost.

4. **Model Evaluation**: Assessing model performance primarily using the AUC-ROC metric due to the dataset's imbalance.

5. **Anomaly Detection**: Leveraging Isolation Forest to identify potential outliers.

6. **Feature Engineering**: Introducing new features such as moving averages over time to enhance fraud detection capabilities.

### Key Observations

- Random Forest and XGBoost models achieved perfect AUC-ROC scores of 1.0, indicating excellent performance.
- Oversampling increased the number of minority class samples, while undersampling decreased the number of majority class samples, balancing the dataset.
- Isolation Forest detected approximately 15% of transactions as outliers, potentially indicating fraudulent activity.
- Feature engineering, particularly the introduction of moving averages over time, demonstrated improvements in fraud detection accuracy.

Feel free to explore the code and experiment with different approaches to enhance credit card fraud detection. If you have any questions or suggestions, please don't hesitate to reach out.
