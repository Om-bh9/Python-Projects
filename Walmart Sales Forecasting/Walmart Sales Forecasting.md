# Weekly Sales Forecasting Project

## Project Overview

This project focuses on forecasting weekly sales for various retail outlets using historical data analysis and predictive modeling techniques. The goals include understanding the impact of external factors on sales trends and accurately predicting sales for the next 12 weeks.

## Problem Statement

### Analytical Goals:
1. Determine if weekly sales are influenced by:
   - Unemployment rates
   - Seasonal trends
   - Temperature variations
   - Consumer Price Index (CPI)

2. Identify top-performing and worst-performing stores based on historical sales data.

### Predictive Modeling Approach:
Due to missing data for upcoming weeks (e.g., holiday flags, temperature, CPI, unemployment), the approach excludes these variables from the modeling process. Instead, the focus is on utilizing time series forecasting models:

- **SARIMA (Seasonal ARIMA)**: Extends ARIMA to handle seasonal patterns in the data.
- **FBprophet (Facebook Prophet)**: Manages time series with multiple seasonalities and handles missing data and outliers.
- **Exponential Smoothing**: Models trends and seasonality by assigning exponentially decreasing weights to past observations.

These models are chosen for their ability to capture both linear trends and complex seasonal patterns in sales data.

## Steps Followed

### 1. Data Preprocessing
Data preprocessing involved cleaning and transforming raw data to ensure accuracy and completeness. This step laid the foundation for effective analysis and modeling.

### 2. Feature Engineering
Feature engineering focused on creating new variables (features) from the raw data. Features included date-based attributes (e.g., day of the week, month), lagged sales values, and store-specific characteristics.

### 3. Model Selection and Implementation
Selected SARIMA, FBprophet, and Exponential Smoothing for forecasting:
- **SARIMA**: Addressed seasonal variations in the data using seasonal differencing.
- **FBprophet**: Adapted to handle complex seasonal patterns and incorporate holidays and trend changes.
- **Exponential Smoothing**: Applied to capture trends and seasonal effects adaptively.

## Next Steps

Implement the forecasting models to predict weekly sales for each store over the next 12 weeks. Evaluate model performance and refine as needed based on forecast accuracy and insights gained from the analysis.

# Analysis of Weekly Sales and External Factors Impact

## Impact of Unemployment on Store Sales

### Correlation Analysis:
Analyzing correlation values reveals a significant trend between unemployment rates and weekly sales across stores. Notably, Store 38 (-0.785), Store 39 (-0.3846), and Store 44 (-0.780) show strong negative correlations. This indicates that as unemployment rates rise, these stores experience a decrease in weekly sales. Other stores exhibit weak or negligible correlations with unemployment.

## Seasonal Trends in Weekly Sales

### Holiday vs. Non-Holiday Sales:
Average sales during holidays are higher (1122887.89) compared to non-holidays (1041256.38). Most stores show a seasonal sales pattern, except for Stores 28, 30, 33, 36, 37, 38, 42, and 43, which exhibit distinct sales behaviors.

### Seasonal Peaks:
Sales peak during Thanksgiving and Christmas, reflecting increased consumer spending during these festive seasons.

## Impact of Temperature on Weekly Sales

### Analysis of Temperature Fluctuations:
Graphical analysis and correlation studies indicate minimal to no discernible impact of temperature fluctuations on weekly sales. Sales patterns remain consistent irrespective of temperature changes.

### Conclusion:
Sales peaks during festive seasons like Thanksgiving and Christmas dominate any potential influence of temperature fluctuations on weekly sales.

## Consumer Price Index (CPI) and Weekly Sales

### CPI Coefficients:
Stores show varied responses to changes in CPI:
- **Positive Coefficients**: Stores like 1, 3, 5, 7, 8, etc., experience higher weekly sales as CPI increases.
- **Negative Coefficients**: Stores like 2, 4, 6, 10, 14, etc., see decreased sales with higher CPI.

### Interpretation:
Positive CPI coefficients suggest increased spending capacity or willingness to purchase. Negative coefficients indicate sensitivity to price changes or consumer preferences for cheaper alternatives.

### Conclusion:
The impact of CPI on weekly sales varies across stores, reflecting different consumer behaviors and market segments.

---

This analysis provides insights into how external factors like unemployment, seasonal trends, temperature, and CPI influence weekly sales across various retail stores.

