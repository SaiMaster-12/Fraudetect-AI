# Fraudetect-AI

## Overview
AI-powered system to detect and prevent fraudulent merchants in e-commerce platforms. Fraudulent merchant activity poses a serious threat to online marketplaces. As e-commerce platforms scale, identifying and mitigating merchants who engage in deceptive practices—such as delivering counterfeit goods or failing to fulfill orders—becomes essential to maintaining trust and operational efficiency.

This project presents a comprehensive machine learning solution to detect fraudulent merchants based on both behavioral and transactional data. The framework helps in proactive fraud detection and assists in optimizing fraud investigation resources.

## Problem Statement
Many e-commerce platforms face increasing challenges with scam merchants who exploit the system, negatively impacting customers and legitimate sellers. The need for a reliable, data-driven solution is urgent to prevent financial loss and reputational damage.

This system predicts whether a merchant is:
- Fraudulent (1)
- Non-Fraudulent (0)

using a combination of quantitative and qualitative features extracted from merchant and order datasets.

## Dataset Description

The dataset includes both training and test data comprising merchant profiles, order information, and fraud labels.

Training Data:
- train_merchant_data.csv – Merchant profile information
- train_order_data.csv – Merchant-related order details
- train.csv – Labels indicating whether a merchant is fraudulent (1) or not (0)

Testing Data:
- test_merchant_data.csv – Merchant profile information (unlabeled)
- test_order_data.csv – Order-level behavior (unlabeled)
- test.csv – Placeholder for predicted output

## Key Features & Insights

- Merchant activity metrics (e.g., order volume, return rate)
- Delivery and fulfillment efficiency
- Customer feedback patterns
- Price consistency and anomalies
- Behavioral red flags (e.g., excessive cancellations)

These features were engineered to uncover patterns linked to fraudulent behavior.

## Tech Stack & Tools

- Python: pandas, NumPy, scikit-learn, matplotlib, seaborn
- Jupyter Notebooks: For exploratory data analysis and modeling
- Machine Learning Models: Logistic Regression, Random Forest, XGBoost
- Evaluation Metrics: F1 Score, Accuracy, Confusion Matrix
- Data Pipelines: Custom preprocessing and feature engineering scripts

## Project Approach

1. Exploratory Data Analysis (EDA)
   - Visualization of merchant and order characteristics
   - Detection of trends, imbalances, and outliers

2. Feature Engineering
   - Aggregated order metrics to merchant level
   - Custom features such as return-to-order ratio and cancellation spikes

3. Model Training & Selection
   - Compared multiple models for classification accuracy and F1 score
   - Tuned hyperparameters using grid search and cross-validation

4. Inference on Test Data
   - Applied pipeline and trained model to predict fraud status for test merchants

## Results

- Achieved high F1 score on validation data (add actual metrics here)
- Reduced false positives while maintaining high fraud detection sensitivity
- Identified top predictors of fraud including delivery delays and low fulfillment rates

## Future Enhancements

- Integration with a real-time fraud alert system
- Dashboard for visual fraud analytics and reporting
- Use of additional metadata such as IP geolocation and device ID
