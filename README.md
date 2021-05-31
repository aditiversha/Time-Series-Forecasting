# Time-Series-Forecasting

## Objective: To forecast the closing price using (I)ARIMA (II)FBprophet

Requirement:
<li>ARIMA (pip install pmdarima)</li>
<li>FBprophet (pip install fbprophet)</li>
<li>Dataset from Data Source : https://www.kaggle.com/rohanrao/nifty50-stock-market-data</li>
  
 ### Approach
 1. Read data files.
 2. Define predictors (i.e exogenous variables for multivariate forecasting).
 3. Compute mean and standard deviation of the predicters (rolling window - 3 days, 7 days, 30 days).
 4. Data Manipulation using pandas.
 5. Perform ARIMA forecasting & plot the results.
 6. Compute RMSE & MAE of ARIMA model.
 7. Perform FBProphet forecasting & plot the results.
 8. Compute RMSE & MAE of FBprophet model.
 9. Plot & compare the results

### Output images

#### ARIMA forecasting
![1](https://user-images.githubusercontent.com/78731243/120175584-0301e880-c224-11eb-86fd-a7c3ecc3819c.png)


#### FBprophet
![2](https://user-images.githubusercontent.com/78731243/120175614-08f7c980-c224-11eb-8387-7506cbbc3e82.png)


#### ARIMA vs FBprophet
![3](https://user-images.githubusercontent.com/78731243/120175648-10b76e00-c224-11eb-9c9b-d03234c631e6.png)

## Observation: 
RMSE of Auto ARIMAX: 3.49
RMSE of Prophet: 4.71

MAE of Auto ARIMAX: 2.72
MAE of Prophet: 3.97


References - 
1. https://www.kaggle.com/rohanrao/a-modern-time-series-tutorial
2. https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/
3. https://www.scribbr.com/statistics/akaike-information-criterion/
4. https://thedatascientist.com/performance-measures-rmse-mae/
5. https://facebook.github.io/prophet/docs/quick_start.html
