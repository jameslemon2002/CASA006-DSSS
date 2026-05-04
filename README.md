# CASA0006 Road Context and Severity Corridors

This repository supports the CASA0006 notebook:

- `CASA0006_Road_Context_Severity_Corridors.ipynb`

The notebook is the source of truth for the analysis.

## Required Data Files

The notebook first checks for local files in `pilot_data/`. If a file is missing, it reads the same file from `https://github.com/jameslemon2002/CASA006-DSSS` using raw URLs.

Required files:

- `framework.png`
- `pilot_data/road_collision_2024.csv`
- `pilot_data/road_casualty_2024.csv`
- `pilot_data/road_vehicle_2024.csv`
- `pilot_data/London_Boroughs.gpkg`
- `pilot_data/traffic-flow-borough.xlsx`
- `pilot_data/osm_london_drive_edges.gpkg`
- `pilot_data/london_lsoa_2011_boundaries.geojson`
- `pilot_data/london_lsoa_imd2019.xlsx`

No required file exceeds GitHub's 100 MB single-file limit. The largest required file is the cached OSM road-link GeoPackage, which is included so the notebook does not need to rebuild the road network from OSM on a fresh run.

## Running

1. Open `CASA0006_Road_Context_Severity_Corridors.ipynb`.
2. Restart the kernel.
3. Run all cells.
The notebook uses standard spatial/data-science libraries used in the coursework environment: pandas, NumPy, GeoPandas, matplotlib, scikit-learn, and OSMnx.
