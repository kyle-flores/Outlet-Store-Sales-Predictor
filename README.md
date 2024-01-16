# Outlet Store Sales Predictor: Project Overview
- Developed and refined a model that predicts product sales for an outlet store, leveraging over 8000 records of product sales
- Explored patterns and discovered meaningful insights through various forms of data visualization after several steps of data cleaning
- Evaluated Linear Regression, Random Forest Regressor, Gradient Boosted Regressor, and other models to procure the best model for this scenario, as scored by accuracy and Root Mean Squared Error (RMSE)
- Tuned the best model, Lasso, using GridSearchCV to enhance performance and proficiency
This model has real world appliations in multiple forms, such as forecasting store business and economic trends.

## Tools Used
**IDE:** Jupyter Notebook

**Language:** Python

**Packages:** Pandas, Numpy, Seaborn, Matplotlib, Scikit-learn, Sci-Py

**Dataset:** https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets/data

## Data Cleaning

The original dataset was riddled with intricacies that hindered data readability and comprehension, prompting these changes to be made:
- Correctly assigned numerical and categorical features to separate lists
- Outlier removal
- Clarified values in "Item Identifier" feature
- Regrouped separate but equivalent values in"Item Fat Content"
- Null value treatment
  - Approach 1: Dropping rows with null values
  - Approach 2: Filling in null values with either feature mean or mode

## Exploratory Data Analysis
Numerous graphs displayed patterns and trends within the data
