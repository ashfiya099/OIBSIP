# Data Analytics Level 1 - Task 4: Sentiment Analysis

## Project Overview

This project develops a machine learning-based sentiment analysis system using Twitter data.

The objective is to classify tweets into three sentiment categories:

- Positive
- Negative
- Neutral

The dataset was cleaned and preprocessed before applying TF-IDF feature extraction and machine learning classification.

## Dataset

The original dataset contained 74,682 tweets.

Columns:

- Tweet ID
- Entity
- Sentiment
- Tweet content

Missing values were handled during preprocessing. Tweets labelled as `Irrelevant` were removed because the project focuses on Positive, Negative, and Neutral sentiment classification.

Final dataset size:

**61,121 tweets**

## Text Preprocessing

The following preprocessing steps were applied:

- Converted text to lowercase
- Removed URLs
- Removed user mentions
- Removed hashtags
- Removed numbers
- Removed punctuation and special characters
- Removed extra whitespace
- Removed common English stopwords

The cleaned text was then used for TF-IDF feature extraction.

## TF-IDF Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) converts text into numerical features that machine learning models can understand.

It gives higher importance to words that are useful for distinguishing tweets while reducing the importance of very common words.

The TF-IDF vectorizer was configured with a maximum of 5,000 features.

Training samples: **48,896**

Testing samples: **12,225**

Training TF-IDF shape: **(48,896, 5,000)**

Testing TF-IDF shape: **(12,225, 5,000)**

## Machine Learning Models

Two classification algorithms were trained and evaluated:

1. Multinomial Naive Bayes
2. Logistic Regression

## Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Multinomial Naive Bayes | 70.34% | 70.73% | 70.34% | 69.87% |
| Logistic Regression | 74.99% | 75.01% | 74.99% | 74.83% |

### Best Model

Logistic Regression achieved the best overall performance with:

- Accuracy: **74.99%**
- Precision: **75.01%**
- Recall: **74.99%**
- F1 Score: **74.83%**

Therefore, Logistic Regression was selected as the better-performing model for this dataset.

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

WordCloud visualizations were also generated to identify frequently occurring words in Positive, Negative, and Neutral tweets.

## Sample Predictions

| Tweet | Predicted Sentiment |
|---|---|
| I absolutely love this product! | Positive |
| This is the worst experience ever. | Negative |
| The product arrived today. | Positive |
| Amazing service and very helpful staff! | Positive |
| I am disappointed with the quality. | Negative |

## Conclusion

This project demonstrates how Natural Language Processing and machine learning can be used to classify the sentiment of Twitter data.

Among the two tested models, Logistic Regression performed better than Multinomial Naive Bayes, achieving an accuracy of **74.99%** and an F1 score of **74.83%**.

The developed sentiment analysis system can be applied to:

- Social media monitoring
- Customer feedback analysis
- Product review analysis
- Customer satisfaction analysis

## Files

- `sentiment-analysis.ipynb` - Complete Jupyter Notebook containing data preprocessing, model training, evaluation, visualizations, and predictions.
- Screenshots - Output and visualization screenshots from the project.
