# PyBer_Analysis

---
An exploratory analysis of PyBer's ride-sharing data by writing Python script, using Panda's libraries, Jupyter notebook, and Matplotlib.

---

## Background and Results

The objective of this assignment was to produce an analysis and visualization to help PyBer improve access to ride-sharing services for all city types, whether that be Urban, Suburban, or Rural cities. The analysis and visulaization will also help PyBer determine affordability for underserved neighborhoods.

### Technical Analysis

1.Loaded the files "city_data_to_load" and "ride_data_to_load".

![Files to Load](/analysis/Files_to_load.png)

2.Read the city data file.

![Files to Read](/analysis/Files_to_read.png)

3.Merge the DataFrames.

![Merge the DataFrames](/analysis/Merge_the_DataFrames.png)

### Results

Calculated total rides for each city types, total drivers for each city types, the total fares for each city types, the average fare per ride for each city types, the average fare per driver for each city types. To create the summary DataFrame, from the merged DataFrame got the total rides, total drivers, and total fares for each city type using the groupby() function on the city type. Calculated the average fare per ride and the average fare per driver for each city type. Deleted the index name pyber_ride summary_df.index.name. Created the summary DataFrame with the appropriate columns- Total fare,Average Fare per Ride, Average Fare per Driver formatted with currency dollar and rounded to 2 decimal places.

The Total fare is shown by City Type. Rural, Subarban and Urban. The fare in Urban cities seems to be more than the rural and subarban is in the mid of the two. The trend seem to remain identical irrespective of the city. The peak of the fares happen between February and March.

![Total Fare by City Type](/analysis/Challenge_fare_summary.png)

## Challenges Encountered and Overcome

### Challenges and Difficulties Encountered

#### Programming

Some rows will contain NaNs.

#### Data analysis

Did not help in the analysis as there was no data showing up.

#### Graphing

The plotting was difficult because of NaNs. I could not draw any inference from the graph.

#### Technical Analyses Used

Created a new df and used resample by week and got sum of the fares for each week weekly_fares_df = fare_Jan_April.resample("W").sum()

## Recommendations and Next Steps

### Recommendations for Future Analysis

#### Additional analysis I

I would probably do a deep dive on Urban. Introduce some incentives such as earning reward point. That will increase the turnover in Urban areas.

Technical Steps I would add a filter to the cities and filter Urban to see the increase in the fare.

#### Additional Analysis II

I would dig deep into weekly analysis involving categories of riders. If we see the rides mainly to the downtown area during weekends or maybe at one particular time the riders are to a particular location where there is college one could start providing offers for those frequent riders, such as a rewards points program.
