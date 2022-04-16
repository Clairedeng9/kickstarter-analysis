# Kickstarting Dataset Analysis by using Excel
## Overview of Project
Kickstarter is a public benefit crowdfunding platform which will help people gain supports from any individuals or organizations to achieve a new idea or project and bring these projects to our vivid life.
### Purpose
The purpose of this project is to provide the public information to anyone who might be a project creator or money funder to develop more ideas on how different outcomes or fundraising goals effect by different categories, subcategories, data created conversion etc. from year 2009 to 2017.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In analysis 1, we measured that how the launch date by month related with the number of successful, failed, or canceled outcomes only in theater campaign from year 2009 to 2017. In order to visualize the data, the pivot chart was built in months in x-axis and counts of outcomes in y-axis, by setting to see the result only among successful, failed and canceled outcomes, then can be filtered by removing the outcomes of live campaigns, grouped dates to only show the months of the year and filtered the parent category to show data for “theater” only. To visualize the data from the pivot chart below, a line chart with markers was created to show the relationship between theater campaign outcomes based on their launch month
.![image](https://user-images.githubusercontent.com/103073631/163684803-45115a77-cb0b-484c-8d46-56df885c8a3c.png)

### Analysis of Outcomes Based on Goals
The analysis 2 is to analyze the percentage of successful, failed, and canceled plays based on the funding goal amount. First of all, in order to build up the table of the percentage of successful, failed, and canceled plays based on the funding goal amount, we set up the goal amounts into 12 different ranges from less 1000 to more than 50,000. Then the ```COUNTIFS()``` function applied to populate the numbers of successful, failed and canceled by filtering on the Kickstarter "outcome" column, on the "goal" amount column, and on the "Subcategory" column using "plays" as the criteria. Next, the total number of each outcome was calculated and generated the percent of outcomes. The pivot chart below was built on percentages of outcomes based on goal ranges and filtered by Plays, x-axis shows goals ranges in dollar amount, and y-axis is the percentages of outcomes.  
![image](https://user-images.githubusercontent.com/103073631/163685362-41312f0f-7c8b-4279-9bbd-41ca474288f8.png)

### Challenges and Difficulties Encountered
During the process of the first analysis, per requesting, the ![image](https://user-images.githubusercontent.com/103073631/163683879-3338747e-28d8-416d-8190-1a868249a1b4.png) should be grouped by month only in pivot table field. It is quite challenging to me at the beginning, the dates in field have the format as "mm/dd/year" without seeing the hints, I tried to use a excel function ```MONTH()``` to extract month column from dataset ![image](https://user-images.githubusercontent.com/103073631/163683879-3338747e-28d8-416d-8190-1a868249a1b4.png) column, when putting month into pivot table rows, the presentations of month were not three abbreviated characters. Until I followed with hints provided me the method on how to group the data in pivot table. the presentations were matched with requirements.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - By analyzing the pivot table, the maximum count of successful is 111 in May, similarly, the maximum count of failed is 52 which also in May, and the maximum of canceled is 7 located in January. These can be concluded that if you want a higher success rate to launch a theater campaign the better choice is in May, then followed by June, but at the same time, you also face a higher rate of fail. There are two declined trends after May to Sept and Oct to Dec, but another peak with relative higher success and failed rate after May is in Oct with 0 canceled outcome.

- What can you conclude about the Outcomes based on Goals?
  - By visualizing the pivot chart, there are two lines the percentage of successful and the percentage of failed are interacted three times, which means in certain ranges the percentage of successful is higher than fail and over that range will be changed to another situation. If the goals amount less than 19,999 and in between 35,000 and 44,999 the percentage of successful is always higher than the percentage of failed. In addition, a funding goal range of less than a $1,000 up to $4,999 has a success rate ranging from 73% to the highest 76%. The goal range in 45,000 to 49,999, it shows 100% failed with 0% successful and 0% canceled.
 
- What are some limitations of this dataset?
  - The limitation of this dataset was only provided the year 2009 to 2017 and all date information came from this one crowdfunding platform. In our second analysis, the percentage of canceled plays were 0, it could be a reason that the sample size was small and timeline range was not long enough.

- What are some other possible tables and/or graphs that we could create?
  - To better observe the trend between successful and failed count of outcomes, a line trend graph was needed to present the successful status counts vs failed status counts from April 2009 to Dec 2019. A pie chart was also needed to have a brief idea to see the percentage of parent categories among campaigns.
