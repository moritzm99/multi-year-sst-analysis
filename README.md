# Multi-year sea surface temperature data downloader, exporter and visualizer with `Copernicus Marine Toolbox`

This repository was mainly created for `Archipelagos` interns to maintain data harvesting from `Copernicus Ocean Products` for marine research purposes, it downloads/fetches, exports and visualizes `Copernicus Marine Data`.

The provided `multi_year_sst_analysis.ipynb` performs an explanatory analysis on *sea surface temperature*.

The user is encouraged to modify and contribute to further analysis on different variables available in the `Copernicus Marine Ocean Products Cataloge`.

## Requirements

Find detailed explanation on how to create the necessary set-up for this repository in the parent repository [here](https://github.com/moritzm99/hot-cold-spot-analysis-cm)

## Usage

Modify your query in the `USER INPUT` section an the beginning of `multi_year_sst_analysis.ipynb` 

```Python
# list with start and end dates organized as tuples
dates = [("2008-05-01T00:00:00", "2008-10-31T00:00:00"), 
         ("2024-05-01T00:00:00", "2024-10-31T00:00:00")]

###------------------------------------------------------###

# metadata for plotting and dataset query
dataset_id = "SST_MED_SST_L3S_NRT_OBSERVATIONS_010_012_b"

variables = ["adjusted_sea_surface_temperature"]

DOI = "https://doi.org/10.48670/moi-00171"

spatial_resolution = "0.01° × 0.01°"

temporal_resolution = "Daily"
```

## Output

### 1. Plots:
         - median plot for every date range per year
         - mean plot for every date range per year

### 2. Data:
         - GeoDataFrame saved to GPKG containing mean and median,
           for every date range per year as seperate attribute columns

## Relevant References

### Copernicus Marine Ocean Products

- access the Copernicus Marine Data Storage and find data compatible with this script [here](https://data.marine.copernicus.eu/products)
- explore quality of Copernicus Marine Data [here](https://pqd.mercator-ocean.fr/?pk_vid=161106812679b150)

### Complementary 

- read about xarray [here](https://docs.xarray.dev/en/stable/getting-started-guide/installing.html)
- watch a video about Hot-Spot Anylsis [here](https://www.youtube.com/watch?v=sjLyJW95fHM)
- learn about geospatial Python [here](https://geog-312.gishub.org)

