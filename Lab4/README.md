# Support Vector Regression on Position Salaries Dataset

This notebook demonstrates Support Vector Regression (SVR) to model the relationship between position levels and salaries.

## Workflow

1. **Libraries**: Import `numpy`, `pandas`, `matplotlib`, and `sklearn`.  
   - These libraries are essential for data manipulation, visualization, and implementing machine learning algorithms. 
   - `numpy` is used for numerical operations, `pandas` for data handling, `matplotlib` for plotting, and `sklearn` for machine learning functionalities.

2. **Dataset**: Load `Position_Salaries.csv`.  
   - This CSV file contains information about various positions and their corresponding salaries, serving as the dataset for our analysis. 
   - Loading the dataset allows us to preprocess and explore the data for insights.

3. **Data Exploration**: Preview the dataset structure.  
   - Understanding the structure of the dataset helps identify features and the target variable, which are critical for building the model. 
   - This step includes checking the first few rows of the dataset, as well as examining data types and missing values.

4. **Feature Extraction**: Extract `Position Level` (X) and `Salary` (Y).  
   - In this step, we separate the independent variable (Position Level) from the dependent variable (Salary) for the regression analysis. 
   - This extraction is crucial as SVR will learn to predict salary based on the position level provided.

5. **Scaling**: Apply `StandardScaler` to both X and Y.  
   - Scaling is necessary for SVR, especially when using the RBF kernel, as it ensures that all features contribute equally to the model training. 
   - `StandardScaler` standardizes the features by removing the mean and scaling to unit variance, helping improve model performance.

6. **SVR Model**: Train an SVR model using the RBF kernel.  
   - The Radial Basis Function (RBF) kernel allows the SVR to fit non-linear relationships between position levels and salaries effectively. 
   - During training, the model learns the underlying patterns in the data, enabling it to make predictions on unseen data.

7. **Prediction**: Predict the salary for position level 6.5.  
   - After training, we can use the model to predict the salary for a specific position level (in this case, 6.5), demonstrating the application of SVR. 
   - This prediction provides insights into expected salaries based on the model’s learned patterns.

8. **Visualization**: Plot the actual data points and the SVR regression line.  
   - Visualization is key to understanding how well the SVR model fits the actual data. 
   - By plotting the actual salary data against the predicted values, we can visually assess the model's performance and accuracy.

## Prerequisites

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn
