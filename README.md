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


### Order of use

Currently it works with one image. The test can be run with the Sentinel-2 Image **S2A_MSIL2A_20170420T103021_N0204_R108_T32UNB_20170420T103454**

In order to extract images based on a buffer of 4km around a PEP725 station, these notebooks need to be excecuted in order. The input of the first file is the PEP725 file with all the observations. The third file needs the Sentinel-2 .SAFE folder as an input.
1. *PEP_725_preprocessing*
2. *PEP_725_2017*
3. *sentinel2_patch_extraction*

A few modifications will be made soon to make it run with different images as well.