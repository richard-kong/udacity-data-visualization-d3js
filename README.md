#Summary 
My visualization shows the percentage of domestic flights that were delayed for each month in 2008 split by the time of day the flight was scheduled to depart:
* morning (6am to 12pm)
* afternoon (12pm to 6pm)
* evening (6pm to midnight)
* late night (midnight to 6am)

An increasing proportion of flights are delayed as the day progresses from morning to evening, perhaps due to delays earlier in the day causing further delays later in the day. 
There were some specific periods which showed lower and higher rates if delays: September - November had the lowest percentage of delayed flights while winter months and June had the highest, this could be due to seasonal factors such as weather and peak travel seasons.

#Design

###Initial Design
A stacked bar was used to show the ratio of flights that were delayed against those that were on time. 
The total height of the bars represents the total flights and the ratio of the colors represent the the number of flights that were delayed or on time.

The data was grouped into Months and then broken up by Time of Day. The month grouping was the first level because there were 12 values which would have been too many to fit as a cluster of bars within each group. This would have made the chart very hard to read.

Month and time of day was placed on the x-axis because it is the time dimension and the number of flights was put on the y-axis because it is the measurement dimension.

###Final Design

The percent of flights delayed was used instead of a count of flights with color encoding. This simplified the chart and enabled easier comparisons across different months and/or times of day.

To improve readability:
* a filter was included where users can deselect some of the Time of Day values so that comparisons can be made for the same times across months and times of day easier.
* Changed the chart from a bar to a line chart. The bar chart had too much ink on the page and made it feel cluttered, the use of a line chart makes better use of white space and enables the reader to see trends easier.


#Feedback
Feedback was obtained from 3 people, the key points were:
* The use of a stacked bar made it hard to work out exactly how many flights were delayed in relation to on time flights. 
* The stacked bar made it hard to comparison between different groups of data.
* The user of multiple groups of bars made the chart seem cluttered and difficult to read.
* The chart was a bit busy, hard to interpret information at a glance.


#Resources
http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple`