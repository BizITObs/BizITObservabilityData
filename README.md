# Business and IT Observability Data

This data contains event logs and time series data for Business and IT Observability. Event log data contains business and IT events. Time Series data contains business (and possibly IT) KPIs and IT events.

The repository is organized in two ways:
- **Complete**: Contains all the data in one place with a unified nomenclatuure. 
- **Publication-wise**: Contains all the data organized by publications, following the same nomenclature used in the published material. Also, the data format is made compatible with the source code pipeline for the particular publication.

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

## Citation
If you wish to cite any particular methodology along with the data, or any part of the data used in the context of a particular publication, please cite the corresponding paper. See the **Publication-wise** folder for details. If you simply wish to cite this dataset as a whole, please cite this paper:
```
@inproceedings{saha2024towards,
  title={Towards Business Process Observability},
  author={Saha, Avirup and Agarwal, Prerna and Ghosh, Sambit and Gantayat, Neelamadhav and Sindhgatta, Renuka},
  booktitle={Proceedings of the 7th Joint International Conference on Data Science \& Management of Data (11th ACM IKDD CODS and 29th COMAD)},
  pages={257--265},
  year={2024}
}
```
