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

Numerous graphs were created to visualize patterns and trends within the data.

![Graph 1](https://github.com/kyle-flores/Outlet-Store-Sales-Predictor/assets/153465652/28e77d30-889c-4192-86f1-ff7d49846964)

![Graph 2](https://github.com/kyle-flores/Outlet-Store-Sales-Predictor/assets/153465652/77f2e477-0ed2-4df8-a2db-27293cbcc35f)

## Preprocessing the Data
The null values were dealt with in 2 different approaches. The first approach completely dropped the rows with null values and the second approach filled in the null values with the mean if the column was a numerical column, or filled in with the mode for the categorical feature. This resulted in two different datasets. For both datasets, outliers were removed and categorical variables were transformed into dummy variables. The data was then split into training and test sets in 80-20 split.

## Model Building
Several different models were used to predict the outlet sales due to the characteristics of the data. Some of these models include Lasso, Random Forest, XGB, and Linear Regression models.

## Model Performance

To assess the performance of various models in predicting outlet sales, we utilized metrics such as accuracy and Root Mean Squared Error (RMSE). RMSE was chosen due to its interpretability and common usage as a performance metric.

![Model Performance](https://github.com/kyle-flores/Outlet-Store-Sales-Predictor/assets/153465652/5f725233-f44f-4102-a88e-e29ce4979742)

### Best Performing Models

The Lasso, Ridge, and Linear Regression models emerged as the top performers, exhibiting the lowest overall RMSEs. While the Gradient Boost Regressor displayed a lower RMSE for Approach 2, discrepancies in accuracies between the training and test sets suggested potential overfitting. This model appeared to adapt too well to the training set, hindering its ability to generalize to the test set.

### Insights and Implications

The best-performing models achieved approximately 53% accuracy with an RMSE of 1040. However, alternative data manipulation approaches resulted in higher model performances, hinting at the potential for further experimentation.

In conclusion, the choice of data manipulation methods significantly influences model outcomes. The current best model offers valuable insights, but continuous experimentation with different approaches may lead to even more accurate predictions and smaller errors in forecasting outlet store sales.
 

## Conclusion

In this project, a model was successfully developed and refined for predicting outlet store sales. Through  data cleaning, exploratory data analysis, and model evaluation, valuable insights into the dataset were obtained.

The best-performing models, Lasso, Ridge, and Linear Regression, showcased promising accuracy and Root Mean Squared Error (RMSE). Despite achieving a moderately low accuracy of approximately 53% with an RMSE of around 1040, the exploration of alternative data manipulation approaches hinted at the potential for greater performance.

The real-world applications of this model are diverse, including the forecasting of store business and economic trends. Business owners could use this model to ensure that they are stocked and prepared for the upcoming business.

