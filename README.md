# TimeSeries_World_Carbon_Emission
1. We will use ARIMA (Time Series) model to predict CO2 emissions of a country for each year since 1900.
2. We can also use AUTO_ARIMA library to expedite the process and calculate the ACF, PACF and difference part of the equation
3. SARIMA model could be used in dataset that have seasonality component to it. For example - AC sales, Ice Cream sales. We would use a seasonality component to the ARIMA model to convert it to SARIMA

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/c4ba19a8-33f4-44f6-976d-9abe717a92da)


__Source__ : https://ourworldindata.org/co2-emissions

* For this analysis, we will only analyze CO2 emissions by USA

## Explanation of Steps : 

Step 1 : Plotting how the data looks and how has the carbon emission been by the USA since 1900

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/5cc085d1-b543-4889-b69d-8e5a81742737)

Step 2 : Divide the dataset into Seasonal, Trend and Residual component to analyze it better

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/5de8fe17-0e26-4561-be87-4ed3261d5e49)

Step 3 : Use Ad-Fuller test to check for stationarity of the data. If data is not stationary, use First difference method to convert it into stationary data

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/dde31645-1609-4136-894b-31f624054be9)

Step 4 : Plot the AutoCorrelation and Partial-Autocorrelation chart to find the ACF and PACF component of ARIMA model

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/7143302d-8cb1-40c0-ac9b-6ad85223f705)
![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/c08ad15d-bedb-412b-99fb-73ec328795d9)

Step 5 : Fit the ARIMA model with the ACF and PACF component and plot the residual graph. Make sure it is a bell-curve

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/10ce6716-68dd-4f63-bcbc-ddc264c09eb6)

Step 6 : Plot the predicted results

![image](https://github.com/SrijanDeo-DA-DS/TimeSeries_World_Carbon_Emission/assets/88278620/85d6dadd-e8f3-4545-ac33-0d05b491b778)



