# Multivariate Time Series Forecasting 

## Data

The Dataset is fully dedicated for the developers who want to train the model on Weather Forecasting for Indian climate. This dataset provides data from 1st January 2013 to 24th April 2017 in the city of Delhi, India.

The 4 parameters here are:

* meantemp (target)

* humidity

* wind_speed

* meanpressure


After a detailed EDA process, I decided to continue with the first 3 features for modeling

## Modelling

Experimented with more than 6 different time series models and compared them:

  1. simple ARIMA (both daily and monthly forecast)

  3. simple SARIMA (both daily and monthly forecast)
  
  5. auto_arima (finds p, q, and d automatically - monthly forecast)
  
  7. Prophet (daily forecast)
    
  9. RNN (daily forecast)
    
  11. LSTM (daily forecast - classic and bidirectional)
    
  13. GRU (daily forecast)


## Results:

1. Deep learning models resulted in the best scores 

2. ARIMA models in both daily and monthly forecasts resulted in very low accuracy, whereas in monthly predictions SARIMA and auto_arima modeling performed better

3. The Prophet model got a very high accuracy in the daily forecast (but lower than DL models)

## Conclusion

After exploring various time series models in detail and leveraging advanced visualizations, I've concluded that Prophet is my preferred choice among the other models. Despite testing over 6 models in a multivariate time series, Prophet's simplicity, performance, and cost-effectiveness make it the standout solution.

I have found that Prophet is able to deliver comparable results to deep learning models without the complexity and resource-intensive training they require. Unlike traditional ARIMA models, it offers a user-friendly interface and requires minimal parameter tuning, making it accessible to users with varying levels of expertise. Also, Prophet's robustness to outliers and its ability to handle irregularly spaced data add to its appeal.

Thanks to everyone for reviewing this notebook! I would appreciate an upvote if you liked it. Also, I'm curious about your thoughts, so please leave a comment to help me improve.
