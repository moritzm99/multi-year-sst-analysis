# Multi-year sea surface temperature data downloader, exporter and visualizer with `Copernicus Marine Toolbox`

This repository downloads/fetches, exports and visualizes `Copernicus Marine Data`.

The provided `multi_year_sst_analysis.ipynb` performs an explanatory analysis on *sea surface temperature*.

The user is encouraged to modify and contribute to further analysis on different variables available in the `Copernicus Marine Ocean Products Cataloge`.

## Requirements

Find detailed explanation on how to create the necessary set-up for this repository in the parent repository [here](https://github.com/moritzm99/hot-cold-spot-analysis-cm)

## Usage

Modify your query in the `USER INPUT` section an the beginning of `multi_year_sst_analysis.ipynb` 

```Python
# List with start and end dates organized as tuples
dates = [("2008-05-01T00:00:00", "2008-10-31T00:00:00"), 
         ("2024-05-01T00:00:00", "2024-10-31T00:00:00")]

###------------------------------------------------------###

# metadata for plotting
dataset_id = "SST_MED_SST_L3S_NRT_OBSERVATIONS_010_012_b"

variables = ["adjusted_sea_surface_temperature"]

DOI = "https://doi.org/10.48670/moi-00171"

spatial_resolution = "0.01° × 0.01°"

temporal_resolution = "Daily"
```

## Output

## Relevant References
