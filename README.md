# Ecommerce-EDA-Linear-Machine-model-
This repository contains a linear regression analysis performed on an e-commerce dataset to predict **Yearly Amount Spent** based on various customer behavior features. The dataset consisted of approximately 400 rows, making it a relatively small dataset for regression analysis.


## Features Used in the Model
The dataset included the following features:
- **Time on Website**: Average time customers spend on the website.
- **Time on App**: Average time customers spend on the mobile app.
- **Average Session Length**: The average duration of a customer session.
- **Membership Length**: The number of years a customer has been a member.
- **Yearly Amount Spent** (Target): The total amount of money spent by a customer annually.

## Results
The regression model produced the following performance metrics:

- **Baseline MAE**: 66.63  
  (Baseline was calculated using the mean value of `Yearly Amount Spent` for predictions.)
  
- **Mean Absolute Error (MAE)**: 8.12  
  On average, the model's predictions were off by about 8.12 units, significantly outperforming the baseline.

- **Root Mean Squared Error (RMSE)**: 10.15  
  Predictions were off by about 10.15 units on average, with larger errors penalized more heavily.

- **R-squared (R²)**: 0.9858  
  The model explained approximately 98.58% of the variance in `Yearly Amount Spent`.

## Key Insights
1. **Feature Correlations**:
   - **Length of Membership** had an 81% correlation with `Yearly Amount Spent`, making it the most significant predictor.
   - **Time on App** showed a 50% correlation, indicating it is also a strong predictor of spending.
   - **Time on Website** had a near-zero correlation, suggesting that website usage has minimal impact on spending.

2. **Residual Analysis**:
   - The residuals followed a roughly normal distribution, centered around zero, indicating no major biases in the model.

3. **Actionable Insights**:
   - The importance of **Length of Membership** highlights the need for retention strategies to increase customer spending.
   - The correlation with **Time on App** suggests that improving app engagement could boost revenue, as the app is a stronger driver of spending compared to the website.

## Steps to Reproduce
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ecommerce-linear-regression.git
