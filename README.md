# CASA0006 Road Context and Severity Corridors

This repository supports the submitted CASA0006 notebook:

- `CASA0006_Road_Context_Severity_Corridors.ipynb`
- `CASA0006_Road_Context_Severity_Corridors.pdf`

The notebook is the source of truth. The PDF is exported from the executed notebook for Moodle Part 2.

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
4. Export the executed notebook to a text-selectable PDF.

The notebook uses standard spatial/data-science libraries used in the coursework environment: pandas, NumPy, GeoPandas, matplotlib, scikit-learn, and OSMnx.

## Moodle Submission

Submit two parts separately:

- Part 1: the executed notebook, or a zip containing the notebook and relevant data files.
- Part 2: the PDF exported from that same notebook.

If the GitHub repository remains public and accessible, the notebook can be submitted as Part 1 without bundling the data. A backup zip can include the notebook, `framework.png`, and the required `pilot_data/` files listed above.
