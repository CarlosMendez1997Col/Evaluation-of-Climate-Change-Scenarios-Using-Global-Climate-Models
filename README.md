# Evaluate climate change using ArcGIS API for Python and ArcGIS Maps SDK for JavaScript

## Use and install this repository

HTTPS
```CSS
https://github.com/CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript.git
```

GitHub CLI
```CSS
gh repo clone CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript
```

## Description

Repository built in `Arcgis for Python` and `ArcGIS Maps SDK for JavaScript`.

Each chapter is described below:

1. The first chapter, geoprocessing `NetCDF` files and convert them to `CRF` (Cloud Raster Format).
```HTML
https://github.com/CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript/tree/main/1.%20Geoprocessing%20NetCDF%20data
``` 
2. The second chapter, analyze trends/patterns and calculate `Multidimensional Anomaly`, `Trend Raster` and `Predict Using Trend Raster`.
```HTML
https://github.com/CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript/tree/main/2.%20Analysis%20of%20trends%20and%20patterns%20using%20multidimensional%20data
```
3. The third chapter, shows some animations and timelines of `19 Bioclimate Projections of WorldClim` using `ArcGIS Maps SDK for JavaScript`. 
```HTML
https://github.com/CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript/tree/main/3.%20Animations%20and%20timeline%20of%20climate%20projections
```
4. The fourth chapter, share the links of original NetCDF files.
```HTML
https://github.com/CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript/tree/main/4.%20Data%20and%20files
```

## Prerequisites and libraries

### ArcGIS API for Python

```python
import arcpy
import datetime as dt
import os
import arcgis
import NetCDF4
import csv

# Arcpy
from arcpy.ia import*

# arcgis
from arcgis.gis import GIS
from arcgis.raster import *
from arcgis.raster.functions import *
from arcgis.raster.analytics import *

```
### ArcGIS Maps SDK for JavaScript

```html
<script>
    require([
      "esri/Map",
      "esri/views/MapView",
      "esri/layers/ImageryTileLayer",
      "esri/layers/support/DimensionalDefinition",
      "esri/layers/support/MultidimensionalSubset",    
      "esri/widgets/Slider",
      "esri/widgets/TimeSlider",
      "esri/widgets/Legend",
      "esri/request",
      "esri/Color",
      "esri/widgets/LayerList",
      "esri/widgets/Expand",
      "esri/layers/TileLayer",
      "esri/layers/BaseTileLayer", 
       "esri/Basemap",
       ], 
            (Map, MapView, ImageryTileLayer, DimensionalDefinition, MultidimensionalSubset,
            Slider,TimeSlider, Legend, esriRequest, Color,LayerList, Expand, TileLayer, BaseTileLayer,Basemap) =>  
<script>
```
## Versions and releases

Version `1.0`

```HTML
https://github.com/CarlosMendez1997Col/Evaluate-climate-change-using-ArcGIS-API-for-Python-and-ArcGIS-Maps-SDK-for-JavaScript/releases
```

## Data acquisition and download

The data used in this program come from the Coordinated Regional Downscaling Experiment (CORDEX) [Website](https://esgf-node.ipsl.upmc.fr/projects/esgf-ipsl/) and the World Climate Research Program (WCRP), using the CCCma-CanESM2, MOHC-HadGEM2-ES and MIROC-MIROC5 models.


| Item                    | Precipitation 2021-2030 SAM                                 | Near Surface Air Temperature 2021-2030 SAM                  |
|-------------------------|-------------------------------------------------------------|-------------------------------------------------------------|
| Project                 | CORDEX                                                      | CORDEX                                                      |
| Product                 | output                                                      | output                                                      |
| Domain                  | SAM-20                                                      | SAM-20                                                      |
| Institute               | INPE                                                        | INPE                                                        |
| Driving Model           | CCCma-CanESM2 (1), MIROC-MIROC5 (1) and MOHC-HadGEM2-ES (1) | CCCma-CanESM2 (1), MIROC-MIROC5 (1) and MOHC-HadGEM2-ES (1) |
| Experiment              | rcp45                                                       | rcp45                                                       |
| Experiment Family       | RCP                                                         | RCP                                                         |
| Ensemble                | r1i1p1                                                      | r1i1p1                                                      |
| RCM Model               | Eta                                                         | Eta                                                         |
| Downscaling Realisation | v1                                                          | v1                                                          |
| Bias Adjustment         | None                                                        | None                                                        |
| Time Frequency          | mon                                                         | mon                                                         |
| Variable                | pr                                                          | tas                                                         |
| Variable Long Name      | Precipitation                                               | Near-Surface Air Temperature                                |
| CF Satandard Name       | precipitation flux                                          | air temperature                                             |
| Datanode                | esg-dn1.nsc.liu.se                                          | esg-dn1.nsc.liu.se                                          |

CCMa-CanESM2 Model
[Model CCCma-CanESM2 information](https://climate-modelling.canada.ca/climatemodeldata/cgcm4/CanESM2/index.shtml)

MOHC-HadGEM2-ES Model
[Model MOHC-HadGEM2-ES information](https://www.metoffice.gov.uk/research/approach/modelling-systems/unified-model/climate-models/hadgem2)

MIROC-MIROC5 Model 
[Model MIROC-MIROC5 information](https://catalogue.ceda.ac.uk/uuid/d90ca0077e3344c7840ca56e49f89ee7/?jump=related-docs-anchor)

## Credits and more information

* [The Intergovernmental Panel on Climate Change](https://www.ipcc.ch/)

* [World Climate Research Programme (WCRP)](https://www.wcrp-climate.org/)

* [The Coordinated Regional Downscaling Experiment (CORDEX)](https://cordex.org/)

* [The Earth System Grid Federation (ESGF)](https://esgf.llnl.gov/)

## Conflict of Interest.

The author declare that there is no conflict of interest in the publication of this data and have approved it for publication.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate. 

## MIT License

Copyright (c) 2025 Carlos Mendez

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
