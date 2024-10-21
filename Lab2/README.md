# Linear Regression Models: Single Variable & Multivariable

This repository demonstrates two types of linear regression models: **Single Variable Linear Regression** and **Multivariable Linear Regression**. Both of these methods are useful for predicting continuous outcomes, but they are applied in different contexts.

---

## What is Linear Regression?

Linear regression is a method used to predict a target variable (usually continuous) based on the relationship between it and one or more independent variables (predictors). The idea is to find the best-fitting line that minimizes the differences between the actual values and the predicted values.

---

## 1. Single Variable Linear Regression

### Real-World Example: Predicting House Prices Based on Area

Consider a scenario where you want to predict the **price of a house** based on its **area (in square feet)**. Here, **area** is the only factor affecting the price.

The model would assume a **linear relationship** between house price and area. The equation for predicting the price might look like this:


Price = \beta_0 + \beta_1 times Area


Where:
- **Price** is the dependent variable (what we're predicting).
- **Area** is the independent variable.
- **\(\beta_0\)** is the intercept (the base price of a house with zero area, which is practically a starting point).
- **\(\beta_1\)** is the slope (how much the price increases for each additional square foot).

### Use Case

Single variable linear regression is often used when:
- There is **one main factor** influencing the outcome.
- You want a simple and interpretable model.

For example, in the real estate market, you might be able to accurately predict the price of houses in a specific neighborhood using just the area of the house as a predictor, assuming other factors like location and condition are constant.

---

## 2. Multivariable Linear Regression

### Real-World Example: Predicting Salary Based on Experience, Education, and Location

Imagine you're an HR analyst trying to predict an employee's **salary** based on several factors like:
1. **Years of Experience**
2. **Education Level** (e.g., Bachelor's, Master's, PhD)
3. **Location** (city or country where the employee works)

The salary in this case depends on **multiple factors**, so a multivariable linear regression model would be more suitable. The equation could be:

Salary = \beta_0 + \beta_1[Experience] + \beta_2[Education Level] + \beta_3[Location]


Where:
- **Salary** is the dependent variable.
- **Experience, Education Level, and Location** are the independent variables.
- **\(\beta_0, \beta_1, \beta_2, \beta_3\)** are the coefficients that measure the effect of each feature on the salary.

### Use Case

Multivariable regression is ideal when:
- The outcome is influenced by **multiple factors**.
- You want to capture the **combined effect** of these variables on the target.

For example, predicting an employee's salary in a company might require knowledge of their experience, educational background, and location, as these factors often affect how much someone earns.

---

## Key Differences Between Single and Multivariable Regression

- **Single Variable Regression** deals with **one independent variable** and is often used when the outcome can be primarily explained by one feature. It's simple, interpretable, and effective for specific use cases.
  
- **Multivariable Regression** deals with **two or more independent variables**, making it suitable for complex scenarios where multiple factors affect the outcome. It's more flexible but requires more data and analysis.

---

## Summary

Both single variable and multivariable regression are powerful techniques that can be applied to various real-world problems:
- Use **single variable regression** when only one feature is important for prediction.
- Use **multivariable regression** when multiple factors need to be considered simultaneously.

---

## How to Run the Code

This repository includes Jupyter Notebook files that demonstrate both types of linear regression using Python's `scikit-learn` library. You can run these examples on any machine that supports Python, or upload them directly to Google Colab for easy execution.

---

## Dependencies

- Python 3.x
- Pandas
- Scikit-learn
- Matplotlib (for visualizations)

