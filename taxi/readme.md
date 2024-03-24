*Project: Taxi order forecasting*

The taxi company accumulated historical data about number of taxi orders at airports. They want to get a forecast about number of orders for every next hour with a purpose to attract more cars in time of maximal load. We have to build ML model for such predictions. The level of RMSE on test data must be less than 48.

Working on this project we resampled data for 1 hour. A time series analysis and an assessment for stationarity were carried out, and seasonality and trend graphs were constructed.

The Dickey-Fuller test doesn't allowed us to reject the null hypothesis about the non-stationarity of the series.

In order to make the dataset more stationary the feature engineering was performed.

Predictions of the number of orders for each hour were obtained using the exponential average method and added to the main dataset;

The next step was to add a number of new features to the dataset; after dividing the dataset into train/test, empty values ​​were removed from the training set. 2 models were trained - DecisionTreeRegressor and LightGBM, hyperparameters were selected on cross-validation for both models.

Model testing results showed that the best model is LGBMRegressor, the model can give a fairly good forecast for next hour.
