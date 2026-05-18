# DSA210-Project
Merve Göktanır DSA210 Project
[proposal2.pdf](https://github.com/user-attachments/files/26386871/proposal2.pdf)
# DSA210 Term Project

## Project Topic
This project investigates whether increasing online interest in matcha is related to demand-related indicators of matcha-based products.

## Data Sources
- Google Trends data for the keywords "matcha" and "matcha latte"
- Publicly available product data collected from online retail pages

## Variables
The product dataset includes:
- product name
- price
- rating
- review count
- category
- source
- collection date

## Work Completed for This Stage
- Data collection
- Data cleaning
- Exploratory Data Analysis (EDA)
- Hypothesis testing

## Main Findings
- Google Trends suggests that online interest in matcha has increased over time.
- The current product data shows variation across categories.
- Spearman correlation between price and review count is negative but not statistically significant.
- Kruskal-Wallis test does not show a statistically significant difference in review counts across categories.

## Limitation
The product dataset is relatively small and represents a single-date snapshot, so the findings should be interpreted cautiously.

## Files
- `google_trends_matcha.csv`
- `google_trends_matcha_5y.csv`
- `matcha_products_real.csv`
- `matcha_products_clean.csv`
- `dsa210project.ipynb`

## AI Usage
AI tools were used for brainstorming, code structuring, and writing support during the project development process.

## Milestone 2: Machine Learning Methods

In this milestone, machine learning methods were applied to the Google Trends dataset to predict the search interest score for "matcha".

### Machine Learning Objective

The main task was designed as a regression problem. The target variable was the Google Trends interest score for "matcha". Time-based features, lag features, rolling average features, and the related search interest variable "matcha latte" were used as predictors.

### Models Applied

Three regression models were tested and compared:

- Linear Regression
- Ridge Regression
- Random Forest Regressor

### Model Evaluation

The models were evaluated using the following regression metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

Among the tested models, Ridge Regression produced the best performance with an R² score of approximately 0.81. This means that the model was able to explain about 81% of the variation in matcha search interest during the test period.

### Interpretation

The results suggest that matcha search interest can be predicted reasonably well using previous interest values, rolling averages, and related search trends such as "matcha latte". The stronger performance of Linear Regression and Ridge Regression compared to Random Forest suggests that the relationship in this dataset is mostly linear.

The hypothesis testing section was also extended based on feedback. Additional statistical tests were added, and each test now includes the research question, null and alternative hypotheses, significance level, test statistic, p-value, decision, and interpretation.

### Reproducibility

The datasets are loaded directly from the GitHub repository using raw CSV links. This allows the notebook to be run without manually uploading data files.

## Final Project Summary

This project examines whether online interest in matcha is related to demand-related indicators of matcha-based products. The project uses Google Trends data for matcha-related keywords and a product dataset collected from publicly available online retail sources.

The analysis includes data cleaning, exploratory data analysis, hypothesis testing, and machine learning. The product dataset includes variables such as product name, price, rating, review count, category, source, and collection date. The Google Trends dataset is used to observe changes in online search interest over time.

For the statistical analysis, relationships between product variables were examined using correlation analysis and non-parametric hypothesis testing. The results showed that the product-level relationships were not statistically strong, which may be due to the limited size and single-date structure of the product dataset.

For the machine learning part, the project was designed as a regression problem to predict Google Trends interest scores for matcha. Linear Regression, Ridge Regression, and Random Forest Regressor models were tested. Ridge Regression achieved the best performance with an R² score of approximately 0.81, suggesting that lag features, rolling averages, and related search interest variables can be useful for predicting matcha search interest.

Overall, the project shows that online trend data can provide useful insights into changing consumer interest. However, stronger conclusions about product demand would require a larger product dataset collected across multiple time periods.

## Final Limitations

- The product dataset is relatively small.
- Product data was collected as a single-date snapshot.
- Review count was used as a demand-related proxy, not as direct sales data.
- The analysis cannot prove causality between online interest and product demand.
- Google Trends scores are relative search interest values, not absolute search volumes.

## Future Work

Future improvements could include collecting product data weekly or monthly, adding more online platforms, using sales rank or availability data, and building a combined time-series dataset that directly connects Google Trends interest with product-level demand indicators.
