# Project Update for Intro-Regional Migration and Transportation in New York Metro Area
*Jan 30, 2021*
 
Team Member:Yushan Tong, Zhendong Long (Jayden)
 
## Project Overall:
Title: Intro-Regional Migration and Transportation in New York Metro Area
Link to our proposal: http://bit.ly/39vJ6nQ 
 
## Roles:
Our primary goal in terms of collaboration is that both of us have the opportunity to do every step of the project. Therefore, we plan to divide the works by content: one person is responsible for one aspect’s data research, collection, processing, code-writing, and visualization of conclusion, while the other person is responsible for the same tasks for another content. After, we will collectively analyze the data findings horizontally.  

The contents are divided into: 
* Team Member 1 - Yushan: 
Transit network analysis
Housing affordability
* Team Member 2 – Zhendong (Jayden): 
Migration pattern analysis
Economic pattern analysis
 
## Status update: 
* Current status: 
We are getting more excited about this project as we process more dataset and visualize them in the maps. However, we are also a little bit unsure if the datasets lead to the conclusions that we are expecting. 
* Something that works: 
We are very glad to see that we are able to visualize data and present them in a way that helps us think about how to answer the research questions. 
* Something that doesn’t work yet:
Because of the complexity of our analysis on population trend on the national and regional level, we sometimes run into trouble when analyzing data with the right command. 
 
## Data update: 
	
We are still following our initial plan for the data collection and processing. There are four groups of data we are currently engaging with: 
### Basemap Data:
#### Geographic borders and contexts maps: 
We already collected and processed the geodata of county and metro level map (shp file). We have used those files as the “geo-map” that match with our other datasets (e.g., csv files)
https://catalog.data.gov/dataset/tiger-line-shapefile-2017-nation-u-s-current-county-and-equivalent-national-shapefile 
#### Transit network: 
Yushan collected the transit system data in the New York Metro Area and combined them into two map layers: rail line and station. We are hoping to capture the relationship between migration trend and transit station density on the county level, so there is a need to combine the transit station layer with the county layer, and calculate station density based on geological location (“geometry”/”FIPS”). 
* Expected/Resulted Conclusion:
At the county level, I hope to capture the relationship between the density of transit stations and migration trend in the New York Metro Area. I expect more people to migrate from the urban core to small cities/suburban areas with higher transit station density. 
 
### Demographic Data:
Migration population data: 
Jayden collected migration population data (both county and metro level) from Census. It’s a CSV file that contains the population number from an area to another area between 2014 to 2018. He then merged this CSV file with the geo basemaps based on FIPS codes so that the data can be spatially mapped. 
https://www.census.gov/topics/population/migration/guidance/county-to-county-migration-flows.html 
* Expected/Resulted Conclusions:
At the regional scale, which metro regions have the most and least migration population => NYC metro has the largest number of migration-out populations. So, we decided to zoom in on this region for a detailed look. 
At the regional level, which county do people in NYC migrate out. 
 
### Economic Data:
Income and local GDP data:
Jayden collected economic data at the county level from 
U.S. Bureau of Economic Analysis. This is going to be downloaded as a CSV file that contains the income and GDP data. Jayden is currently processing those data and then merging it with the geo-data.  
https://apps.bea.gov/iTable/index_regional.cfm 
* Expected/Resulted Conclusions:
The change of income level and local GDP for each county between 2014 to 2018.
 
	
### Housing Affordability Data
Yushan is currently analyzing the housing affordability data on the county level based on the American Community Survey results. We analyze the housing affordability in the New York Metro Area by processing the data and mapping the results on the map by combining different dataframes. 
https://data.census.gov/cedsci/table?g=0400000US34_0500000US34037&tid=ACSDP5Y2019.DP04
* Expected/Resulted Conclusion
As housing costs decrease with distance from urban core increases, and the increasing migration trend from city center to suburban areas, and the increased commuter population, we expect to see an increased affordability as the distance from urban core increases as a result of lower housing costs and higher income. 
Based on the analysis we conducted on housing affordability so far, we observed a pattern of high housing affordability in the center of New York Metro Area (New York County). In addition, we observed the decreased affordability in the surrounding regions of New York County.
 
## Concerns: 
### Major Concern: 
* Narrative of the study (tell a story why we do national and regional analysis)
* Analysis/data is good enough to draw a conclusion?
### Minor Concern: 
* Technical difficulty to find the right code to analyze the data as we would like.
* Time management
