# Unit_10_Assignment-

## Time Series Analysis 
In this notebook we: 
* Import libraries and their dependencies. 
* Construct a dataframe with JPY/CAD prices between 1982 and 2020. 
* Plot the initial price time series from 1990-2020. 
* Identify patterns based on our time series plot above. 
* Decompose the 'Price' (i.e. closing price) column of our dataframe into trend and noise, using a Hodrick-Prescott Filter. 
* Construct a new dataframe with renamed columns displaying noise and trend (from the ts_trend, ts_noise, and price_df dataframes). We name the new dataframe price_noise_trend_df. 
* Plot the Exchange Rate Price vs. the Trend for 2015 to the present. 
* Identify long and short-term patterns from the plot above. 
* Plot the noise from the settle price. 
* Create a stationary percentage change series based on closing prices. 
* Estimate a (2,1) ARMA model based on the percentage changes computed above. 
* Plot a 5 day exchange rate forecast based on our ARMA model. 
* Conclude that the ARMA model is not a good fit, given the high p-value of its 2nd lag. 
* Forecast the exchange rate using an ARIMA model, and conclude that the ARIMA model is also not a good fit due to the elevated p-values of all its lags. 
* Forecast volatility using GARCH. 
* Conclude that the GARCH model is a good fit, given its very low p-values. 
* Plot volatility over the following 5 days. 
* Offer our conclusions on whether (1) we should buy the yen now, (2) the risk of the yen is expected to increase or decrease, and (3) whether we feel confident using the models for trading. 

## Regression analysis
In this notebook we: 
* Prepare a dataframe using the same .csv file in the prior section. 
* Slice the dataframe for periods from 1990. 
* Create a return column which we add to our dataframe. 
* Create a lagged return column using the shift function. 
* Create a train/test split for the data using 2018-2019 for testing and the rest for training. 
* Create 4 dataframes (1): X_train (training set using just the independent variables), X_test (test set  of just the independent variables). 
*  Create 4 dataframes (2): Y_train (training set using just the "y" variable, i.e., "Futures Return"), Y_test (test set of just the "y" variable). 
*  Create a Linear Regression model and fit it to the training data. 
*  Fit a SKLearn linear regression using  just the training set (X_train, Y_train). 
*  Make predictions using the Testing Data. 
*  Evaluate the model using "out-of-sample" data (X_test and y_test). 
*  Evaluate the model using in-sample data (X_train and y_train)
*  Conclude that, based on the test data's lower RMSE, the model performs better on out-of-sample data compared to in-sample data. 
