# zeynep_yagmur_demir_dsa210project
# DSA 210 Project - Fashion Product Popularity Analysis

## Project Topic
This project explores how fashion product popularity differs across selected women's clothing categories.

## Dataset
The dataset consists of products from the following categories:
- Dresses & Jumpsuits
- Skirts
- Tops & Bodysuits
- Knitwear

## Data Processing
- Combined multiple category datasets into one dataset
- Added category labels
- Cleaned the price column
- Removed unnecessary columns

## Exploratory Data Analysis (EDA)
- Analyzed number of products per category
- Compared average prices across categories
- Visualized category distribution and price differences

## Detailed Results

- Total number of products: 1038
- Dresses & Jumpsuits: 643 products
- Knitwear: 228 products
- Tops & Bodysuits: 108 products
- Skirts: 59 products

### Average Prices

- Dresses & Jumpsuits: 4415.51
- Skirts: 3395.08
- Knitwear: 3318.07
- Tops & Bodysuits: 2654.81

### Keyword Counts

- "dress": 572
- "knit": 278
- "top": 157
- "skirt": 59

## Visualizations

### Category Distribution
![Category Distribution](category_distribution.png)

### Average Price by Category
![Average Price](average_price_by_category.png)

### Keyword Frequency
![Keyword Frequency](keyword_frequency.png)

## Initial Findings
- Dresses are the most common category in the dataset
- Dresses have the highest average price
- Tops have the lowest average price
- Product name analysis shows “dress” appears most frequently

## Hypothesis
Products associated with popular fashion trends appear more frequently in the dataset.

## Next Steps
- Improve analysis
- Add trend-based data (Google Trends)
- Apply machine learning methods

## Machine Learning

In this stage, I built a classification model to predict the product category based on product names.

### Method

- Product names were converted into numerical features using **CountVectorizer**
- The dataset was split into training and testing sets (80% / 20%)
- A **Multinomial Naive Bayes** model was used for classification

### Results

- Model Accuracy: **0.90**

### Performance by Category

- Dresses: F1-score = 0.94 (highest performance)
- Knitwear: F1-score = 0.84
- Skirts: F1-score = 0.83
- Tops: F1-score = 0.79 (lowest performance)

### Interpretation

The model performs well overall, showing that product names contain strong information about their category. In particular, dresses are very easy to identify from text.

However, categories like tops are more difficult to classify, likely because the term “top” is more general and overlaps with other categories.

These results suggest that text-based features are useful for predicting fashion categories, but additional features or external data could further improve performance.
