# DEM Clipper Tool
Developed by Declan Knies with help from Sam Johnstone and the USGS's [dem_getter](https://code.usgs.gov/gecsc/dem_getter/-/tree/1.0.0).

## Introduction

This tool uses the USGS' webmap and internal map APIs to generate a DEM based off of an input shapefile.

## Setup

1. Within your workspace, extract the DEMClipper Zip to a folder labelled DemClipper

2. Add the atbx (arctoolbox) to the contents panel in ArcPro

3. Choose an input shapefile and an output folder

## Using the Toolbox

Open the *DEMClipper* atbx. You now have several options to select the source and resolution

### Input Shapefile

In this box, select your input shapefile

### DEM Output Folder

In this box, select the folder where your new DEM should end up

### Vertical Unit in Feet

This box determines whether the program should convert your final DEM's vertical scale to feet

### Output Name

This box allows you to customize the name of your output DEM, remember to change this for different outputs to avoid confusion

### Service

The box determines which USGS service the tool should use to acquire the DEMs, it also determines which boxes below are necessary

### 3DEP Options

**3DEP Sample Resolution** determines the resolution of the DEM tiles acquired, 3m recommended

**3DEP Polygon Buffer** determines the buffer on the edge of downloaded tiles, 300m recommended

**3DEP Tile Dimensions** determines the geographic size of the tiles to be downloaded, 1500m is recommended

### USGS Direct Options

**USGS Direct Source** determines the resolution (i.e. 1 meter, 3 meter, 1/9 arcsecond) of the DEM to be downloaded, 1m recommended

**USGS Direct Spacial Reference** determines the spacial reference of the tiles to be downloaded, NAD_1983_UTM_Zone_13N recommended

## Troubleshooting

For any issues email Declan Knies at dknies@mines.edu

## Credit

DEMClipper ArcToolbox developed by Declan Knies at the Colorado Geological Survey

Credit for the USGS dem_getter modules goes to Sam Johnstone at the USGS and you can get the latest version here: https://code.usgs.gov/gecsc/dem_getter
