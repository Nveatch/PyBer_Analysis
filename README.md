# PyBer_Analysis

## Overview of Project

### Purpose
The purpose of this PyBer_Analysis was to use csv files of city and ride data to create two visualizations:
1. A PyBer summary data frame broken down for each city type
2. A line graph showing weekly total fares for each city type

These visualizations were created in order to provide recommendations for improving Pyber access and affordability. 

## Results
![PyBer Summary](https://github.com/Nveatch/Pyber_Analysis/blob/main/analysis/PyBer_summary.png)

As shown in the above dataframe, there are a few trends I noticed between the city types:

-The more developed the city type is, the more rides, drivers, and total fares it has. This is most likely due to the increase in population that follows increased development, as more people means more fares and rides, and consequently more drivers to accommodate that.

-As development decreases (from urban to rural), the average fare per ride increases. I attribute this to the fare distance most likely being longer in rural areas compared to the city, and thus costing more on average

-Also as development decreases, the average fare per driver increases. This could be a by-product of the average fare per ride being higher, or it could be that because rural areas have significantly less drivers than urban areas, and thus each driver accumulates a larger portion of the total fares.  


![Total Fares by City Type](https://github.com/Nveatch/Pyber_Analysis/blob/main/analysis/PyBer_fare_summary.png)

The line graph shows the same trend for total fares as the dataframe does: as development increases, the total fares dollars increases as well, with urban having the most while rural has the least. The graph also shows that regardless of city type, the total fares is consistent within its own city type(roughly the same over the four month period), and also somewhat proportionately with each other, with similar flat areas and a peak towards the end of february. 

## PyBer Analysis Summary
From these visualizations, my three recommendations for PyBer are as follows:
1. Increase the number of drivers for rural areas. Considering the higher average fare per ride, these trips are "probably" longer than the trips in the other city types, resulting in less available drivers at any given moment, and thus potentially underserving those areas. I would recommend increasing the drivers from the current ratio of .62 drivers : 1 ride to the ratio in suburban areas, .78 drivers : 1 ride (an addition of ~20 rural drivers).

2. Similarly, I recommend decreasing the number of drivers in urban areas. I would assume the trips are shorter for two reasons: the lower average fare, and that locations in urban areas tend to be clustered closer together. With shorter trips, more drivers should be available more often, meaning that urban areas are being potentially overserved here. While factors like traffic in urban areas might decrease the overall available driver pool, 1.48 drivers per ride seems excessive, especially compared to the other city types.

3. My third recommendation would be to perform this analysis again with another variable that was not included in the ride data csv: fare rate. I used "probably" in my first recommendation, because that recommendation is assuming that rates are uniform accross the city types, whether it be calculated by "cost per distance traveled", "cost per trip time", or some other method. I suspect this assumption is wrong though. For instance, supply and demand in rural areas leads me to believe the fare rate would be higher there due to less available drivers. Rates could be lower in urban areas due to the surplus of drivers, or they could be higher due to traffic increasing trip time. There's no way to tell definitively with the current data given, and so my prior recommendations should be re-evaluated with new visualizations that include that data column in the ride data csv.    










