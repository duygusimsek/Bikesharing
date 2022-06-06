# Bikesharing - NYC CitiBike 

## Overview 

The purpose analysis is to prepare a series of visualization of the successful NYC Citibike bike-sharing program, CitiBike, and use these visualizations to attract investors for a bike-sharing program in Des Moines. 

For that purpose, August 2019 CitiBike data had been used and a series of graphs were created.  For this analysis, after formatting the trip duration data type to the DateTime, visualizations for the length of time that bikes are checked out for all riders and genders,  the number of bike trips for all riders and genders for each hour of each day of the week, and the number of bike trips for each type of user and gender for each day of the week were created. 


## Result 
 
To format the data type of the trip duration from an integer to DateTime, using Python and Pandas functions, to get the time in hours, minutes, and seconds (00:00:00), the “tripduration” column was converted. [NYC_Citibike_Challenge.ipynb](https://github.com/duygusimsek/Bikesharing/blob/main/NYC_Citibike_Challenge.ipynb)

[Image of the formated data type](https://github.com/duygusimsek/Bikesharing/blob/main/images/Deliverable_1d.png)

After changing the data type, the DataFrame was exported as a CSV file to use for the visualizations. 

Using Tableau and the formatted data, visualizations that show
* How long bikes are checked out for all riders and genders?
* How many trips are taken by the hour for each day of the week, for all riders and genders?
* A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender
were created. 
 
 ### Checkout Times for Users Viz
 ![Checkout Times for Users Viz](https://github.com/duygusimsek/Bikesharing/blob/main/images/Deliverable_2a.png)

In this visualization, the graph shows the length of time that bikes are checked out for "all riders". According to the graph, most of the bikes are checked out in less than 10 minutes. 

### Checkout Times by Gender Viz

![Checkout Times by Gender Viz](https://github.com/duygusimsek/Bikesharing/blob/main/images/Deliverable_2b.png)

The graph displays the length of time that bikes are checked out for "each gender". The orange color represents the "male" users and the blue color is for "female" users. The red color is used for the "unknown" category. The count of the bikes that are used by male users, is approximately 3  times larger than the number of female users. 

### Trips by Weekday for Each Hour Viz

![Trips by Weekday for Each Hour Viz](https://github.com/duygusimsek/Bikesharing/blob/main/images/Deliverable_2c.png)

In this visualization,  the number of bike trips by weekday for each hour of the day is displayed by a  heatmap. The heatmap shows  That Thursday is the busiest day of the week.  For weekdays, 6- 9 am and 5-7 pm are the times that the CitiBike is most in use. On weekends, 10 am to 7 pm are preferred times. 

### Trips by Gender (Weekday per Hour) Viz

![Trips by Gender (Weekday per Hour) Viz](https://github.com/duygusimsek/Bikesharing/blob/main/images/Deliverable_2d.png)

This heatmap shows the number of bike trips by gender for each hour of each day of the week as a heatmap. 

### User Trips by Gender by Weekday Viz

![User Trips by Gender by Weekday Viz](https://github.com/duygusimsek/Bikesharing/blob/main/images/Deliverable_2e.png)

In this visualization,  the heatmap shows the number of bike trips broken down by gender for each day of the week by each "User type". As the heatmap displays that most of the CitiBike users are "subscribers" and they are mostly male. 

After creating these visualizations, using Tableau, a storybook was created including the "top starting and ending locations" and "the trip durations based on users' birth year" of the CitiBike and uploaded to the Tableau Public. 

[Link to Dashboard](https://public.tableau.com/shared/2696HNY2P?:display_count=n&:origin=viz_share_link)

## Summary

The result of the ‘Top Starting Locations' and 'Top Ending Locations' visualizations shows that the most active starting locations are also among the most active ending locations. That help to determine to know whether there might be an excess or shortage of bikes at particular stations over time. The “Average Trip Duration by Birth Year” graph helps to understand the pattern of usage by age. Also, the results of this analysis have given insight into the patterns of usage by time and by gender. 

When examining the weekday usage of the CitiBike, it is clear that morning and afternoon are the busiest times, while weekend usage of CitiBike is more spread throughout the day. 

 Recommendations for further analysis;

* Using the BikeID column of the data source we can identify mostly used bikes and then we can rotate them into a location that has less usage which can increase the lifetime of the bike and reduce the maintenance by avoiding repeated maintenance on the bike.

* By analyzing weekend trip durations and weekday trip durations and comparing these graphs, the patterns and purpose of usage can be found and give more insight into the CitiBike data. 

## Sources

* Data Source: From the [Citi Bike System Data page](https://ride.citibikenyc.com/system-data) the zip file [201908-citibike-tripdata.csv.zip](https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip)
* Visualization: [Tableau](https://www.tableau.com/)
* Software: [Visual Studio Code, 1.65.2](https://visualstudio.microsoft.com/downloads/)
* Library: Pandas
* Language: [Python 3.10.2](https://www.python.org/downloads)
