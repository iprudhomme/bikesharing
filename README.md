# Bikesharing
## Overview 
For our 14th data analytics project, we were given bike sharing information for August, 2019, and we were asked to present an analysis on the data to investors looking at a business proposal for a similar venture in Des Moines, IA.  We were asked to use Tableau to create a story illustrating the Citi-bike example from New York City.  

## Resources
-  Tableau Public
-  Jupyter Notebook
-  Pandas

## Results
[CitiBike NYC Story - Tableau Dashboard](https://public.tableau.com/app/profile/ilan.prudhomme/viz/CityBikeAnalysis_16486056942700/Citi-bikeNYCStory)


### Rider Information
![Rider Information](/Images/RiderInformation.png)

The First step in the story is the information of the riders.  There are 2.3M bike rides for the month of Aug. 2019  (1.5M Male, 588k Female, and 225k unknown).  The majority of the riders are subscribers and not one-off  customers (1.9M to 443k).  Most of the unknown riders are one-off riders.  By far the biggest client base is Male subscribers.

### Checkout Duration for Riders
![Rider Checkout Times](/Images/RiderCheckOutTime.png) 
The next graph shows the breakdown of ride durations broken out by hour and by minute.  Each group is an hour and the graph shows the count of rides matching each minute in that hour.  The highest would be 0h:5m with 146k rides.   

### Checkout times by Gender
![Checkout times by Gender](/Images/RiderCheckOutTimeByGender.png) 

The next graph shows the same data as the previous one, except it breaks it out by gender.  Still, the most common duration for Male and Female is 5-6mins.  The unknown seems to have a more even peak between 10 to 20 min rides.  

### Trips by Weekday by Hour
![Heatmap Trips by Weekday](/Images/TripsByWeekdayByHour.png) 
This heatmap gives us some insight into the time of day that riders are using the bikes.  Clearly the commute times are the heaviest, 7a to 9am and 5pm to 8pm both on Monday through Friday.  Also, the mid day on the weekends from 10am to 8pm Saturday and Sunday.

### Trips by Gender by Hour
![Heatmap Trips by Weekday](/Images/TripsByGender.png) 
This heatmap gives us a little deeper insight into the usage patterns.  Males are certainly the higher users for commuting, the concentration around 8am and 5-6pm is much less for Females and the unknown gender category.  There's even a noticeable lull on Wednesday evenings compared to the other week days.  

### Trips by Gender by Weekday by UserType
![Heatmap Trips by Gender by Weekday](/Images/TripsByGenderByWeekday.png) 
This further highlights the mid week lull, however it offers some further insight.  The subscribers are seem to be the ones that are commuting, especially on Thursdays and Fridays, which seems to be the most heavily used period.  

### Trips by Weekday by Hour
![Ride Count vs Duration by hour](/Images/RideCountvsDurationByHour.png) 
The last graph I created, was to show the kinds of rides being used over the course of the day, and who's taking them.  I compared the total ride count for each hour of the day, also I showed the total duration of minutes for each hour of the day.  Since the duration is directly related to the profit of the business, it's important to know if the rides are short or long.  Which time of day is most profitable.  It is clear that the evening time is by far the most profitable as it has the highest total duration. Close to 4M minutes of ride time in just the 5pm hour.  However, if you look at the middle graph, the average duration, you see it's pretty consistent across the day (except for some really long averages very early in the morning).  You can also tell that subscriber ride duration is much shorter than the one-off customer durations.  Around 14mins vs 35mins for the evening hours.  Also, you see a very high average for customers in the 2am and 4am time period.  (Perhaps there are people retrieving the bikes?). 

## Summary
From these graphs, it seems you can see there are two main types of clients.  Commuter subscribers who take more frequent shorter trips and one-off customers, possibly tourist type, who take longer trips on average.  The subscribers makes up the majority of total duration of ride time, so is the most valuable clientele.  Something to consider is the average commuter had a ride duration of around 15 mins.  For the Des Moines area, where would the commuter population live and what would the distance to work.  A further analysis might look at the number of unique bikes per day of the week per hour.  This would answer the question of how many bikes are needed, based on the area studied.  Also, the average, min, and max trips per day each unique bike takes.  This would tell us if bikes get repeat rides or not.  Finally, an analysis of unique bikes and the duration until the next ride (assuming that the bike was picked up where it was previously left off) vs rides on unique bikes that started at a different location from the previous ride.  This would indicate how many bikes were transported back to a likely more populated area.  

