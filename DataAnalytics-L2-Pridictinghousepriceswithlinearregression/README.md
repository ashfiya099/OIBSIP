# DataAnalytics-L2-Task1-HousePricePrediction

## House Price Prediction using Linear Regression

### Objective

The objective of this project is to build a machine learning model to predict house prices using property-related features. Linear Regression is used as the primary prediction model, with Ridge Regression used for comparison.

## Dataset

The dataset contains information about residential properties, including:

- Seller type
- Under construction status
- RERA registration
- Number of BHKs
- BHK/RK type
- Square footage
- Ready-to-move status
- Resale status
- Longitude
- Latitude
- House price in lakhs

The target variable is:

`TARGET(PRICE_IN_LACS)`

## Data Preprocessing

The following preprocessing steps were performed:

- Inspected the dataset structure and data types
- Checked for missing values
- Checked for duplicate records
- Removed 401 duplicate rows
- Excluded the `ADDRESS` column because of its high-cardinality text values
- Applied One-Hot Encoding to categorical variables
- Split the dataset into training and testing sets using an 80:20 ratio

After removing duplicates, the dataset contained:

- **29,050 rows**
- **12 columns**

## Exploratory Data Analysis

The analysis included:

- Descriptive statistics
- House price distribution
- Missing-value analysis
- Duplicate-value analysis
- Correlation heatmap

## Machine Learning Models

Two regression models were evaluated:

1. Linear Regression
2. Ridge Regression

### Linear Regression Performance

| Metric | Score |
|---|---:|
| MAE | 139.2218 |
| MSE | 364451.6602 |
| RMSE | 603.6983 |
| R² | 0.3344 |

### Ridge Regression Performance

| Metric | Score |
|---|---:|
| MAE | 139.2224 |
| MSE | 364456.2698 |
| RMSE | 603.7021 |
| R² | 0.3344 |

## Model Comparison

Linear Regression performed slightly better than Ridge Regression on the test data.

The difference between the two models was very small, indicating that Ridge regularization did not provide a significant improvement for this dataset.

Therefore, **Linear Regression was selected as the final model**.

## Visualizations

The project includes:

- House price distribution
- Correlation heatmap
- Actual vs Predicted house prices
- Residual plot
- Feature coefficient analysis
- Linear Regression vs Ridge Regression comparison

## Conclusion

The Linear Regression model achieved an R² score of approximately **0.3344**, explaining about 33.44% of the variation in house prices.

The model demonstrates how property characteristics such as BHK count, square footage, seller type, resale status, and geographical information can be used for house-price prediction.

The remaining variation in prices may be influenced by additional factors such as specific location, neighborhood characteristics, property amenities, construction quality, and market conditions
