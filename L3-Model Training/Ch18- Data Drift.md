**Lesson 3:Model Training**

# Chapter 18 - Data Drift

Change in input data overtime, that may often affect the performance of the model
## Causes

- **Natural drift in data**- A change in customer behavior over time.
- **Data quality issues**- A sensor breaks and starts providing inaccurate readings
- **Upstream process changes**- A sensor is replaced, causing the units of measurement to change (e.g., from minutes to seconds).
- **Covariate shift/Change in relationship between features** -Decreasing the number of features

## Monitoring Data Drift
 
Scenarios for setting up  dataset monitors
- Monitoring a model's input data for drift from the model's training data
- Monitoring a time-series dataset for drift from a previous time-period
- Performing analysis on past data


### monitoring data drift process

- Specifying a baseline dataset – usually the training dataset
- Specifying a target dataset – usually the input data for the model
- Comparing these two datasets over time, to monitor for differences

### Other compasirons
- Comparing input data vs. training data. This is a proxy for model accuracy; that is, an increased difference between the input vs. training data is likely to result in a decrease in model accuracy.
- Comparing different samples of time series data. In this case, you are checking for a difference between one time period and another. For example, a model trained on data collected during one season may perform differently when given data from another time of year. Detecting this seasonal drift in the data will alert you to potential issues with your model's accuracy.

