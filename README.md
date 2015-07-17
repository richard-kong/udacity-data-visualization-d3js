#Summary 
My visualisation shows the percentage of domestics flights that were delayed in each month in 2008. There was a very noticeable lower percentage of delayed flights between September and November, these months also had the lowest number of flights. June and December had the highest percentage of delayed flights.

#Design

###Initial Design
A stacked bar was used to show the ratio of flights that were delayed against those that were on time. 
The total height of the bars represents the total flights and the ratio of the colors represent the the number of flights that were delayed or on time.

The data was grouped into Months and then broken up by Time of Day. The month grouping was the first level because there were 12 values which would have been too many to fit as a cluster of bars within each group. This would have made the chart very hard to read.

Month and time of day was placed on the x-axis because it is the time dimension and the number of flights was put on the y-axis because it is the measurement dimension.

A stacked bar was the best way to show trends in flight numbers at different times of the day across different months of the year. I am able to show trends for both the total number of flights for each part of the day as well as the ratio of on time and delayed flights.

Other chart types that were considered:
* Pie chart: Although these look pretty, they are not the best at communicating data. The human eye is not very good at perceiving proportions in a circular object. It would also have been difficult to show trends in the percentage of delayed flights over months or during various parts of the day. To present the same information, we would need to have a total of 48 pie charts (4 for each month). Alternatively, I could have presented 1 pie chart per month which only recorded the delayed flights and split them into different parts of the day. This would have been misleading since I saw in the bar chart the number of flights is much greater in some parts of the day.
* Line chart: Time of day with delayed/on time as line series. This would result in 8 lines which is too many for a single chart. I could have split this line chart into 2 charts with 1 showing the delayed flights and the other showing the on time flights. Having the the data split out would make it difficult to look at the total flights for each part of the day. 
  

###Final Design

The final visualisation was a bubble chart with the percentage of flights delayed on the y axis, months on the x, flight number on the z. The z axis was encoded into the size of the bubbles. The use of a percentage removed the need to split the data into 2 series, therefore, making it easier to see trends across time. As per the feedback, I removed the time of day variable from the chart since the number of flights vary throughout the day and having this in the chart may have lead to some false conclusions.
 
Other chart types methods I considered were:
* Line chart with different size points: I could not get a good balance for the size of the points to make differences visible whilst keeping the line in the chart visible. 
* Add a bar chart with another axis for the flight count: Including another axis is confusing and the flight count encoding is quite seperated from the trend of delayed flight percentage so it is hard to relate the two together.

A bubble chart was a good choice because it kept the chart simple and easy to interpret. Flight counts, and the trend of delayed flights across the months were all encoded into the size and placement of the bubbles making it easy to interpret the data together. 

The largest change in flight numbers between months was about 12%, this was hardly visible when looking at the the size differences of the bubbles. I choose to modify the z scale to reduce the size of bubbles to reduce overlapping and also to show the reduction in flights more prominently. I was conscious that changing the scale would exaggerate small differences in flight numbers, so, I experimented with a few different settings to minimise the effect.   

I also did some additional data exploration into the flight data to see if there were any clues on why the September to October period had such low flight delay percentages.
There were 5 fields in the data which could have explained this:
* CarrierDelay
* WeatherDelay
* NASDelay
* SecurityDelay
* LateAircraftDelay

Unfortunately, I could not use these fields to enrich my visualisation. The data in these fields were not complete or there were other reasons for delays that were not captured. I found that of fights that were delayed, over 50% of them had a value of "NA" for all of the fields listed above.

Based on the data I have, I am unable to provide any strong evidence to support any conclusions. It looks like that the lower percent of delayed flights was due to an overall number of flights in the September - November period, this is probably not the only factor in play. If you look at December there are a similiar number of flights but the rate of delay is almost the highest of any month. 

I would like to investigate the number of passengers, the ratio of aircraft fleet size to daily flights operated to see if there is any corelation with delayed flights. The global financial crisis started around September 2008, with the US entering a recession both business and recreational air travel would have been reduced significantly, so there would have been less passengers on each flight. The airlines may have reduced their flights as a result of reduced demand. Although flights were reduced, the airlines still had the same levels of staff and aircraft available to them which meant they had more resources to service the operating flights. There was a surge in delayed flights in December, this could have been, due to the increase in the number of passegners due to the Thanksgiving holidays.

#Feedback

###Feedback 1:
I don't actually see any trends that jump out at me in the stacked bar chart. I only see a couple of trends:
* Modest reduction in the total number of flights at the end of the year
* Most flights are in the morning and afternoon

I cannot get any useful information out of the chart. It would be more interesting to see if there is a trend in delayed flights throughout the year, perhaps displayed as a percentage of delayed flights by month and time of day.

###Feedback 2:
Questions and Relationships
* What is the overall percentage of delayed flights per month?
* Why are the the percentage of delayed flights highest in the afternoon and evening?
* Why is there a lower percentage of delayed flights in the August - November period?
* What happened in June and December? there appear to be spikes in delayed flights.

The main takeaway is that there are lower rates of delay in the morning than the afternoon and evening, and, September to November is the time of the year to travel if you want the lowest chance of having a flight delayed.

###Feedback 3
It would be nice to somehow compare the trends of a specific part of the day across all months

###Feedback 4 (Udacity Review)
Analysing the flight delays across different times of the day could be misleading due to a disprotional number of flights at different times of the day. I would also need to somehow bring the flight count into the visualisation to show a more complete picture.
The first versions illustrated an interesting trend where between September and November exhibited a much lower percentage of delayed flights than other months, it would be very interested to present more data to show why this might have been.

#Resources
http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple`