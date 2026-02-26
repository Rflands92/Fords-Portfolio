Wildfire Analysis 

---

About This Portfolio

This repository contains GIS projects completed as part of my ArcGIS Enterprise and Server coursework. Projects focus on spatial analysis, Python scripting with the ArcGIS API, and real-world environmental data. I chose to create this project with a Colorado Wildfire in mind versus the course works suggestion. 

---

Repository Contents

| File | Description |
|---|---|
| `Final Project Notebook.pdf` | Jupyter/ArcGIS Pro notebook analyzing the East Troublesome Fire (2020) — includes spatial intersection, National Forest acreage calculation, burn severity analysis, and ArcGIS Online map publishing |
| `Capastone Final.pdf` | 
Description of 3 Public GIS web applications that ste local to Colorado. 

---

Project: East Troublesome Fire (2020) — National Forest Burn Analysis

Overview
The East Troublesome Fire ignited on October 14, 2020 in Grand County, Colorado and became the **second-largest wildfire in Colorado recorded history**, burning over 193,000 acres. This project uses Python and ArcGIS Pro to answer:

- What was the total acreage burned?
- How much of that area fell within National Forest boundaries?
- How did burn severity break down across affected forest land?

Tools & Technologies
- **ArcGIS Pro** — Project workspace, geoprocessing, spatial analysis
- **arcpy** — Spatial intersection, geometry calculations, feature class management
- **ArcGIS API for Python** — ArcGIS Online authentication, hosted feature layer publishing, Web Map creation
- **Pandas** — Tabular data analysis and summary statistics
- **Matplotlib** — Data visualization and charting
- **Git / GitHub** — Version control and portfolio publishing

Data Sources
| Dataset | Source |
|---|---|
| Fire Perimeter & Burn Severity (dNBR) | [MTBS — Monitoring Trends in Burn Severity](https://www.mtbs.gov/direct-download) |
| National Forest Boundaries | [USFS Enterprise Data Warehouse](https://data.fs.usda.gov/geodata/edw/datasets.php) |
| Basemap Imagery | Esri Living Atlas (ArcGIS Online) |
| Historic Fire Perimeters | [NIFC Open Data Portal](https://data-nifc.opendata.arcgis.com) |

Methodology
1. Loaded MTBS fire perimeter shapefile and USFS National Forest boundaries
2. Reprojected all data to **NAD 1983 UTM Zone 13N** (EPSG:26913) for accurate area calculations in Colorado
3. Performed spatial **intersection** of fire perimeter × National Forest boundary
4. Calculated **acreage** within and outside National Forest land
5. Overlaid MTBS **dNBR burn severity raster** and tabulated area by severity class
6. Visualized results with charts and an **interactive ArcGIS Online Web Map**
7. Published hosted feature layers to ArcGIS Online portal

---

Study Area

**Grand County, Colorado** — The East Troublesome Fire burned primarily through the **Arapaho & Roosevelt National Forest** and threatened the communities of Grand Lake and Granby before containment.

---

How to Run the Notebook

1. Open **ArcGIS Pro** and launch the notebook from the Catalog pane
2. Update `PROJECT_FOLDER` in Section 1 to your local working directory
3. Download MTBS data from https://www.mtbs.gov/direct-download (Event ID: `CO4023510601020201021`)
4. Ensure **Spatial Analyst** extension is licensed in ArcGIS Pro
5. Run cells sequentially from top to bottom. 

---

References

- MTBS Program: https://www.mtbs.gov
- USFS EDW Open Data: https://data.fs.usda.gov/geodata/edw/datasets.php
- NIFC Historic Perimeters: https://data-nifc.opendata.arcgis.com
- Esri ArcGIS API for Python Documentation: https://developers.arcgis.com/python/
- Colorado State Forest Service: https://csfs.colostate.edu/gis-data/

---

Contact

**GitHub:** [Rflands92](https://github.com/Rflands92)  *

---
*This portfolio was created for educational purposes for BootcampGIS.
