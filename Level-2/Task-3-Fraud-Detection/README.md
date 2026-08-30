# Task 3 - Fraud Detection

## Objective

Build a machine learning pipeline to detect fraudulent credit card transactions from a highly imbalanced dataset.

## Dataset

**Credit Card Fraud Detection Dataset**

The dataset contains 284,807 transactions, including only 492 fraudulent transactions.

### Class Distribution

- Non-Fraudulent: 284,315 (99.83%)
- Fraudulent: 492 (0.17%)

The dataset is highly imbalanced, making accuracy alone an unsuitable metric for evaluating fraud detection models.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
- Kaggle

## Data Preparation

The following preprocessing steps were performed:

- Loaded and inspected the dataset
- Analyzed class imbalance
- Performed stratified train-test splitting
- Applied SMOTE only to the training data
- Scaled features for Logistic Regression
- Kept the test dataset unchanged for unbiased evaluation

## Models

Two classification models were trained:

1. Logistic Regression
2. Random Forest

## Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 98.99% | 13.41% | 89.80% | 23.34% | 97.65% |
| Random Forest | 99.94% | 82.65% | 82.65% | 82.65% | 96.44% |

## Results

Logistic Regression achieved higher Recall and AUC-ROC, meaning it detected a larger proportion of fraudulent transactions and provided strong class discrimination.

Random Forest achieved substantially higher Precision and F1-score while maintaining strong Recall. Therefore, Random Forest provides a better overall balance between detecting fraud and reducing false positive alerts.

## Feature Importance

The most important Random Forest features included:

- V14
- V10
- V4
- V12
- V17
- V3
- V11
- V16
- V2
- V9

These features are anonymized PCA components, so their individual real-world meanings are not directly available.

## Key Learning

Accuracy can be misleading in highly imbalanced fraud datasets. Precision, Recall, F1-score, and AUC-ROC provide more useful information about fraud detection performance.

## Conclusion

The Random Forest model was selected as the preferred model because it provided the best balance between Precision, Recall, and F1-score. A production fraud detection system should continuously monitor model performance and retrain periodically because fraud patterns can change over time.
