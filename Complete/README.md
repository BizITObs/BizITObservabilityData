# Business and IT Observability Data

This data contains event logs and time series data for Business and IT Observability. Event log data contains business and IT events. Time Series data contains business (and possibly IT) KPIs and IT events.

## Event logs
The event log data is present in the ```Event Logs``` folder. 
It contains two CSV files:
- ```L2C.csv``` representing the synthetic data for a sample L2C order approval process
- ```BPI2012(A+O).csv``` representing the synthetically augmented data for BPI2012 (A+O) logs.

## Time series data
The time series data is present in the ```Time Series``` folder.

This folder contains three subfolders:
- **SO**: consists of a small `Original` dataset representing the data for a real-world Sales Order process and a larger `Simulated` dataset for a simulated process based on this Sales Order process.
- **RobotShop**: contains the service-level and application-level data for the Robot Shop application monitored by Instana.
- **L2C**: contains the data for an Order Approval process based on a real-world Lead-to-Cash process.

These datasets consist of IT alerts encoded as discrete events and time-varying KPI values. Data is available in two formats: `.csv` and `.h5`.

Any `.csv` file can be loaded as a pandas dataframe using the following code:
```
import pandas as pd
data = pd.read_csv("<path_to_data_file>", index_col=0)
```

Any `.h5` file can be loaded as a pandas dataframe using the following code:
```
import pandas as pd
data = pd.read_hdf("<path_to_data_file>")
```
