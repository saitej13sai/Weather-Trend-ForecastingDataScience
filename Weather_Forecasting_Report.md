# Weather Trend Forecasting Report

## PM Accelerator Mission
To empower professionals with cutting-edge skills and accelerate their careers through hands-on, real-world tech projects.

## 1. Data Cleaning & Preprocessing
- **Missing Values**: Filled with column means where applicable.
- **Outliers**: Removed temperature values below -0.25°C or above 45.75°C using IQR.
- **Normalization**: Standardized temperature data.
- **Time Series**: Converted `last_updated` to datetime and set as index.

## 2. Exploratory Data Analysis
- **Temperature Trend**: Visualized over time (see `temperature_trend.png`).
- **Precipitation by Country**: Average precipitation for top 20 countries (see `precipitation_by_country.png`).
- **Correlations**: Analyzed relationships between temperature, precipitation, humidity, and wind speed (see `correlation_matrix.png`).

## 3. Model Building
- **Model**: ARIMA(5,1,0) for temperature forecasting.
- **Time Series**: Daily average temperature from `last_updated`.
- **Evaluation**: MAE = 1.19°C, RMSE = 1.29°C.
- **Forecast**: Next 7 days visualized (see `temperature_forecast.png`).

## 4. Insights
- Temperature varies widely (e.g., 1°C in Santiago, 38.4°C in Dhaka).
- Precipitation is sparse, with most regions showing 0 mm on sampled days.
- ARIMA model provides reasonable short-term forecasts with MAE of 1.19°C.

## 5. Conclusion
This analysis demonstrates basic data science skills in cleaning, EDA, and time series forecasting, aligning with the PM Accelerator mission.
