# BizITProcessPredictionData

## Event logs
The event log data includes two CSV files:
- ```L2C.csv``` representing the synthetic data for a sample L2C order approval process
- ```BPI2012(A+O).csv``` representing the synthetically augmented data for BPI2012 (A+O) logs.

## Time series data
The file ```L2C_Time_Series_Data.h5``` contains time series data for the L2C order approval process, which consists of IT alerts encoded as binary signals and time-varying KPI values. It can be loaded as a pandas dataframe using the following code:
```
import pandas as pd
data = pd.read_hdf("L2C_Time_Series_Data.h5")
```
