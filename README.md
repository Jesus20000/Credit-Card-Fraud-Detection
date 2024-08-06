# Credit Card Fraud Detection

## Overview
This project aims to detect fraudulent credit card transactions using a dataset containing transactions from European cardholders. The dataset is highly unbalanced, with fraud cases accounting for only 0.172% of transactions. The goal is to build a model that can accurately identify fraudulent transactions.

## Libraries Used
- `pandas` - Data manipulation and analysis.
- `numpy` - Numerical computing.
- `matplotlib` - Plotting and visualization.
- `seaborn` - Statistical data visualization.
- `sklearn` - Machine learning tools including `RandomForestClassifier`, `precision_recall_curve`, and `StandardScaler`.

## Data
- **Source**: The dataset is from transactions made by credit cards in September 2013 by European cardholders.
- **Features**: 
  - **V1** to **V28**: Principal components obtained with PCA transformation.
  - **Time**: Seconds elapsed between each transaction and the first transaction.
  - **Amount**: Transaction amount.
  - **Class**: Response variable where 1 indicates fraud and 0 indicates non-fraud.

## Analysis Steps
1. **Data Exploration**:
   - Load and explore the dataset.
   - Check for missing values and data types.
   - Analyze feature correlations.

2. **Preprocessing**:
   - Scale the `Time` and `Amount` features.
   - Split the data into training and testing sets.

3. **Modeling**:
   - Train a `RandomForestClassifier` on the training data.
   - Predict probabilities on the test data.

4. **Evaluation**:
   - Calculate precision-recall curve and AUPRC.
   - Generate a classification report with precision, recall, and F1-score.

## Insights
- The model achieved an AUPRC of 0.868, indicating good performance in identifying fraudulent transactions.
- The dataset is highly imbalanced, which is a significant challenge for model accuracy.

## Conclusion
The Random Forest model effectively identifies fraudulent transactions, though further improvements could be made by exploring additional algorithms or advanced techniques to handle class imbalance.

## Requirements
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/Credit-Card-Fraud-Detection.git
