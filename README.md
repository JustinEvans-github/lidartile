<img src="docs\montreal-panel.jpg" alt="drawing" width="800"/>

LidarTile
=========
A 3D printing project that utilizes open-source python code (LidarTile), geographic information system (GIS) software (QGIS), and 3D slicing software to make printable elevation maps.  

### General Process
1. Obtain open source DSM data through [High Resolution Digital Elevation Model (HRDEM) - CanElevation Series](https://search.open.canada.ca/openmap/957782bf-847c-4644-a757-e383c0057995) at 10m resolution or [Ontario Digital Surface Model (Imagery-Derived)](https://geohub.lio.gov.on.ca/maps/mnrf::ontario-digital-surface-model-lidar-derived/about) at 2m resolution
2. Use GIS tool (QGIS) to extract ROI
3. Run Python: [Lidartile](https://github.com/andrewgodwin/lidartile) or QGIS: [DEMto3D plugin](https://plugins.qgis.org/plugins/DEMto3D/) to generate a Stereolithography File required for 3D printing
4. 3D slicing software (Ideamaker) generates commands saved in a GCode File
5. Budget 3D printer (Kingroon K3Ps) with PLA filament

### Example
1. Source DSM data: 2016-dsm_1m_utm10_w_0_145.tif (260MB)
2. QGIS: 1.5km ROI extraction and conversion to ASC file (46MB)
3. Lidartile program conversion to Stereolithography File (.stl): bounding box of 116mm, 270k edges, and over 3.8 million triangles (180MB)
4. Slicer: IdeaMaker Project File (360MB)
5. GCode File (.gcode): 33hr runtime on 3D printer (120MB)

### Montreal, Quebec
 
- Downtown Montreal, 2018  
- 12 1/8" square, 3 x 3 tiles
- At a map scale of 1:13000, 317.7 millimeters on the map is equivalent to 4.13 kilometers on the ground.
  
<img src="docs\montreal-top.jpg" alt="drawing" width="800"/>


### Canadian Cities
City, Province |  Details: 5" square tile, 1.5km
:-------------------------:|:-------------------------:|
| Ottawa, Ontario | Halifax, Nova Scotia
| <img src="docs\ontario-ottawa.jpg" alt="drawing" width="400"/> | <img src="docs\novascotia-halifax.jpg" alt="drawing" width="400"/> |
| Calgary, Alberta | Vancouver, British Columbia
| <img src="docs\alberta-calgary.jpg" alt="drawing" width="400"/> | <img src="docs\british-columbia-vancouver.jpg" alt="drawing" width="400"/> |
| Winnepeg, Manitoba | Saskatoon, Saskatchewan
| <img src="docs\manitoba-winnepeg.jpg" alt="drawing" width="400"/> | <img src="docs\saskatchewan-saskatoon.jpg" alt="drawing" width="400"/> |
| Quebec City, Quebec | St. Johns, Newfoundland and Labrador
| <img src="docs\quebec-quebec-city.jpg" alt="drawing" width="400"/> | <img src="docs\NewfoundlandandLabrador-StJohns.jpg" alt="drawing" width="400"/> |
