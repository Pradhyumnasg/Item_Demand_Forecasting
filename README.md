# Item_Demand_Forecasting
"The goal of a demand forecasting project is to help businesses optimize their inventory levels, production schedules, and pricing strategies"
code is for time-series forecasting using different regression models like Linear Regression, Random Forest Regression, and XGBoost Regression.

The dataset is loaded from the 'project2data.csv' file using Pandas library, then the date column is converted into datetime format. Further, new columns of year, month, and day are added to the dataset using the Pandas library.

Then, the dataset is filtered to select the data for a specific store and item. The dataset is prepared for time-series forecasting by first grouping the data by month and then taking the difference between consecutive months. The resulting dataset is then used to create a supervised learning problem by using a sliding window approach to create features for the input and target variable.

MinMaxScaler is used to normalize the dataset, and then it is split into train and test sets. Linear Regression, Random Forest Regression, and XGBoost Regression models are trained on the train set and evaluated on the test set using various performance metrics like RMSE, MAE, and R2 score. Finally, the predicted values are plotted against the actual values.
