# Time-series-Japanese-Yen-

Introduction
This project focuses on analyzing and forecasting Japanese Yen exchange rates using time series analysis techniques. The dataset contains daily exchange rates of Indian Rupee to Japanese Yen.

Table of Contents
Introduction About the Dataset Data Preprocessing Exploratory Data Analysis (EDA) Time Series Decomposition Stationarity Test Auto-Correlation Analysis ARIMA Model Implementation Forecasting Conclusion

About the Dataset
The dataset contains daily exchange rates of Indian Rupee to Japanese Yen. The key features include:

Date: Date of the exchange rate Yen: Exchange rate of Indian Rupee to Japanese Yen

Data Preprocessing
Loading Data:
Loaded the dataset into a pandas DataFrame for inspection.

Handling Missing Values:
Converted exchange rate values to float and handled missing values by dropping them.

Date Conversion:
Converted the Date column to datetime format and set it as the index.

Exploratory Data Analysis (EDA)
Visualizing Time Series:
Plotted the time series data to visualize the exchange rate trends over time.

Filtering Data:
Filtered the data for the period from 1-Jan-2022 to 1-Jan-2023.

Time Series Decomposition
Decomposing the Time Series:
Used the seasonal_decompose function to decompose the time series into its components (trend, seasonality, and residuals). Plotted the components to analyze the structure of the time series.

Stationarity Test
Augmented Dickey-Fuller Test:
Applied the Augmented Dickey-Fuller test to check the stationarity of the time series. Analyzed the test results to determine if the series is stationary or not.

First Difference:
Calculated the first difference of the time series to make it stationary. Re-applied the Augmented Dickey-Fuller test on the differenced series to check for stationarity.

Auto-Correlation Analysis
Plotting Auto-Correlation:
Plotted the auto-correlation function (ACF) of the original and first-differenced time series to analyze the correlations at different lags.

ARIMA Model Implementation
Building the ARIMA Model:
Built an ARIMA model with order (5,1,1) using the differenced time series.

Fitted the model and summarized the results.
Plotting Fitted Values:
Plotted the original time series and the fitted values from the ARIMA model to visualize the model's performance.

Forecasting
Making Predictions:
Forecasted the exchange rates for the next few days using the ARIMA model. Compared the forecasted values with the actual values for a short test period.

Conclusion
The analysis demonstrated the application of time series analysis techniques, including decomposition, stationarity tests, auto-correlation analysis, and ARIMA modeling for forecasting exchange rates. Key findings include:

The original time series was non-stationary, but taking the first difference made it weakly stationary. The ARIMA model provided reasonable forecasts for the exchange rates based on the historical data. These insights highlight the utility of time series analysis in understanding and predicting trends in financial data. The approach can be applied to various time series forecasting scenarios, such as stock prices, sales, and economic indicators. ​​
