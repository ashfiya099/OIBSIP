# 📊 Oasis Infobytes – Data Analytics Internship

Welcome to my **Data Analytics Internship Portfolio at Oasis Infobytes**.

This repository contains the projects I completed during my internship, covering **Data Cleaning, Exploratory Data Analysis, Customer Segmentation, Natural Language Processing, Machine Learning, Data Visualization, and Predictive Analytics**.

The internship provided me with hands-on experience working with real-world datasets and applying Python-based analytical and machine-learning techniques to practical problems.

---

## 👩‍💻 About My Internship

**Organization:** Oasis Infobytes  
**Role:** Data Analytics Intern  
**Domain:** Data Analytics / Data Science  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, NLTK, Jupyter Notebook, Kaggle

### 🎯 Internship Objective

The main objective of this internship was to gain practical experience in:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Statistical analysis
- Data visualization
- Customer analytics
- Natural Language Processing (NLP)
- Machine Learning
- Classification and prediction
- Model evaluation
- Data-driven problem solving

---

# 📂 Projects

## 1. 🧹 Data Cleaning & Preprocessing

The first project focused on preparing raw data for analysis.

### Work Performed
- Inspected the dataset
- Checked missing values
- Identified duplicate records
- Examined data types
- Cleaned and organized the data
- Validated the final dataset

### Skills
`Python` `Pandas` `NumPy` `Data Cleaning`

---

## 2. 🛍️ Exploratory Data Analysis on Retail Sales

This project analyzed retail transactions to understand sales performance and customer purchasing behavior.

### Dataset
- **Rows:** 1,000
- **Columns:** 9
- Product categories: Clothing, Electronics, Beauty

### Analysis Performed
- Product category analysis
- Gender-wise sales analysis
- Customer age analysis
- Monthly sales trends
- Descriptive statistics
- Correlation analysis
- Data visualization

### Key Findings

- Clothing had the highest sales share at **35.1%**
- Electronics contributed **34.3%**
- Beauty contributed **30.6%**
- Female customers contributed **51.7%** of sales
- Male customers contributed **48.3%**
- Sales peaked in **May**
- Customers aged **64** recorded the highest purchases
- Price per Unit and Total Amount had a correlation of approximately **0.72**

### Skills
`Python` `Pandas` `Matplotlib` `Seaborn` `EDA` `Data Visualization`

---

## 3. 👥 Customer Segmentation

This project focused on identifying meaningful customer groups based on purchasing behavior.

### Work Performed
- Prepared customer data
- Selected relevant features
- Analyzed customer behavior
- Applied clustering techniques
- Visualized customer segments
- Interpreted differences between customer groups

### Skills
`Python` `Pandas` `NumPy` `Scikit-learn` `Clustering` `Data Visualization`

---

## 4. 💬 Sentiment Analysis

This project used Natural Language Processing and Machine Learning to classify sentiment from Twitter data.

### Dataset

The project used Twitter entity sentiment data containing tweet text, entities, and sentiment labels.

After preprocessing and filtering irrelevant records:

- **Total relevant records:** 61,121
- Positive: **22,358**
- Neutral: **20,655**
- Negative: **18,108**

### Work Performed

- Text preprocessing
- Removal of irrelevant records
- Text cleaning
- TF-IDF feature extraction
- Sentiment classification
- Confusion matrix visualization
- Word cloud generation
- Sample prediction analysis

### Models

- Naive Bayes
- Logistic Regression

### Skills
`Python` `Pandas` `NLTK` `TF-IDF` `Scikit-learn` `NLP` `Sentiment Analysis`

---

## 5. 🛡️ Credit Card Fraud Detection

This project focused on detecting fraudulent transactions using machine learning.

Because fraud datasets are highly imbalanced, multiple evaluation metrics were considered instead of relying only on accuracy.

### Models

- Logistic Regression
- Random Forest

### Model Comparison

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 98.99% | **99.94%** |
| Precision | 13.41% | **82.65%** |
| Recall | **89.80%** | 82.65% |
| F1-Score | 23.34% | **82.65%** |
| ROC-AUC | **97.65%** | 96.44% |

### Key Insight

Logistic Regression achieved higher recall but produced many false positives because of its low precision.

Random Forest provided a much more balanced performance, achieving **99.94% accuracy, 82.65% precision, 82.65% recall, and 82.65% F1-score**.

### Feature Importance

Important Random Forest features included:

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

### Skills
`Python` `Pandas` `Scikit-learn` `Random Forest` `Logistic Regression` `Classification` `Model Evaluation`

---

## 6. 📱 Google Play Store Analysis

This project explored Google Play Store applications and user reviews to understand patterns in app performance and user sentiment.

### Datasets

- Google Play Store Apps dataset
- Google Play Store User Reviews dataset

### Data Preparation

The Apps dataset originally contained duplicate records and missing values in several fields.

After cleaning:

- **Apps dataset:** 10,358 rows
- **Reviews dataset:** 37,427 rows

### Analysis Performed

- App category analysis
- Ratings analysis
- Install analysis
- Price and size analysis
- Review sentiment analysis
- Data cleaning and feature engineering
- Data visualization

### Review Sentiment

- Positive: **64.12%**
- Negative: **22.10%**
- Neutral: **13.78%**

### Skills
`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `EDA` `Data Visualization`

---

## 7. 🏠 House Price Prediction

This project focused on applying machine learning techniques to predict house prices based on relevant property features.

### Work Performed

- Dataset inspection
- Data preprocessing
- Feature preparation
- Exploratory analysis
- Model training
- Prediction
- Model evaluation

### Skills
`Python` `Pandas` `NumPy` `Scikit-learn` `Machine Learning` `Regression`

---

## 8. 🍷 Wine Quality Prediction

This project applied machine learning to analyze wine characteristics and predict wine quality.

### Features Analyzed

- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

### Work Performed

- Data inspection
- Data preprocessing
- Exploratory Data Analysis
- Feature analysis
- Machine learning
- Model evaluation
- Quality prediction

### Skills
`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Scikit-learn` `Machine Learning`

> Model performance metrics are documented in the project notebook.

---

## 9. ⌨️ Autocomplete & Autocorrect

This project explored Natural Language Processing techniques for predicting the next word and correcting spelling mistakes.

### Corpus

- Characters: **6,521,824**
- Original tokens: **1,188,562**
- Cleaned tokens: **612,650**
- Unique words: **21,310**

### Autocomplete

Two language-model approaches were explored:

- Bigram model
- Trigram model

### Top-3 Accuracy

| Model | Top-3 Accuracy |
|---|---:|
| Bigram | 28.46% |
| Trigram | **93.07%** |

The trigram model performed significantly better for the tested prefixes.

### Autocorrect

A custom edit-distance based approach was used to identify possible spelling corrections.

- Words tested: **20**
- Correct corrections: **12**
- Accuracy: **60%**

### Skills
`Python` `NLP` `Tokenization` `N-grams` `Edit Distance` `Text Processing`

---

# 🛠️ Technologies & Tools

### Programming
- Python

### Data Analysis
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn
- Logistic Regression
- Random Forest
- Clustering
- Regression

### Natural Language Processing
- NLTK
- TF-IDF
- N-gram models
- Text preprocessing
- Edit-distance based autocorrection

### Platforms
- Jupyter Notebook
- Kaggle
- GitHub

---

# 📈 Overall Internship Workflow

```text
Raw Data
   ↓
Data Cleaning & Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Data Visualization
   ↓
Feature Engineering
   ↓
Machine Learning / NLP
   ↓
Model Evaluation
   ↓
Insights & Conclusions
