# Credit Score Analysis Project

## Overview
This project analyzes user wallet transactions to estimate credit scores using data-driven methods. The workflow includes data extraction, feature engineering, model training, and evaluation.

## Method Chosen
We use a supervised machine learning approach to predict credit scores based on wallet transaction data. The method involves:
- **Data Cleaning:** Handling missing values, outliers, and data normalization.
- **Feature Engineering:** Extracting relevant features from transaction data (e.g., transaction frequency, average transaction amount, asset diversity).
- **Model Selection:** Using models such as Random Forest, Gradient Boosting, or Logistic Regression for prediction.
- **Evaluation:** Assessing model performance using metrics like accuracy, precision, recall, and ROC-AUC.


## Components
- **Raw Data:** JSON files containing user wallet transactions.
- **Preprocessing:** Scripts/notebooks to clean and transform raw data into structured features.
- **Feature Matrix:** CSV files with engineered features for each wallet.
- **Model Notebook:** Jupyter notebook for model training, validation, and feature importance analysis.
- **Results:** Output files with predicted credit scores and analysis.

## Processing Flow
1. **Data Loading:**
   - Load transaction data from JSON files.
2. **Preprocessing:**
   - Clean data, handle missing values, and normalize fields.
3. **Feature Engineering:**
   - Extract features such as transaction count, average amount, asset price, and wallet activity patterns.
4. **Model Training:**
   - Train machine learning models using the feature matrix.
   - Tune hyperparameters and select the best model.
5. **Prediction:**
   - Apply the trained model to generate credit scores for each wallet.
6. **Analysis:**
   - Analyze feature importance and visualize results (see `Analysis.md` and `images/`).

## Files
- `user-wallet-transactions.json`, `dataset.json`: Raw transaction data.
- `feature_importance.csv`, `detailed_wallet_analysis.csv`: Engineered features and analysis.
- `wallet_credit_scores.csv`: Predicted credit scores.
- `model.ipynb`: Jupyter notebook for modeling and analysis.
- `Analysis.md`: Markdown file with detailed analysis and visualizations.
- `images/`: Folder containing plots and figures.

## How to Run
1. Install dependencies (see `venv/` or use your own virtual environment).
2. Open `model.ipynb` and run all cells to process data and train the model.
3. Review results in the output CSV files and `Analysis.md`.

