🔋 Energy Consumption Time Series Analysis
Project Overview
The project focuses on analyzing historical energy consumption data to uncover trends, seasonal patterns, and forecast future consumption. The goal is to provide stakeholders with insights that support resource planning and energy optimization decisions.

🎯 Objectives
Trend Analysis: Understand the changes in energy consumption over time.
Pattern Recognition: Identify seasonal trends and anomalies in the data.
Forecasting: Build predictive models to forecast future energy consumption.
Insights for Decision-Making: Offer actionable insights to help with energy resource planning and optimization.

📊 Dataset Details
Time Index: Daily data from January 1973 to January 2021.
Energy Consumption: Total energy consumed each day.
Sample Data:
Date	Total Energy Consumed (kWh)
1973-01-01	1957.641
1973-01-02	1712.143
1973-01-03	1510.079
1973-01-04	1183.421
1973-01-05	1006.326
🛠️ Data Preprocessing
The following steps were implemented to ensure data quality and readiness for analysis:

Data Cleaning: Removed whitespaces from column names and ensured consistency.
Outlier Handling: Applied the Interquartile Range (IQR) method to detect and replace outliers with rolling mean values.
Stationarity Checks: Conducted the Augmented Dickey-Fuller (ADF) test for stationarity and applied differencing when necessary.

📈 Methodology
1. Data Import & Initial Exploration
Loaded and explored the dataset.
Checked for missing values and visualized initial trends.
2. Exploratory Data Analysis (EDA)
Performed time series decomposition to analyze trend, seasonality, and noise.
Created visualizations to identify anomalies and seasonal patterns in energy consumption.
3. Model Building
Linear Regression: Developed baseline models using lagged features to predict future consumption.
ARIMA Model: Tuned the ARIMA model using pmdarima for automatic parameter selection, but the Linear Regression model ultimately outperformed.
4. Model Evaluation
Models were evaluated using standard metrics:
RMSE (Root Mean Square Error)
MAE (Mean Absolute Error)
MAPE (Mean Absolute Percentage Error)

🔍 Key Findings
Seasonal Trends: The data displayed strong seasonal patterns, with peaks in energy consumption during certain months each year.
Outlier Impact: Proper outlier management played a crucial role in improving model accuracy.
Best Model: The Linear Regression model provided the best results based on evaluation metrics, proving to be the most reliable for forecasting energy consumption.

📝 Conclusion
While ARIMA demonstrated potential, the Linear Regression model emerged as the most effective tool for predicting future energy consumption based on historical data. This analysis underscores the significance of statistical techniques and predictive modeling in energy management, offering valuable insights for optimizing energy consumption and planning for future demands.
