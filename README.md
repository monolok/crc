## Exploratory Data Analysis (EDA) -> eda.ipynb
Key findings from the EDA phase include:

1. **Outliers in Age**:
   - Significant outliers were found in the `age` variable, exceeding 3 standard deviations from the mean.
2. **Column Grouping**:
   - Identified two columns suitable for grouping due to similar characteristics.
3. **Feature Correlation**:
   - `total_page_visited` emerged as a crucial feature with strong predictive potential.

## Modeling Approach -> models.ipynb
Multiple models were tested, with focus on:

- **Pipeline 1**: `LogisticRegression()`
- **Pipeline 2**: A comparison model with ridge - shrink the coefficients towards zero, but not exactly zero

Given the data's imbalance (few instances where `y = 1`), the F1 score was used for evaluation. Despite various attempts like SMOTE and feature engineering, the baseline `LogisticRegression` model outperformed others.

## Recommendations from features coeff - cell 43 (models.ipynb):
1. **Increase User Engagement**:
   - Encourage more page visits to boost conversions, leveraging the importance of `total_page_visited`.

2. **Enhance Direct and SEO Traffic**:
   - Improve the quality of direct and SEO traffic to address their negative impact.

3. **Age-Specific Strategies**:
   - Tailor content and strategies for older users to mitigate the negative correlation of age with the target variable.
