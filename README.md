# House Price Prediction 

This repository contains code for predicting house prices based on a given dataset. Below, you will find a detailed explanation of the code and its functionality.

## Introduction

The goal of this code is to predict the prices of houses based on a provided dataset. This is a common problem in the field of machine learning and data analysis, where we aim to build a predictive model that can estimate the sale prices of houses based on various features.

## Dataset Description

The dataset contains the following columns:

- **ID:** A unique identifier for each property.
- **MSSubClass:** The building class.
- **MSZoning:** The general zoning classification.
- **LotArea:** Lot size in square feet.
- **SaleCondition:** Condition of sale.
- **SalePrice:** Dependent variable, representing the sale price of houses.

## Libraries Used

The code utilizes several Python libraries for data analysis and machine learning, including:

- `pandas` for data manipulation.
- `numpy` for numerical operations.
- `matplotlib` and `seaborn` for data visualization.
- `sklearn` for machine learning tools and metrics.
- `linear_model`, `RandomForestRegressor`, and `DecisionTreeRegressor` for regression modeling.

## Usage

1. **Read the Data:**

   The code starts by reading the training dataset from a CSV file named "train.csv" using the `pandas` library.

2. **Data Exploration:**

   - It checks the data type and information about the dataset.
   - Generates summary statistics to understand the data distribution.
   - Displays the names of columns in the dataset.

3. **Identify Outliers:**

   - The code identifies outliers in the `SalePrice` column using the Interquartile Range (IQR) method.
   - Outliers above a certain threshold (566,075) are removed from the dataset.

4. **Data Visualization:**

   - It creates pair plots to visualize relationships between features, especially focusing on the relationship with the target variable (`SalePrice`).
   - Heatmaps are generated to explore correlations between features.

5. **Data Preprocessing:**

   - The `Id` column is removed as it does not contribute to the prediction.
   - Categorical data is one-hot encoded to convert it into a numerical format.

6. **Split Data:**

   - The data is split into input features (`x_train`) and the target variable (`y_train`).

7. **Test Data:**

   - The test data is read from a CSV file named "test1.csv" and preprocessed in a similar way as the training data.

8. **Modeling:**

   - Two regression models are implemented: Linear Regression and Decision Tree Regression.
   - Model accuracy is evaluated on both the training and test datasets.

9. **Conclusion:**

   - The code concludes that Decision Tree Regression is more suitable for this dataset due to its non-linear nature.
   - It generates a CSV file containing predictions for the test data.

## Conclusion

This code demonstrates the process of predicting house prices using machine learning techniques. It provides insights into data exploration, preprocessing, modeling, and evaluation. The Decision Tree Regression model is recommended for accurate predictions on this dataset.

## References

- [pbpython.com](https://pbpython.com)
- [seaborn.pydata.org](https://seaborn.pydata.org)
- [machinelearningmastery.com](https://machinelearningmastery.com)
- [datascience.stackexchange.com](https://datascience.stackexchange.com)
- [wikipedia.org](https://wikipedia.org)
- [scikit-learn.org](https://scikit-learn.org)
- [journaldev.com](https://www.journaldev.com)
- [geeksforgeeks.org](https://www.geeksforgeeks.org)
- [datacamp.com](https://www.datacamp.com)
- [kaggle.com](https://www.kaggle.com)
- [programmersought.com](https://www.programmersought.com)
