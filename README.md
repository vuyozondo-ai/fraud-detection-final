# Fraud Detection Using Machine Learning

This project focuses on detecting fraudulent financial transactions using machine learning techniques. The goal is to identify patterns in transaction behaviour that distinguish fraudulent activities from legitimate ones.

## Project Overview

The dataset contains transaction details such as transaction type, amount, and account balances. Due to the highly imbalanced nature of fraud data, special attention was given to feature engineering and model evaluation.

## Feature Engineering

To improve model performance, the following features were created:

- **balance_error** – captures inconsistencies between expected and actual account balances  
- **is_full_drain** – identifies transactions that completely empty an account  
- **is_logical** – flags whether a transaction follows expected financial behaviour  

These features helped highlight suspicious transaction patterns.

## Models Used

- **Random Forest** – used as a baseline model  
- **XGBoost** – used as the final model due to its performance on structured and imbalanced data  

## Results

Both models achieved high performance, with XGBoost slightly outperforming Random Forest. The results indicate that the engineered features provide strong signals for detecting fraudulent transactions.

## Repository Structure

- `fraud_detection_model.ipynb` – final modelling notebook  
- `EDA.ipynb` – exploratory data analysis  
- `README.md` – project overview  

## Notes

While the model performance is strong, the dataset contains some unrealistic transaction patterns, which may simplify fraud detection compared to real-world scenarios.
