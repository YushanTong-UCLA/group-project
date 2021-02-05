<h2>
  <code style="background:black;color:white">
Project Proposal (Midterm Update)  </code>
</h2>

**"Intra-Regional Migration and Transportation in New York Metro Area"**<br />
**Yushan Tong & Zhendong Long (Jayden)**<br />


## **Section 1. Project Introduction**
This project is to capture the intra-regional migration trend in the New York Metropolitan Area in relation to transportation, and its effects on the local economy, employment, and housing affordability.


## **Section 2. Why Does It Matter?**
On a personal level, we are interested in the transportation system and regional economics, and we chose this project because we want to use spatial data science to analyze the impact of the transit system on population migration patterns, and the effects of migration on the local economy, housing, and employment. In addition, both of us shared the connection with the New York Metropolitan Area since we have lived on the east coast, and would love to deepen our understanding of the urban system of the region.<br /> 

On the broader scale, the recent trend of population decline in primary cities and suburban population growth in the American Snow belt (Northeast and Midwest), and the expansive rail services in "transit desert" (where residents need to walk at least 15 minutes to the nearest rail station) led us to consider the possible relationship between the two. The rezoning of the neighboring boroughs that allowed higher density in the early 2000s filled up the land near the train tracks, while job growth, and demand for affordable housing continue to push development outwards. The recent pandemic further led outwards migration of the New York City population to nearby cities, and we hope to capture this trend using map visualization to predict future migration trends between cities and suburbs. By analyzing the trend and impact, we want to inform policymakers of the potential outcomes of population migration on the local economy, housing costs, and job markets. 


## **Section 3. Spatial Scope**
This project focuses on the geography of the New York Metropolitan Area (the “Area”). Specifically, this region refers to the “NY-NJ-CT-PA” combined statistical area (CSA) which includes four states and 31 countries. The Area is the largest metropolitan area in the U.S. and includes many largest cities in their states such as New York City, Jersey City, and New Haven. Also, the U.S. busiest commuter railways serve the Area, including MTA’s Long Island Rail Road, NJ Transit Rail, and MTA’s Metro-North. Therefore, the Area’s dynamics of population, economy, and living environments are self-evident, which will provide us a huge amount of available data for the research and analysis purpose.<br /> 

As for time span, this project will engage the data within the last 10 years because the regional developments and changes happen more frequently in the longer run. 


## **Section 4. Data Sources**
We are still following our initial plan for the data collection and processing. There are four groups of data we are currently engaging with: 
Basemap Data:<br />

### 1. Geographic borders and contexts maps:<br />

We already collected and processed the geodata of county and metro level map (shp file). We have used those files as the “geo-map” that match with our other datasets (e.g., csv files)<br />
https://catalog.data.gov/dataset/tiger-line-shapefile-2017-nation-u-s-current-county-and-equivalent-national-shapefile<br /> 

- **1.1. Transit network:** <br />
Yushan collected the transit system data in the New York Metro Area and combined them into two map layers: rail line and station. We are hoping to capture the relationship between migration trend and transit station density on the county level, so there is a need to combine the transit station layer with the county layer, and calculate station density based on geological location (“geometry”/”FIPS”).<br />
<br />
**Expected/Resulted Conclusion:**<br />
At the county level, I hope to capture the relationship between the density of transit stations and migration trend in the New York Metro Area. I expect more people to migrate from the urban core to small cities/suburban areas with higher transit station density.<br /> 
 
### 2. Demographic Data:<br />
- **2.1. Migration population data:**<br /> 
Jayden collected migration population data (both county and metro level) from Census. It’s a CSV file that contains the population number from an area to another area between 2014 to 2018. He then merged this CSV file with the geo basemaps based on FIPS codes so that the data can be spatially mapped.<br /> 
https://www.census.gov/topics/population/migration/guidance/county-to-county-migration-flows.html<br /> 
<br />
**Expected/Resulted Conclusions:**<br />
At the regional scale, which metro regions have the most and least migration population => NYC metro has the largest number of migration-out populations. So, we decided to zoom in on this region for a detailed look.<br /> 
At the regional level, which county do people in NYC migrate out. 
 
### 3. Economic Data:<br />

- **3.1 Income and local GDP data:**<br />
Jayden collected economic data at the county level from 
U.S. Bureau of Economic Analysis. This is going to be downloaded as a CSV file that contains the income and GDP data. Jayden is currently processing those data and then merging it with the geo-data<br />.  
https://apps.bea.gov/iTable/index_regional.cfm<br />
<br />
**Expected/Resulted Conclusions:**<br />
The change of income level and local GDP for each county between 2014 to 2018.
 	
### 4. Housing Data:<br />
Yushan is currently analyzing the housing affordability data on the county level based on the American Community Survey results. We analyze the housing affordability in the New York Metro Area by processing the data and mapping the results on the map by combining different dataframes.<br /> 
https://data.census.gov/cedsci/table?g=0400000US34_0500000US34037&tid=ACSDP5Y2019.DP04<br />
<br />
**Expected/Resulted Conclusion:**<br />
As housing costs decrease with distance from urban core increases, and the increasing migration trend from city center to suburban areas, and the increased commuter population, we expect to see an increased affordability as the distance from urban core increases as a result of lower housing costs and higher income.<br /> 
Based on the analysis we conducted on housing affordability so far, we observed a pattern of high housing affordability in the center of New York Metro Area (New York County). In addition, we observed the decreased affordability in the surrounding regions of New York County.<br />

## **Section 5. Methodology**

## **Section 6. Expected Insights**
Through this research project, we hope to conclude and record the intra-regional migration trend in the New York Metro Area from the perspectives of the migration direction, speed, and nature. Furthermore, by exploring the relationship between population migration and the transit network, we hope to be able to generalize the research findings to other metropolitan areas in the U.S. On the other hand, through studying the effects of migration, we hope to understand how we can respond and manage future migration and the challenges it will bring, especially in today’s pandemic context.  



An introduction of your research question
An explanation of why it is important to you, why it matters to others, and what is at stake
A description of the spatial scope (e.g. Boyle Heights or Hong Kong), and why space and/or time matters for your project
A preliminary but definitive description of data sources (at least two) that you will use
Include datasource with links
A description, accompanied by a visual flow chart that explains the methodology for the intended analysis and resulting visualizations for your project
A concluding paragraph of what insights you expect to gain from your research
