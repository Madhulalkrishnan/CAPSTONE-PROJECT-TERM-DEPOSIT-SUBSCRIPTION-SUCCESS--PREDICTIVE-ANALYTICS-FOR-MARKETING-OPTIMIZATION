# CAPSTONE-PROJECT-TERM-DEPOSIT-SUBSCRIPTION-SUCCESS--PREDICTIVE-ANALYTICS-FOR-MARKETING-OPTIMIZATION
Predictive analytics for term deposit subscription success using Logistic Regression
# Term Deposit Subscription Success: Predictive Analytics for Marketing Optimization

## 🚀 Project Overview

This capstone project focuses on developing a robust *Binary Classification Model* to optimize the direct telemarketing campaigns of a Portuguese banking institution. The primary objective is to accurately predict whether a client will subscribe to a *Term Deposit*, enabling the bank to transform expansive, high-cost campaigns into a targeted, data-driven strategy.

## 📊 Dataset

* *Source:* UCI Machine Learning Repository (Bank Marketing Data Set)
* *Instances:* 45,211
* *Features:* 17 attributes covering client demographics, financial status, and campaign history.
* *Target:* y (Client subscribed to the term deposit: 'yes' or 'no').
* *Key Challenge:* The target variable exhibits a *severe class imbalance* ('no' $\approx 89\%$, 'yes' $\approx 11\%$).

## 🛠️ Methodology and Pipeline

### 1. Data Integrity and Preprocessing
* *Data Leakage Prevention:* The highly influential duration feature (which is known only after the outcome is achieved) was *removed* from the training set to ensure the model’s real-world predictive validity.
* *Feature Engineering:* Managed implicit missing values (string 'unknown') and applied *One-Hot Encoding* to all nominal categorical features.

### 2. Model Implementation
* *Model:* A *Logistic Regression* classifier was implemented as the initial, highly interpretable baseline model.
* *Splitting:* Data was split into 80% Training and 20% Testing sets, using stratification to maintain the class balance.

## 🎯 Results and Evaluation

Given the class imbalance, model performance was evaluated with a focus on metrics relevant to the minority class ('yes').

| Metric | Score (Test Set) | Business Implication |
| :--- | :--- | :--- |
| *Overall Accuracy* | $0.897$ | Strong performance on the majority class. |
| *'Yes' Precision* | $0.63$ | $63\%$ of clients predicted to subscribe actually did. (Good for efficient targeting) |
| *'Yes' Recall* | $0.30$ | Identified $30\%$ of all positive subscribers. (Area for future improvement) |
| *'Yes' F1-Score* | $0.40$ | Balanced measure of the model's predictive power on the positive class.
### Conclusion:
Machine learning models can successfully predict customer subscription for bank campaigns. While overall accuracy is high, identifying actual subscribers requires handling class imbalance. Insights can guide targeted marketing strategies.In this project, we analyzed the Bank Marketing Dataset to predict whether a customer would subscribe to a term deposit. After performing data preprocessing, encoding, visualization, and model training, we built a classification model that achieved an accuracy of approximately 90%.

The model performed very well in predicting the majority class (“no”), but struggled with the minority class (“yes”) due to strong class imbalance in the dataset. Despite this limitation, the project successfully highlighted important patterns in customer behavior.
