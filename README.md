GIS Spatial Analysis: Wildfire Impact Area Percentages in California Counties

Project Overview
This project is part of GIS specialization from the University of California, Davis. The objective is to perform spatial data processing and vector analysis using ArcGIS Pro to calculate the percentage of land area affected by wildfires across California counties.

Tools and Skills Applied
Software: ArcGIS Pro
Core Concepts: Vector overlay, spatial measurement, data aggregation, relational table joins, data normalization, and cartographic design.
Geoprocessing Tools: Dissolve, Intersect, Calculate Geometry, Summary Statistics, Join, and Field Calculation.

Geoprocessing Workflow
Dissolve: Combined individual wildfire perimeter polygons into a single unified feature.
Intersect: Overlaid the dissolved wildfire layer with the California Counties layer to isolate overlapping spatial zones.
Calculate Geometry: Added an attribute field to compute the area of each intersection polygon in US Survey Acres.
Summary Statistics: Summarized total wildfire areas grouped by county using the COUNTY case field.
Join and Update: Joined the summary statistics table back to the County layer to populate wildfire area values, then removed the join.
Percentage Calculation: Created a new field and computed the wildfire impact percentage using the expression: (!Wildfire_Area! / !Area_Area!) * 100
Cartography and Layout: Styled the map using a 5-class Natural Breaks (Jenks) classification scheme, complete with a professional layout, scale bar, north arrow, data sources, and metadata.

Map Preview
[<img width="3300" height="2550" alt="image" src="https://github.com/user-attachments/assets/0cc3fbbd-ee27-4acf-a55a-33167d860008" />](https://github.com/sabrinazulfahn/gis-california-wildfire-analysis/blob/main/Wildfire%20Impact%20Area%20Percentages%20in%20California%20Counties.png?raw=true)

Author
Sabrina Zulfa
