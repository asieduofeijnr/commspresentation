# Linear Regression for Hospital Infection Risk Prediction

## Introduction

This Python project demonstrates the concept of linear regression using the `plotly.express` library for data visualization. It focuses on predicting the infection risk (InfctRsk) in a hospital based on the length of stay (Stay) of patients. 

## Linear Regression

Linear regression is a statistical method used for modeling the relationship between a dependent variable (in this case, InfctRsk) and one or more independent variables (in this case, Stay). It assumes a linear relationship between the variables, which can be represented as:

InfctRsk = Bo + B1 * Stay


- `InfctRsk`: The dependent variable we want to predict (infection risk).
- `Stay`: The independent variable (length of stay).
- `B1`: The slope of the line (the change in InfctRsk for a unit change in Stay).
- `Bo`: The y-intercept (the value of InfctRsk when Stay is zero).

## Code Explanation

Here's an overview of the code:

1. Import necessary libraries: `plotly.express`, `pandas`, and `sklearn.linear_model`.

2. Load the dataset from the CSV file (`hospital_infection.csv`) into a Pandas DataFrame.

3. Extract the independent variable `Stay` and the dependent variable `InfctRsk` from the dataset.

4. Create a linear regression model using scikit-learn's `LinearRegression`.

5. Fit the model to the data to find the optimal values for `m` (slope) and `b` (intercept).

6. Calculate the slope and intercept of the regression line.

7. Create a scatter plot using Plotly Express to visualize the data points, and add a linear trendline using the calculated coefficients.

8. Add a text annotation to the plot with the equation of the regression line, displaying the values of `m` and `b`.

9. Display the plot showing the data points and the regression line.

10. Finally, the code calculates the infection risk (`infctRSK`) for a hypothetical length of stay (`stay = 10.5`) using the equation derived from the linear regression model.

## Running the Code

To run this code:

1. Clone this repository or download the `hospital_infection.csv` dataset.

2. Make sure you have the required libraries installed as mentioned above.

3. Execute the code in your Python environment.

## Conclusion

Linear regression is a fundamental machine learning technique used for predictive modeling. In this example, it helps us understand and predict hospital infection risk based on the length of stay. You can adapt this code and apply linear regression to various other real-world problems by adjusting the variables and dataset.
