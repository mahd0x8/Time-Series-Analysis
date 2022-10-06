# Time-Series-Analysis
In this project different Time series models are implemented like ARIMA, SARIMA, SARMA and ARMA with a Passenger of a flight data set.

Time series is the data which changes over a period. An example of this would be stock price or sales growth. There are a few models which allow us to analyze Time series. These models allow us to forecast the observation based on the historical data of the previous time phases for the same observation. A small condition to this prediction method is to know whether the data is stationary or not, if it is not stationary then we apply the differencing factor and conduct the tests once more to check for its prediction and how accurate it may be.

We conduct the Dicky fuller test using Adfuller from statsmodel.
Dicky Fuller Test is Implimented. A lot of tests are available to test if your time series stationary or non-stationary. DT or Dicky Fuller test is the test which determines and sets apart stationary from non-stationary data. But before going to discuss dicky fuller test we check graphically if our graph shows curve according to the below figure then our series will be nonstationary. And if our graph curve is moving in such a way that the average and time both increase together then series will be stationery.

Adfuller function calculate ADF statistics, lags, p-value and critical value. We notice p- value, if p-value is below 0.05 then series will be stationary on the other hand if value will be greater than or equal to 0.05 then the series shows nonstationary behavior. Critical values are the probability of a series to be stationary for example, at 99% its -3.48, 95% -2.88 and 90% it’s - 2.57.

o ACF (Auto-Correlation Function) 
  The correlation coefficients between lagged values can be plotted to form the autocorrelated function also known as correlogram. 
o PACF (Partial Auto-Correlation Function) 
  PACF is a plot that shows the correlation of a series with its lagged values. You can determine the ARIMA model's AR and MA components using the ACF and PACF plots. ACF and PACF plots can be used to determine both seasonal and non-seasonal AR and MA components.ACF and PACF are used to find values for P, D, Q in ARIMA model.
  
  ARIMA model is one of the most Used models to predict the outcome of the future events Which have Occurred with respect to Time. This model Is used when we have Nonstationary data. First if it’s confirmed our data is non-Stationary then we have to performance of our model For which we have to train our model and then test it with known values. Then we will find the difference in between.
  
 Just like ARIMA that is used to predict in a linear pattern we use seasonal ARIMA that predicts the output in a seasonal manner. In SARIMA model four new hyper parameters are included in existing ARIMA model for the conversion that are seasonal (p,d,q) or seasonal order and frequency.
 
 ARMA is combined from AR (Auto-Regressive) and MA (Moving Average). It means when we are predicting future, we will consider impact of previous lags as well as residual too.
 
 The SARMA model deals with the ARMA model however in the context of seasonality. The python code for this was not implemented since there were not that many sources and the implementation was a bit more difficult than the rest.
 
 Complete details of our implimentations are available in Report.
