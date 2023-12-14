# Business and IT Observability Data

This data contains event logs and time series data for Business and IT Observability. Event log data contains business and IT events. Time Series data contains business (and possibly IT) KPIs and IT events. 

There are currently 4 publications using this data:

- AutoMixer for Improved Multivariate Time-Series Forecasting on Business and IT Observability Data (IAAI 2024)
- Forecasting the Impact of Anomalous Events on Business Process Performance (CODS-COMAD 2024)
- Predicting Business Process Events in Presence of Anomalous IT Events (CODS-COMAD 2024)
- Towards Business Process Observability (CODS-COMAD 2024)

The data in this folder follows the same nomenclature used in the published material. In particular, the `SO` data used for "AutoMixer for Improved Multivariate Time-Series Forecasting on Business and IT Observability Data" is the same as the `Simulated` data used for "Forecasting the Impact of Anomalous Events on Business Process Performance". It is also referred to as `Simulated` data in the unified nomenclature used in the **Complete** folder.  Also, the data format in a folder specific to a particular publication is made compatible with the source code pipeline for that publication.

## Data formats
Data is available in two formats: `.csv` and `.h5`.  

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
