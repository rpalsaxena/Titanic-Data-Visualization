# Project 6: Data Visualizations of Titanic Dataset
-------
## Summary
-------
On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. Here we have a dataset of 837 people. I have done analysis as well as drawn some visualizations. My main interest is to show the survival chances of people w.r.t Sex , Age, Embarkment station, Person's Category.

In the chart, you can observe the following things.

**Chart1 : Distribution of Survival Percentage vs Categorization according to ticket fare**
  
  If a person is travelling with high price ticket i.e, VIPs then their survival rate is much higher then General & Lower Class / Employees.

**Chart2 : Distribution of Survival Percentage vs Sex Ratio**
  
  It gives an insight that Females were preferred to be saved i.e, their survival rate was high.

**Chart3 : Distribution of Survival Percentage vs Age Categorization**
  
  It gives an insight that survival of children were higher than Adults and Senior Citizens.

**Chart4 : Distribution of Survival Percentage vs Passenger Class**
  
  It shows that Upper Class(1st) were preffered over Middle Class(2nd) & Lower Class(3rd) passenger.
 
 
I have done some analysis work on Dataset. I have attached python notebook in the same repo, kindly check it for reference. Raw dataset is named with _"titanic_data.csv"_ & updated dataset after analysis is _"titanic_updated.csv"_.

---------
## Design
--------
In this data set our main motive was to understand, which attributes influenced survival rate. So, I chose BarGraph using dimplejs API which is build on top of D3js. These helped me to give an interactive look for this analysis. In my python analysis I used seaborn library for drawing graphs but still the quality and interactiveness in the graphs drawn by Dimplejs is amazing.

### Changes in design after Feedback:
 * I changed y-axis from numerical(count) scale to percentage scale i.e, changed "No. of people survived" to "Percentage of people survived".
 * Increased the Font-size of X-label and y-label
 * Changed the 3rd graph's distribution.
 
-----------
## Feedback
-----------
### Feedback-1
Hi Rahul,

Good work! I have two suggestions for your consideration:

1. Using percentage scale versus the raw scale for the y-axis could be more intuitive for the audience as that's the normal practice people anticipate. You can use percentages based on each graph, i.e. for the first graph, use percentages that are calculated based on the total of that graph for each bar combination;
2. Since the bars can clearly show the relationship, maybe it's not necessary to have the grid-lines any more, also since when you mouse over, the numbers will show anyways.
Hope this helps.

by George Liu -udacity forum

Feedback provided by George about using percentage scale is a good suggestion. I have changed the numerical scale to percentage scale. But his suggestion about grid-lines is not implemented in my final report ,since mouse over option is available on Desktop devices but on mobile device mouseover  doesn't work. So, it may give a good look for desktop users but not for mobile one

### Feedback-2
The 3rd graph/distribution - can you make the colors different than others or make that graph similar to others because in my mind after 2 graphs one represents male, one female.

by Sankalp:whatsapp group

I have changed the graph's distribution to implement the feedback given by Sankalp regarding 3rd graph's issue. 

### Feedback-3
You need to work on third graph. I took time to interpret it. The x-labels and y-labels are quite small. Can you increase its font size?

by Akshit:whatsapp group

Feedback regarding 3rd graph is implemented by changing its distribution. I have increased the size of x/y-labels.

-----------
## Resources 
-----------
* https://discussions.udacity.com/t/need-feedback-for-project-6-titanic-dataset/192680/
* https://discussions.udacity.com/t/how-to-change-no-of-survived-people-to-survival-rate-on-y-axis-titanic/192685
* https://github.com/PMSI-AlignAlytics/dimple/wiki
* https://github.com/d3/d3/wiki
* http://stackoverflow.com/questions/36171665/dimplejs-y-axis-values-in-percentages
* http://www.d3noob.org/2012/12/the-css-portion-of-d3-graph.html
