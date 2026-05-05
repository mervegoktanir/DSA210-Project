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
