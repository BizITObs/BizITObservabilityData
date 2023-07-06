# BizITProcessPredictionData

## Event logs
The event log data is present in the ```Event Logs``` folder. 
It contains two CSV files:
- ```L2C.csv``` representing the synthetic data for a sample L2C order approval process
- ```BPI2012(A+O).csv``` representing the synthetically augmented data for BPI2012 (A+O) logs.

## Time series data
The time series data is present in the ```Time Series``` folder.

This folder contains three subfolders, representing: 
- the original data
- the data with ground truth relations
- the data with pruned relations where the pruning is done using the PC-stable algorithm available [here](https://github.com/jakobrunge/tigramite).

Each folder contains at least the following two .h5 (HDF formatted) files:
- ```SO_data.h5``` representing the data for a Sales Order process
- ```Simulated_data.h5``` representing the data for the simulated process based on the above Sales Order process.

In addition, the `Original` folder contains the following .h5 (HDF formatted) file:
- ```L2C_data.h5``` representing the data for an Order Approval process

These datasets consist of IT alerts encoded as binary signals and time-varying KPI values. Any .h5 file can be loaded as a pandas dataframe using the following code:
```
import pandas as pd
data = pd.read_hdf("<path_to_data_file>")
```
