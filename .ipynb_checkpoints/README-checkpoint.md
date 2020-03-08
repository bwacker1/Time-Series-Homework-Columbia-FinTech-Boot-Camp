# time-series-homework

In this assignment, I used both time series models and a linear regression model predict future movements in the exchange rate of the Japanese Yen against the US Dollar. 

Using 29 years of USDJPY exchange rate data (from January 1990 through October 2019) as an input, I ran the following models to make predictions on various aspects of the Yen over the next 5 trading days:
* ARMA Model - to forecast returns
* ARIMA Model - to forecast price
* GARCH Model - to forecast volatility

Based on these models, I predicted that returns on the Yen should decrease, its value should fall vs. the dollar, and volatility should rise. As such, I can draw the conclusion that it would be unwise to go long Yen at this time. However, due to a high p-value for each of these models, I cannot fully rely on the predictions they produced. 

Following this analysis, I used the same dataset to construct a linear regression model aimed at predicting returns for the yen. I trained the model on returns data from 1990 to 2018. Once trained, I fed this model both the in-sample data used to train the model and out-of-sample from 2019 to "predict" historical returns. When comparing the outputs of the in-sample and out-of-sample applications of this model, I found that the root mean squared error for the out-of-sample application was actually lower than for the in-sample application, giving me confidence that this model could be used to make somewhat accurate predictions on data it is not familiar with. 