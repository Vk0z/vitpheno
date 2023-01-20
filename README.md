# ViTPheno

## A Vision Transformer model for phenophase prediction

This is a work in progress and will be updated with any new changes

The project uses the Pan European Phenological Database data (PEP725) which provided by them.

### Preprocessing
The notebook *PEP_725_preprocesing* shows the preprocessing steps followed for the tabular data

The outputs are the stations and 4km buffers around them for all the relevant observations in Germany. They are in two versions.
One in WGS84/UTM zone 32N and another in WGS 84.

**WGS84/UTM zone 32N file names:**
  - PEP725_stations.geojson
  - PEP725_buffers.geojson

**WGS84/UTM zone 32N file names:**
  - PEP725_stations_WGS84.geojson
  - PEP725_buffers_WGS84.geojson



