# Insurance Claim Forecasting using ARIMA

This project applies the ARIMA (AutoRegressive Integrated Moving Average) model to forecast monthly vehicle insurance claim volumes using real-world data from Kaggle.

## Objective
To predict future insurance claims by building a statistically sound time series model based on historical monthly data.

## Dataset
- **Source**: Kaggle (Monthly vehicle insurance claims)
- **Features Used**: Date, Monthly Claim Volume

## Methodology
1. **Data Preprocessing**
   - Converted date column to datetime and set as index
   - Resampled data to monthly frequency

2. **Stationarity Check**
   - Conducted Augmented Dickey-Fuller (ADF) test
   - Differenced data to achieve stationarity

3. **Model Selection**
   - Analyzed ACF and PACF plots to identify potential AR and MA terms
   - Chose optimal ARIMA(p,d,q) parameters using AIC/BIC

4. **Model Fitting**
   - Fitted ARIMA model using `statsmodels`
   - Diagnosed residuals to validate model assumptions

5. **Forecasting**
   - Forecasted 12 future months of insurance claims
   - Visualized historical and predicted values

## Results
- Successfully generated a 12-month ahead forecast
- Residuals appeared white-noise, indicating a good fit
- Plots provided visual confirmation of model accuracy

## Tools Used
- Python
- Pandas, NumPy
- Statsmodels
- Matplotlib, Seaborn

## Author
Aahna Shresth  
[GitHub Profile](https://github.com/aahna-shresth)
