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

#### Ultrachemco
![ucmco - sa](https://user-images.githubusercontent.com/78731243/133252194-0902118a-3d30-4a2d-862c-c48c21db2d63.png)
![ucmco - fb](https://user-images.githubusercontent.com/78731243/133252222-0719135c-b200-475c-8568-845d9d67e780.png)

#### Tata Steel
![ts-sa](https://user-images.githubusercontent.com/78731243/133252453-8e839c5d-0a0d-48ba-ba5a-c12c4db9044a.png)
![ts-fb](https://user-images.githubusercontent.com/78731243/133252472-6c585d85-6878-4f4d-bc39-ad1602d1d8eb.png)

#### Power Grid
![pg - sa](https://user-images.githubusercontent.com/78731243/133252739-49a53c51-9663-47d6-80f9-fdd57bdd65fc.png)
![pg - fb](https://user-images.githubusercontent.com/78731243/133252751-d339ff58-11d6-45ad-83b6-105764229c40.png)

#### NTPC
![ntpc - sa](https://user-images.githubusercontent.com/78731243/133252951-9f898bdd-96de-49a2-b181-a00660a2a770.png)
![ntpc - fb](https://user-images.githubusercontent.com/78731243/133252957-ebabc86d-efc8-45a2-a1ac-385042a074b0.png)

#### Nestle
![nst - sa](https://user-images.githubusercontent.com/78731243/133253198-ccf8f701-cabd-494b-85d8-45610aa33dc4.png)
![nst - fb](https://user-images.githubusercontent.com/78731243/133253209-3bd855bd-0760-4aba-9aaa-db62ed53d4f2.png)

#### Maruti
![mar - sa](https://user-images.githubusercontent.com/78731243/133253364-ab58caa2-23da-4c32-85ba-544294d16769.png)
![mar - fb](https://user-images.githubusercontent.com/78731243/133253377-a39d5789-7742-4e70-ac87-457c1feac749.png)

#### Coal India
![ci - sa](https://user-images.githubusercontent.com/78731243/133253509-6686b1f1-b858-41a0-a894-ef35b997299f.png)
![ci - fb](https://user-images.githubusercontent.com/78731243/133253516-948e5437-6b85-453f-9f21-549a22b03a01.png)

#### Bajaj FinServ
![bj - sa](https://user-images.githubusercontent.com/78731243/133253623-bf0c6f18-06d1-4375-92d9-42ff5797d434.png)
![bj - fb](https://user-images.githubusercontent.com/78731243/133253638-28b69926-ee81-4aa7-a910-3e6233897e2e.png)

 
## Inference:
The Prophet model generally performs better for time series values having a certain cyclicality. In the case of stocks from the various industry sectors, this can possibly be the case as fundamentally we see some months with spiked sales of cars/fertilisers and so on.
Hence the Prophet model may outperform the ARIMA/ARIMAX models for some assets.

References - 
1. https://www.kaggle.com/rohanrao/a-modern-time-series-tutorial
2. https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/
3. https://www.scribbr.com/statistics/akaike-information-criterion/
4. https://thedatascientist.com/performance-measures-rmse-mae/
5. https://facebook.github.io/prophet/docs/quick_start.html
