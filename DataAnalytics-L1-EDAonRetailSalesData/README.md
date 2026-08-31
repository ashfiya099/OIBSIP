
## Objective

Perform exploratory data analysis (EDA) on retail sales data to identify sales trends, customer behavior, product-category performance, and relationships between numerical variables.

The analysis uses Python and data visualization techniques to generate actionable business insights.

## Dataset

The project uses a Retail Sales Dataset containing **1,000 transactions** and **9 original columns**.

### Dataset Columns

- Transaction ID
- Date
- Customer ID
- Gender
- Age
- Product Category
- Quantity
- Price per Unit
- Total Amount

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Kaggle

## Data Quality

Initial data inspection showed:

| Metric | Result |
|---|---:|
| Rows | 1,000 |
| Columns | 9 |
| Missing Values | 0 |
| Duplicate Rows | 0 |

The `Date` column was converted from object format to datetime format for time-series analysis.

## Exploratory Data Analysis

### 1. Descriptive Statistics

Descriptive statistics were calculated for numerical variables including:

- Age
- Quantity
- Price per Unit
- Total Amount

This provided an overview of customer characteristics, purchasing quantities, pricing, and transaction values.

### 2. Monthly Sales Trend

Monthly sales were calculated by aggregating total transaction amounts by month.

The monthly trend helps identify periods of relatively high and low sales activity.

### 3. Quarterly Sales Trend

Sales were also aggregated by quarter to provide a broader view of revenue patterns and reduce short-term fluctuations.

### 4. Customer Demographics

Customer behavior was analyzed using:

- Age groups
- Gender
- Age group and gender combinations

These analyses help identify important customer segments for targeted marketing strategies.

### 5. Product Category Analysis

The dataset does not contain individual product names. Therefore, product-level ranking was not possible.

Instead, product categories were analyzed using:

- Transaction count
- Total revenue

This identifies the categories contributing most strongly to overall sales.

### 6. Correlation Analysis

A correlation matrix was created for:

- Age
- Quantity
- Price per Unit
- Total Amount

A heatmap was used to visualize the strength and direction of relationships between numerical variables.

### 7. Additional Analysis

A scatter plot was created to investigate the relationship between:

**Quantity Purchased vs Total Transaction Amount**

Product category and price per unit were also considered to provide additional insight into purchasing behavior.

## Key Insights

- Sales vary across different months and quarters.
- Customer age groups contribute differently to total revenue.
- Gender-based sales patterns provide useful information for customer segmentation.
- Product categories differ in both transaction volume and revenue contribution.
- Quantity purchased and price per unit influence the total transaction value.
- Correlation analysis provides insight into relationships between the numerical variables.

## Business Recommendations

### 1. Focus on High-Revenue Categories

Invest in inventory and marketing for the categories generating the highest revenue. Promotional campaigns can be targeted toward these high-performing categories.

### 2. Target High-Value Customer Segments

Use age-group and gender analysis to identify important customer segments and develop targeted marketing campaigns and promotions.

### 3. Optimize Pricing and Quantity-Based Promotions

Use purchasing quantity and transaction-value patterns to design volume discounts, bundles, and promotional offers that can increase average transaction value.

## Limitations

The dataset does not contain individual product names or product IDs. Therefore, a true Top 10 individual product analysis could not be performed.

The analysis is also based on a relatively small dataset of 1,000 transactions, so the observed patterns may not represent all retail customers or longer-term business behavior.

## Conclusion

This project demonstrates how exploratory data analysis can be used to transform retail transaction data into useful business insights.

Sales trends, customer demographics, product categories, and numerical relationships were analyzed using Python. Visualizations such as line charts, bar charts, scatter plots, and a correlation heatmap were used to communicate the findings.

The results can support business decisions related to marketing, inventory planning, customer segmentation, pricing, and promotional strategies.
