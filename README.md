# India Administrative Boundaries GeoJSON Files
This repository contains GeoJSON files representing the administrative boundaries of India at different levels of granularity. These files can be used for mapping and spatial analysis purposes.

## Files Description
1. #### **gadm41_IND_0.json**
   - *Description:* This file contains the border layout of India at the national level.
   - *Usage:* Suitable for visualizing the national boundary of India.
   
2. #### **gadm41_IND_1.json**
   - *Description:* This file includes the border layout of India as well as the borders of all states and union territories.
   - *Usage:* Suitable for visualizing and analyzing data at the state and union territory level.
   
3. #### **gadm41_IND_2.json**
   - *Description:* This file contains the border layout of India, the borders of all states and union territories, and the borders of all districts.
   - *Usage:* Suitable for detailed visualization and analysis at the district level.

4. #### **gadm41_IND_3.json**
   - *Description:* This file includes the border layout of India, the borders of all states and union territories, all districts, and taluks (sub-districts).
   - *Usage:* Suitable for the most granular level of spatial analysis, including taluk-level data.
   
## Usage
To use these GeoJSON files, you can load them into any GIS software or mapping library that supports the GeoJSON format. Below are some libraries in different programming languages that can be used to work with GeoJSON data.

### Python
- **GeoPandas:** For reading, writing, and manipulating geospatial data.
- **Shapely:** For geometric operations.
- **Fiona:** For reading and writing vector data.
- **Folium:** For creating interactive maps.
### JavaScript
- **Leaflet:** For interactive maps.
- **Mapbox GL JS:** For interactive maps with vector tiles.
- **Turf.js:** For advanced geospatial analysis.
- **D3.js:** For creating dynamic and interactive data visualizations.
### R
- **sf:** For simple features in R.
- **sp:** For spatial data classes and methods.
- **rgdal:** For bindings to the 'Geospatial' Data Abstraction Library.
- **leaflet:** For interactive maps.
### Java
- **GeoTools:** For Java GIS toolkit.
- **JTS Topology Suite:** For spatial operations and geometric algorithms.
### C#
- **NetTopologySuite:** For spatial operations and geometric algorithms.
- **SharpMap:** For mapping and spatial analysis.
### Visualizing GeoJSON Online
You can also visualize these GeoJSON files online using geojson.io. Simply follow these steps:

- Go to [geojson.io](https://geojson.io/)
- Click on the "Open" button on the top left corner.
- Choose "File" and then select the GeoJSON file from your local machine.
- The map will display the boundaries from the GeoJSON file.
#### Example: Loading GeoJSON with GeoPandas in Python
Here's a basic example of how to load and visualize these GeoJSON files using Python's GeoPandas library:

```python
import geopandas as gpd
import matplotlib.pyplot as plt

# Load the GeoJSON file
gdf = gpd.read_file('path/to/gadm41_IND_2.json')

# Plot the GeoDataFrame
gdf.plot()
plt.title('India District Boundaries')
plt.show()
```
#### Make sure you have the required libraries installed:

```bash
pip install geopandas matplotlib
```
## Acknowledgments
The GeoJSON files are derived from the GADM database of Global Administrative Areas.
