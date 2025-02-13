# Housing Price Prediction using Multiple Linear Regression

## Overview
This project aims to predict housing prices using Multiple Linear Regression (MLR). The dataset contains various features such as area, number of bedrooms, number of bathrooms, availability of air conditioning, furnishing status, and other factors influencing housing prices. The project explores different regression models, evaluates their performance, and provides insights through statistical analysis and visualization.

## Dataset
The dataset consists of various features that influence the price of houses. The key attributes include:
- Area: Total area of the house in square feet
- Bedrooms: Number of bedrooms in the house
- Bathrooms: Number of bathrooms
- Stories: Number of floors in the house
- Parking: Availability of parking space
- Main Road Access: Whether the house is accessible from the main road (Yes/No)
- Guest Room: Presence of a guest room (Yes/No)
- Basement: Availability of a basement (Yes/No)
- Hot Water Heating: Whether hot water heating is available (Yes/No)
- Air Conditioning: Whether the house has air conditioning (Yes/No)
- Preferred Area: Whether the house is in a preferred area (Yes/No)
- Furnishing Status: Whether the house is furnished, semi-furnished, or unfurnished
- Price: The target variable (dependent variable) representing the cost of the house

## Project Structure
```
├── data/                        # Dataset files (if applicable)
├── images/                      # Visualizations and model performance plots
│   ├── Actual_vs_Predicted.png  # Scatter plot of actual vs predicted values
│   ├── Boxplots.png             # Categorical variable boxplots
│   ├── Residuals_Distribution.png # Residual histogram
│   ├── MSE_R2_Comparison.png    # MSE and R-squared scores across models
│   ├── OLS_Regression_Results.png # Summary of OLS regression results
│   ├── VIF_Analysis.png         # Variance Inflation Factor analysis
├── Housing_Multi_Linear_Regression.ipynb  # Jupyter notebook for analysis
├── requirements.txt             # Python dependencies
├── README.md                    # Project documentation (this file)
```

## Model Implementation & Evaluation
1. Data Preprocessing
- Checked for missing values and handled categorical variables.
- Performed **one-hot encoding** for categorical features.
- Scaled numerical variables where necessary.

2. Exploratory Data Analysis (EDA)
- Created boxplots to visualize the impact of categorical variables.
- Generated correlation matrices to understand feature relationships.
- Analyzed the distribution of residuals to check model assumptions.

3. Model Training & Comparison
- Ordinary Least Squares (OLS) Regression for feature significance analysis.
- Multiple Linear Regression (MLR) as the baseline model.
- Compared alternative models: Ridge Regression, Lasso Regression, Random Forest, and Gradient Boosting.
- Gradient Boosting performed the best with the highest R² score (0.697) and lowest MSE.

4. Model Performance Metrics
- Mean Squared Error (MSE): Measures the average squared difference between actual and predicted values.
- R² Score**: Indicates how well the model explains variance in housing prices.
- Variance Inflation Factor (VIF): Checked for multicollinearity among features.

## Key Insights
- Area, number of bedrooms, bathrooms, and stories strongly influence house prices.
- Air conditioning, preferred area, and furnishing status also have significant effects.
- Unfurnished homes are generally cheaper, while furnished homes command higher prices.
- Gradient Boosting outperformed other models, making it the best fit for this dataset.

## Future Improvements
- Experiment with feature engineering (interaction terms, polynomial features).
- Optimize hyperparameters using GridSearchCV.
- Try non-linear models like XGBoost or Neural Networks for better predictions.

## Author
Sweety Seelam
Feel free to contribute, raise issues, or reach out for collaboration at sweetyrao670@gmail.com.

