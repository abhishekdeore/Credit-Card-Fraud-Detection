# Credit Card Fraud Detection Project

## Overview
This project implements advanced anomaly detection techniques to identify fraudulent credit card transactions. Using machine learning models, specifically Isolation Forest and Local Outlier Factor (LOF), the system detects unusual patterns that may indicate fraudulent activity in credit card usage.

## Dataset
Link - https://drive.google.com/file/d/1M3MyNFqT3659qfOOcp30nUAe9UaU8uZP/view?usp=drive_link
The project uses the Credit Card Fraud Detection dataset, which contains transactions made by European cardholders in September 2013. Key characteristics:
- Total transactions: 284,807
- Fraudulent transactions: 492 (0.172% of total)
- Features: 28 principal components (V1-V28), 'Time', and 'Amount'
- Target variable: 'Class' (1 for fraud, 0 for normal)

## Features
- Comprehensive Exploratory Data Analysis (EDA)
- Data preprocessing and feature engineering
- Advanced handling of class imbalance using SMOTE (Synthetic Minority Over-sampling Technique)
- Implementation of Isolation Forest and Local Outlier Factor (LOF) for anomaly detection
- Detailed model evaluation using ROC curves and AUC scores
- Comparative analysis of model performance

## Requirements
- Python 3.8+
- Jupyter Notebook
- Key libraries: numpy, pandas, scikit-learn, imbalanced-learn, matplotlib, seaborn
- Full dependencies listed in `requirements.txt`

## Installation
1. Clone the repository:
   git clone https://github.com/abhishekdeore/credit-card-fraud-detection.git
   cd credit-card-fraud-detection

2. Create and activate a virtual environment (optional but recommended):
   python -m venv venv
   source venv/bin/activate  # On Windows use venv\Scripts\activate

3. Install the required packages:
   pip install -r requirements.txt

## Usage
1. Ensure the dataset file 'creditcard.csv' is placed in the 'data' folder.
2. Launch Jupyter Notebook:
   jupyter notebook

3. Navigate to the 'notebooks' directory and open the notebooks in order:
- `1_EDA_and_Preprocessing.ipynb`
- `2_Model_Evaluation.ipynb`
4. Run the cells in each notebook sequentially to perform EDA, preprocess the data, train the models, and evaluate their performance.

## Results
The project demonstrates the effectiveness of Isolation Forest and LOF in detecting credit card fraud:
- Isolation Forest: AUC score of 0.8942
- Local Outlier Factor: AUC score of 0.8640

These results indicate strong performance in distinguishing fraudulent transactions from legitimate ones, with Isolation Forest showing a slight edge in overall effectiveness.

## Key Findings
- Both models significantly outperform random guessing (AUC > 0.5).
- Isolation Forest shows superior performance, particularly in maintaining a high true positive rate at low false positive rates.
- The models' high AUC scores suggest effective separation between normal and fraudulent transactions.
- EDA revealed important insights into the distribution of fraudulent transactions and the characteristics of the dataset.

## Future Work
- Implementation of additional models (e.g., Random Forest, XGBoost) for comprehensive comparison
- Exploration of deep learning approaches for anomaly detection
- Hyperparameter optimization for enhanced model performance
- Development of a real-time fraud detection system
- Investigation into model interpretability for better understanding of fraud indicators

## Contributing
Contributions to this project are welcome. Please follow these steps:
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes and commit (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new Pull Request

