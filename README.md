# PyBer_Analysis

## Overview of the Analysis

The purpose of this analysis is to investigate data from the ride-sharing app, Pyber, to present to PyBer's CEO, V. Isualize. The data includes information on city type (either urban, suburban, or rural), the cost of the ride, ride count, and driver count. The time frame for this data is from January to early May of 2019. The analysis seeks to uncover any differences in ride-sharing usage across city type, so as to make recommendations for addressing any disparities and increase revenue.

### Process and Tools

This analysis was completed using Python and the Pandas library in Jupyter Notebook, along with MatPlotLib for data visualization.

## Results

### Full Report

The full report and code can be found [here](https://github.com/ehalprin/PyBer_Analysis/blob/main/PyBer_Challenge.ipynb).

### Differences by City Type

Several differences between different city types were uncovered, including:
- Urban cities had more than twice as many total rides in the time period compared to suburban cities, and 13 times the number of rides as in rural cities.
- Urban cities had nearly five times the number of drivers compared to suburban cities, and over 30 times the number of drivers as in rural cities.
- Urban cities made twice as much in their total fares compared to suburban cities, and almost ten times as much total fares compared to rural cities.
- The average fare per ride in urban cities was $10 lower than in rural cities, and $6 lower than in suburban cities.
- The average fare per driver in urban cities was less than third of the average fare per driver in rural cities, and less than half of the average fare per driver in suburban cities.

### Differences by City Type - Summary Data Frame

![Differences_by_City_Type_Summary.png](https://github.com/ehalprin/PyBer_Analysis/blob/main/analysis/Differences_By_City_Type_Summary.png)

### Total Fare by City Type Across Time

After uncovering the initial differences in rides, drivers, and fares by city type, I used the "groupby" function to sort the fares by date. I then create a pivot table with the date as the index, and pulled out the data for January 1, 2019 through April 28, 2019. I then "resampled" this data by week to get total fares by week for each city type. This revealed that total fares for urban cities was higher than suburban and rural across the entire time period. All city types appeared to have an increase in fares toward the end of February, and again at the beginning of April. Suburban fares seemed to be increasing at the end of April, while urban and rural fares were plateauing.

### Total Fare by City Type Across Time - Graph

![PyBer_Fare_Summary.png](https://github.com/ehalprin/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

## Summary

### Overview of Disparities

Overall, it is clear that using PyBer in urban cities is easier due to a higher number of drivers, and cheaper for the consumer, but less lucrative for the driver. On the other end of the spectrum, driving for PyBer is very lucrative for the fewer number of drivers in rural cities, but it is much more expensive for consumers there and not as highly utilized.

### Recommendations for Addressing Disparities

To address the disparities among the city types, I would recommend the following:
- Advertise the higher average fare per driver in suburban and rural areas to drivers in urban areas, to incentivize them to serve those areas and increase the number of drivers there;
- Offset the cost of using PyBer in rural or suburban areas to decrease the cost to the passenger, to increase usage in those areas alongside increasing driver availability;
- Increase the cost of using PyBer in urban areas to keep revenue high there and to subsidize the decrease in cost for suburban and rural areas.
