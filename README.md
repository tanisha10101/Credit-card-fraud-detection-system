
# Credit Card Fraud Detection System

## Introduction

Credit card fraud is a critical issue affecting millions of people and financial institutions globally. It occurs when someone illegally uses credit card information to make unauthorized transactions. As the world moves towards digital payments, the complexity and frequency of such fraudulent activities are increasing.

### Why Fraud Detection is Necessary
- **Protecting Financial Assets**: Fraudulent transactions can result in significant monetary losses for both consumers and financial institutions.
- **Ensuring Trust**: Customers rely on financial systems to keep their transactions secure, and failure to do so can erode trust.
- **Compliance with Regulations**: Financial entities are obligated to implement robust security measures to meet regulatory requirements.

### Global Impact
- The Nilson Report highlighted over $28 billion in global fraud losses in 2022.
- The U.S. alone accounts for one-third of these losses.
- Card-not-present (CNP) fraud and phishing remain the most common fraud types.

## Project Overview
This project presents a comprehensive approach to detecting credit card fraud using state-of-the-art Machine Learning (ML) and Neural Network (NN) models. By leveraging advanced techniques in data preparation, model training, and evaluation, this system ensures high accuracy in identifying fraudulent activities.

## Methodology

### Step 1: Data Preparation
- **Data Cleaning**: Handled missing values, removed duplicates, and ensured data integrity.
- **Feature Engineering**: Developed new predictive features and optimized existing ones to capture hidden patterns.
- **Data Visualization**: Leveraged bar plots, heatmaps, and histograms to understand transaction distributions and spot anomalies.

### Step 2: Data Preprocessing
- Normalized data to maintain uniformity across features.
- Split data into training (80%) and testing (20%) subsets to evaluate model performance.

### Step 3: Model Training
#### Machine Learning Models
1. **Logistic Regression**
2. **Random Forest**
3. **Extreme Gradient Boost (XGBoost)**
4. **Light Gradient-Boosting Machine (LightGBM)**

#### Neural Networks
1. **Deep Neural Network (DNN)**
2. **Recurrent Neural Network (RNN)**

### Step 4: Performance Metrics
- **AUC (Area Under the Curve)**: Evaluates the model’s ability to differentiate between classes (higher is better).
- **Hamming Loss**: Measures the fraction of incorrect predictions (lower is better).
- **ROC Curve**: Visual tool to assess classification thresholds.

## Key Findings

### Transaction Patterns
- Fraudulent transactions are exclusive to `TRANSFER` and `CASH_OUT` transaction types.
- Fraudulent activities are always between customer accounts.
- A single recipient account was used 4,097 times in fraudulent `TRANSFER` transactions.

### Model Performance
#### Machine Learning Models
- **Logistic Regression**: AUC - 0.9837, Hamming Loss - 0.000834
- **Random Forest**: AUC - 0.7469, Hamming Loss - 0.001035
- **Extreme Gradient Boost**: AUC - 0.9176, Hamming Loss - 0.001152
- **LightGBM**: AUC - 0.4936, Hamming Loss - 0.00142

**Insight**: Logistic Regression performed best among ML models, while LightGBM showed the weakest results.

#### Neural Networks
- **DNN**: AUC - 0.9957, Hamming Loss - 0.000538
- **RNN**: AUC - 0.9971, Hamming Loss - 0.000471

**Insight**: Neural Networks significantly outperformed ML models, with RNN delivering the highest accuracy and lowest error rates.

## Observations
1. RNN excels in capturing sequential patterns, making it ideal for fraud detection.
2. Neural Networks generally outperform traditional ML models for complex tasks.
3. Fraud detection systems can greatly benefit from tailored feature engineering and advanced NN architectures.

## Notes
- **Data Source**: [Kaggle Paysim1 Dataset](https://www.kaggle.com/datasets/ealaxi/paysim1)
- **Acknowledgments**: Inspired by [Waleed Faheem's Kaggle Notebook](https://www.kaggle.com/code/waleedfaheem/credit-card-fraud-detection-auc-0-9). Key enhancements include:
  - Incorporating Neural Networks.
  - Additional insights and metrics.

## Future Directions
- Integrate additional datasets for increased robustness.
- Experiment with advanced architectures like Transformers and Graph Neural Networks.
- Develop real-time fraud detection systems using streaming technologies.
- Explore interpretability tools to better understand model predictions.

## Conclusion
This credit card fraud detection system demonstrates the power of combining Machine Learning and Neural Networks. The use of sophisticated models and performance metrics ensures accurate identification of fraudulent transactions, offering a reliable tool to combat financial fraud on a global scale.


