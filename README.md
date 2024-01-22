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

**Dataset:** https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets/data(url)

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

Numerous graphs were created to visualize patterns and trends within the data.

![Graph 1](https://github.com/kyle-flores/Outlet-Store-Sales-Predictor/assets/153465652/28e77d30-889c-4192-86f1-ff7d49846964)

![Graph 2](https://github.com/kyle-flores/Outlet-Store-Sales-Predictor/assets/153465652/77f2e477-0ed2-4df8-a2db-27293cbcc35f)

## Preprocessing the Data
The null values were dealt with in 2 different approaches. The first approach completely dropped the rows with null values and the second approach filled in the null values with the mean if the column was a numerical column, or filled in with the mode for the categorical feature. This resulted in two different datasets. For both datasets, outliers were removed and categorical variables were transformed into dummy variables. The data was then split into training and test sets in 80-20 split.

## Model Building
Several different models were used to predict the outlet sales due to the characteristics of the data. Some of these models include Lasso, Random Forest, XGB, and Linear Regression models.

## Model Performance

Performance of the models were evaluated based on accuracy and on RMSE (Root Mean Squared Error). RMSE was chosen as the performance metric because of it's interpretability as well as being a commonly used metric.

![image](https://github.com/kyle-flores/Outlet-Store-Sales-Predictor/assets/153465652/5f725233-f44f-4102-a88e-e29ce4979742)

The best performing models were the Lasso, Ridge, and Linear Regression models. They had the lowest overall RMSEs. Gradient Boost Regressor had a lower RMSE for Approach 2, however, the accuracies between the training and test sets varied, meaning that it was likely overfitting and adapted too well to the training set, preventing it from achieving a similar accuracy in predicting the test set.

The best model performance was about 53% accuracy and a RMSE of 1040. However, different approaches at manipulating the data resulted in higher model performances, meaning that other approaches could be experimented on to reach upwards of 90% accuracy and smaller RMSEs.
