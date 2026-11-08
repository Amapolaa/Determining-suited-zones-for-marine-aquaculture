# EDS223- Hw3

# Background
Marine aquaculture has the potential to play an important role in the global food supply as a more suitable protien option than lan-based meat production. Mapping the potential for marine aquaculture globally based on multiple constraints, including ship traffic, dissolved oxygen and bottom depth.

# Description
For this assignment, we are tasked with determining which Exclusive Economic Zones (EEZ) on the West Coast of the U.S. are best suited to developing marine aquaculture for several species of oysters and a species of our choice (Lobsters). Suitable locations will be determined based on range of suitable sea surface temperature (SST) and depth values for the species.

To make my workflow generalizeable, Im going to be creating a function that has the following characteristics:

- **arguments:**
    * minimum and maximum sea surface temperature
    * minimum and maximum depth
- **species name:**
    * outputs:
    * map of EEZ regions colored by amount of suitable area
        * species name should be included in the map’s title
          
## Data Details:
----
**Oysters**

Research has shown that oysters need the following conditions for optimal growth:

- sea surface temperature : 11-30 C
- depth: 0 - 70 meters below sea level

**Labstaas(Lobsters)**

 - sea surface temperature: 15 - 20 C
 - depth: 0 - 480m

**Sea Surface Temperature**

We are going to be working with was originally generated from [NOOA's 5km Daily Global Satilite Sea Surface Temperature Anomaly]. 

## Workflow Outline
---
1. The Setup - Prepare the data
2. Process the data
3. Find Suitable Locations
4. Determine the most suitable EEZ
5. Reflection

## Repository Structure
EDS223-HW3
└─── README.md
└─── qmd/Rmd/Proj files
└─── aquaculture_analysis.qmd # Name your file a title that is representative of your analysis!
|   .gitignore
    └───data
        └─── wc_regions_clean.shp
        └─── depth.tif
        └─── average_annual_sst_2008.tif
        └─── average_annual_sst_2009.tif
        └─── average_annual_sst_2010.tif
        └─── average_annual_sst_2011.tif
        └─── average_annual_sst_2012.tif
