# Time Series Analysis on Fatal Car Accidents in Michigan

### Overview

This project focuses on analyzing time series data of fatal car accidents in Michigan using statistical modeling techniques. The objective is to identify patterns, trends, and seasonality in the data and develop predictive models to better understand accident occurrences.

### Data Description

The dataset is sourced from the National Highway Traffic Safety Administration (NHTSA) through the Fatality Analysis Reporting System (FARS). It contains monthly records of fatal car accidents in Michigan from 2008 to 2022.

### Methodology

**1. Exploratory Data Analysis (EDA)**

* Visualization of accident counts over time.

* Identification of trends and seasonal variations.

* Decomposition of time series data into trend, seasonal, and remainder components using STL decomposition.

**2. Stationarity Analysis**

* Conducted stationarity tests to assess whether differencing is required.

* Applied transformations such as log transformation and detrending to achieve stationarity.

**3. Autocorrelation Analysis**

* Examined the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) to identify patterns in lagged values.

* Used spectral analysis to detect dominant frequencies in the time series data.

**4. Time Series Modeling**

* ARMA Model: Used as a baseline model after ensuring stationarity.

* SARMA Model: Incorporated seasonal components based on findings from decomposition and ACF analysis.

* Model Selection: Compared models using AIC values and conducted likelihood ratio tests (LRT) to determine the best-fitting model.

**5. Forecasting**

* Generated predictions for future accident counts using the selected SARMA model.

* Evaluated forecasting performance using metrics such as MAPE and RMSE.

### Key Findings

* Fatal car accidents exhibit strong seasonality, peaking in summer months.

* ARMA(3,1) was initially selected as the best model, but further analysis revealed that incorporating seasonal components improved model performance.

* The SARMA(3,1) × (2,2)[12] model provided the best fit, effectively capturing seasonal trends while maintaining stable residuals.

* Residual analysis confirmed that the final model met the assumptions of stationarity and normality.

### Future Work

* Incorporate external factors such as weather conditions and traffic volume to improve model accuracy.

* Investigate additional seasonal effects beyond annual seasonality.

* Explore machine learning-based approaches for time series forecasting.


### References

[1] [Fatal Accidents Reporting System](https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/813556)

[2] [Time Series Analysis by Edward L. Ionides](https://ionides.github.io/531w25/)



### License

This project is for academic purposes and follows the guidelines of STATS531 at the University of Michigan.
