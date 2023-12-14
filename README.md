# Business and IT Observability Data

This data contains event logs and time series data for Business and IT Observability. Event log data contains business and IT events. Time Series data contains business (and possibly IT) KPIs and IT events.

The repository is organized in two ways:
- **Complete**: contains all the data in one place, categorized by type
- **Publication-wise**: contains all the data organized by publications, following the same nomenclature used in the published material. Also, the data format is made compatible with the source code pipeline for the particular publication.

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
