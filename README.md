# BizITProcessPredictionData
This is the data for the research paper "Predicting Business Process Events in Presence of Anomalous IT Events" submitted to BPM 2023 TRACK II: ENGINEERING

The data includes two CSV files:
- ```L2C.csv``` representing the synthetic data for a sample L2C process
- ```BPI2012(A+O).csv``` representing the synthetically augmented data for BPI2012 (A+O) logs.

There is a third file, ```L2C_Time_Series_Data.h5``` containing time seies data for the L2C process containing IT alerts and KPI values. It can be loaded as a pandas dataframe using the following code:
```
import pandas as pd
data = pd.read_hdf("L2C_Time_Series_Data.h5")
```
