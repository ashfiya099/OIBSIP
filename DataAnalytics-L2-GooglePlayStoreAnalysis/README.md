# Level 2 - Task 4: Google Play Store Analysis

## Objective

Analyze the Google Play Store ecosystem to understand app categories, ratings, installations, pricing, application size, and user sentiment.

## Datasets

Two datasets were used:

1. Google Play Store Apps
2. Google Play Store User Reviews

### Final Dataset

- Apps dataset: 10,358 rows and 15 columns
- Reviews dataset: 37,427 rows and 5 columns

The original app columns and cleaned review dataset contain no missing values.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Kaggle

## Data Cleaning

The following preprocessing steps were performed:

- Removed duplicate app records
- Handled missing ratings using the median
- Handled missing categorical values using the mode
- Converted Reviews to numeric
- Converted Installs to numeric
- Converted Price to numeric
- Converted application Size into MB for numerical analysis
- Removed incomplete review records for sentiment analysis

Applications with `"Varies with device"` in the original Size field were retained. These records were excluded only from the numerical Size vs Installs analysis.

## Analysis Performed

### 1. App Category Analysis

The number of applications in each Google Play Store category was analyzed to identify the most common categories.

### 2. Rating Analysis

App ratings were analyzed using:

- Rating distribution
- Rating categories
- Average rating by category

### 3. Reviews vs Ratings

The relationship between the number of reviews and app ratings was examined.

### 4. Size vs Installs

Application size was compared with installation counts to investigate whether app size is associated with popularity.

### 5. Pricing Analysis

Free and paid applications were compared, including:

- Number of free and paid apps
- Paid app price distribution
- Most expensive applications
- Install statistics by app type

### 6. Sentiment Analysis

User reviews were classified into:

- Positive
- Neutral
- Negative

## Sentiment Results

| Sentiment | Percentage |
|---|---:|
| Positive | 64.12% |
| Negative | 22.10% |
| Neutral | 13.78% |

Positive reviews represented the largest share of analyzed reviews.

## Key Insights

1. **Positive sentiment dominates:** 64.12% of analyzed reviews were positive, indicating generally favorable user opinions.

2. **Negative feedback is significant:** 22.10% of reviews were negative, highlighting opportunities for developers to improve application quality and user experience.

3. **App popularity varies considerably:** Installation counts and app categories show that some areas of the Play Store attract substantially more users and applications than others.

## Visualizations

The notebook includes:

- App category distribution
- Rating distribution
- Rating category distribution
- Reviews vs ratings
- Free vs paid app comparison
- App size vs installs
- Paid app price distribution
- Median installs by app type
- Sentiment distribution
- Sentiment percentage

## Conclusion

The analysis demonstrates how exploratory data analysis and sentiment analysis can be used to understand the Google Play Store market.

The dataset contains applications across a wide range of categories with differences in ratings, installations, pricing, and size. User sentiment analysis showed that positive reviews were the dominant sentiment, accounting for 64.12% of analyzed reviews.

The findings can help developers and businesses understand user preferences, identify opportunities for improvement, and make more informed decisions about application development and market positioning.
