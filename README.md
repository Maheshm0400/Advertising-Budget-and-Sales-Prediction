# Advertising-Budget-and-Sales-Prediction

This project analyzes the relationship between advertising budgets (TV, Radio, Newspaper) and product sales. It applies data visualization and linear regression modeling to predict future sales based on advertising spend.

## Business Objective

- Determine if there's a statistically significant relationship between advertising budget and sales.
- Develop a model to **predict future sales** based on planned advertising budget.
- Example query answered: *What should be the expected sales if the advertising budget is $4000?*

---

## Dataset

The dataset used contains the following features:

| Feature        | Description                      |
|----------------|----------------------------------|
| TV             | Budget allocated to TV ads ($)   |
| Radio          | Budget allocated to radio ads ($)|
| Newspaper      | Budget allocated to newspaper ads ($) |
| Sales          | Units sold                       |

---

## Tools & Libraries

- Python (Pandas, NumPy)
- Data Visualization: Matplotlib, Seaborn
- Machine Learning: Scikit-Learn (`LinearRegression`)
- Evaluation Metrics: MAE, MSE, RMSE, R²

---

## Process Overview

1. **Data Cleaning**
   - Renamed columns for ease of use.
   - Created a `total` budget column combining all ad spends.

2. **Exploratory Data Analysis**
   - Scatter plots to visualize correlation between budget and sales.
   - Linear regression line fit using `sns.regplot`.

3. **Model Development**
   - Used `LinearRegression` from Scikit-learn.
   - Split data into training and testing sets (67% / 33%).
   - Trained model and generated predictions on test data.

4. **Model Evaluation**
   - Evaluated using:
     - **MAE (Mean Absolute Error)**
     - **MSE (Mean Squared Error)**
     - **RMSE (Root Mean Squared Error)**
     - **R² Score**

---

## Sample Output

Example prediction formula derived from regression:
```
Predicted Sales = 0.05 × Total_Budget + 4.24
```
For a total advertising budget of **$500**, the expected sales would be approximately **29.24 units sold**.

---

## Future Improvements

- Try multiple regression using individual ad channels.
- Apply regularization (Lasso, Ridge) to reduce overfitting.
- Evaluate residual plots to assess linear model assumptions.

---

## Conclusion

Advertising spending shows a strong positive correlation with sales. A linear regression model can effectively estimate future sales based on total ad budget.
