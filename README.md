# PA11_2
# What drives the Price of a Car ?
#Practical Project II, Mod 11

## Summary
This project predicts used car prices and identifies key drivers using linear regression models, following the CRISP-DM framework. The dataset, containing 426,880 used car listings, was cleaned to handle missing values, outliers, and skewed variables. Key findings include:
- **Key Drivers**: Car age, mileage, manufacturer, vehicle type, and condition significantly influence prices.
- **Model Performance**: Lasso regression performed best, with the lowest RMSE and highest R², indicating good predictive power.
- **Findings**: Newer cars, lower mileage, and brands like Toyota command higher prices. SUVs and pickups are also more expensive.
- **Recommendations based on Findings**: Buyers will prioritize newer, low-mileage cars while sellers can highlight these features to maximize value.

## Notebook
The analysis is detailed in the Jupyter notebook: [JK_prompt_II_Mod11.ipynb](JK_prompt_II_Mod11.ipynb)

## Files
- `JK_prompt_II_Mod11.ipynb.ipynb`: Main analysis notebook.
- `purified_vehicles.csv`: Cleaned dataset output.
- `vehicles.csv`: Original dataset.


## Next Steps
- Refine imputation for (condition) and (cylinders)
- Explore polynomial features for nonlinear relationships , for example on (age)
- Collect more data on missing features to improve model accuracy.
- Test the model on new data to ensure generalizability.
- 
Model Results
- Linear Regression: Moderate performance but sensitive to multicollinearity (high correlation) 
- Ridge Regression: More stable due to regularization in finding best alpha using grid search
- Lasso Regression: Best for feature selection and eliminated unimportant features by shrinking their coefficients to zero

Best Performing Model
- Lasso Regression had the lowest RMSE (RMSE: 1.0404) and highest R² (R²: 0.2644), making it the most effective at predicting prices
