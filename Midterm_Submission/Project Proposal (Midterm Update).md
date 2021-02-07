<h2>
  <code style="background:black;color:white">
Project Proposal (Midterm Update)  </code>
</h2>

**"Intra-Regional Migration and Transportation in New York Metro Area"**<br />
**Yushan Tong & Zhendong Long (Jayden)**<br />


## **Section 1. Project Introduction**
This project focuses on the study of internal migration (infra-region migration) and transportation (mobility) in metropolitan areas. It involves the topics of migration, demography, economy, housing, transportation, and mobility. The spatial geography this project mainly explores is New York Metropolitan Area. The project aims to answer three research questions: what is the migration pattern at both national and local scales? What are the impacts of migration on the local economy and housing? Does and how transportation infrastructure affect migration and its impacts?


## **Section 2. Why Does It Matter?**
There are three contexts that we think make those research questions matter:<br />
<br />
First, they matter in the context of our personal interests in planning. Yushan’s interest is in transportation, while Zhendong(Jayden)’s is in regional economic development. Therefore, we thought this topic a good intersection of our shared interests. We hope to use spatial data science to deepen our existing knowledge of such fields and further expand our analytical horizon in planning research and study. Also, both of us have been living on the East Coast in the past. Therefore, we are able to develop the research with our prior experiences and pieces of knowledge about the New York Metropolitan Area.<br /> 
<br />
Second, they matter in the context of the post-COVID workstyle. As we’ve been dealing with the pandemic for a year, we have to acknowledge the changes it brings to everyone. Some are temporary, but some are potentially structural, like adapting to work-from-home modes on a regular basis. Those changes are going to further lead the migration at both local and national scales. With this research project, we are trying to capture the migration pattern and observe the potential impacts. We hope to provide planning professionals with some insights on migration and design for future change in a more proactive way.<br />
<br />
Third, they matter in the context of transit-oriented development and migration. On the one hand, we see a recent trend of population decline in primary cities and suburban population growth in many US regions. On the other hand, there is an increasing interest and development in transited oriented planning models. This research project is trying to see if there is an underlying relationship between those two trends, which is able to inform planers how transportation mobility can support and direct the regional internal migration and avoid population outflows. 



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
This project is designed with five steps to expand the discussion vertically and with three categories of data develop each research step horizontally.<br />
<br />
As for the vertical development of research, those five steps range from the national scale to the local scale and from capturing the trend to analyzing the micro-relationship. The first step is to take a look at the current moving trend during the pandemic. The second step is to understand the migration trend. The third step is to zoom in on New York metro area’s regional migration pattern and its transportation network. The fourth step is to observe the economy and housing changes during the migration process. Furthermore, the last step is to analyze all individual findings and look for the relationship between migration, the impacts of migration, and transportation.<br />
<br />
As for the horizontal development of the research, our workflow generally involves three categories. First, working with SHP geodata, we want to map out the necessary geographic locations and perform spatial analysis (e.g., transportation network analysis). Second, working with various CSV census data, we clean, sort, filter, and combine datasets to look for individual findings and produce charts for them. Lastly, we combine the CSV census data with SHP geodata to spatially analyze and visualize the findings.<br />
<br />

## **Section 6. Expected Insights**
Through this research project, we hope to conclude and record the intra-regional migration trend in the New York Metro Area from the perspectives of the migration direction, speed, and nature. Furthermore, by exploring the relationship between population migration and the transit network, we hope to be able to generalize the research findings to other metropolitan areas in the U.S. On the other hand, through studying the effects of migration, we hope to understand how we can respond and manage future migration and the challenges it will bring, especially in today’s pandemic context.  


