# Time-Series-Forecasting

## Objective: To forecast the closing price of Tata Motors using (I)ARIMA (II)FBprophet

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
![download](https://user-images.githubusercontent.com/78731243/119270339-d5141700-bc19-11eb-8d49-32b472e68b1e.png)

#### FBprophet
![download (1)](https://user-images.githubusercontent.com/78731243/119270356-eb21d780-bc19-11eb-85b0-41eab268588d.png)

#### ARIMA vs FBprophet
![download (2)](https://user-images.githubusercontent.com/78731243/119270384-14426800-bc1a-11eb-9d74-2718c55358c6.png)

## Inference: Since the values of RMSE and MAE of FBprophet are less than Auto Arima, we can conclude that FBprophet performed better than Auto Arima at forecasting the Time Series.
