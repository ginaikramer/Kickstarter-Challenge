# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this project is to analyze Kickstarter Campaign data to make recommendations to my client, Louise, for future fundraising initiatives. Louise's fundraising campaign for her play, Fever, came close to her goal in a short amount of time. For her next campaign, Louise is interested to learn if and how the launch date of a campaign affects the outcome of its fundraising goal. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
- In order to analyze fundraising campaign outcomes by launch date, I created a pivot table to organize and dynamically filter the data.  The pivot table can be viewed in the **Theater Outcomes by Launch Date tab** in the [Kickstarter Challenge Deliverables spreadsheet](/Kickstarter_Challenge_Deliverables.xlsx)
- My obversations included:
  - Even though there was data between 2009 and 2017, the majority of the data was within years 2014, 2015 and 2016.
  - The data for 2017 didn't include a full year of data, ending in mid-March 2017.
  - When looking at the data across all of the years
     - The months of May, June and July had the highest number of total campaigns (166, 153 and 138 respectively).
     - The months of May, June and July had the highest number of successful campaigns (111, 100 and 87 respectively).
     - The months of May, June and July had the highest number of failed campaigns (52, 49 and 50 respectively).
     - The month of January had the highest number of canceled campaigns, 7.
     - Reference Theater Outcomes by Launch Date (All Years)
     
     ![Theater Outcomes by Launch Date - All Years](/Parent_Category_Outcomes_2.png)
 
  - When looking at the data only in years 2014, 2015 and 2016
     - The months of May, June and July had the highest number of total campaigns, 166, 153 and 138 respectively.
     - The months of May, June and July had the highest number of successful campaigns, 111, 100 and 87 respectively.
     - The months of May, June and July had the highest number of failed campaigns, 52, 49 and 50 respectively.
     - The month of January had the highest number of canceled campaigns, 5.
  -  There weren't a lot of theater fundraising campaigns
o	I can conclude that the two most successful months to launch a play fundraising campaign are May and June. 
	Both of these months have more than double the amount of successfully launched campaigns over failed campaigns. The month of May has a slight edge over June.
o	  I can conclude that December is the worst month to launch a play fundraising campaign. 
	Not only does December have the lowest number of successfully launched campaigns over the course of the year, there were almost as many failed launched campaigns during the month.
o	Please reference the following graph:


### Analysis of Outcomes Based on Goals
o	I can conclude that of all the fundraising goals chosen by play campaigns, the goal of $1,000 to $4,999 was chosen the most. 
	534 play campaigns chose this fundraising goal.  
o	I can conclude that the second most popular fundraising goal chosen by play campaigns was the goal of less than $1,000. 
	186 play campaigns chose this fundraising goal.
o	I can conclude that fundraising campaigns for plays with a goal of less than $1,000 had the highest percentage of successful campaigns compared with those that chose other fundraising goals. 
	Seventy-six percent (76%) of fundraising campaigns for plays with this goal were successful. Only twenty-four percent (24%) of campaigns with this goal failed. None were canceled.
	Fundraising campaigns for plays that had this goal were more than three times as likely to be successful as they were to fail or be canceled.  
o	I can conclude that fundraising campaigns for plays with a goal between $1,000 and $4,999 had the second highest percentage of successful campaigns compared with those that chose other fundraising goals.
	Seventy-three percent (73%) of play fundraising campaigns with a goal between $1,000 and $4,999 were successful. Only twenty-seven percent (27%) of campaigns with this goal failed. None were canceled.
	Play fundraising campaigns that had this goal were almost three times as likely to be successful than to fail or be canceled.  
o	I can conclude that of the fundraising campaigns for plays with goals of $35,000 to $39,999 and $40,000 to $44,999, sixty-seven percent were successful. However, only 6 total campaigns had a goal of $35,000 to $39,999 and only 3 campaigns total had a goal of $39,999 and $40,000. 
•	Therefore, I would recommend


### Challenges and Difficulties Encountered
- One of the challenges I faced when creating the 'Theater Outcomes by Launch Date' deliverable was converting the launched_at column into a user-friendly formatted date value.
  - I overcame this challenge by creating two new columns – one to hold the full converted date and one to hold only the converted year. I applied the Unix to Date conversion    formula within the first new column and then used the @Year function for the second. While I could have just created one new column, I wanted to visually see the full date for possible further analysis. 
- One of the challenges I faced when creating the 'Outcomes Based on Goals' deliverable was when I attempted to create the visual line graph.
  - When I created the line graph off of the table I created, the Y axis displayed a different data point than the one I wanted (percentages). 
  - I overcame this by right-clicking on the line graph and choosing Select Data to edit what displays on the Y axis.  

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - I can conclude that May is the best month for Louise to start a fundraising campaign in terms of highest chance of success.
  - I can conclude that December is the worst month for Louise to start a fundraising caompaigns in terms of highest chance of failure.
  - the two most successful months to launch a play fundraising campaign are May and June. 

- What can you conclude about the Outcomes based on Goals?
  - I can conclude that the two best goals for Louise to make for her fundraising campaign are either less than $1,000 or between $1,000 and $4,999. 
  -
- What are some limitations of this dataset?
  - Not having data on how many people the fundraising communication was sent to
  - Not having data on the demographics of the recipients of the fundraisign communication 
  - Not having data on what forms of communications were used to perform fundraising
  - Not having data on how often communications were sent and what time of day
  - The year 2017 only had data through mid March and not the full year.

- What are some other possible tables and/or graphs that we could create?
  - Some of the other tables/graphs that could be created to provide more information include
    - A table to calculate various statistics such as mean, median, standard deviation, upper quartile, lower quartile and IQR. Once I had this table, I can create a Box and Whisker chart to visualize the data outliers. 
      - I can then analyze the data again with outliers removed.
    - A table to hold the number of days the campaigns were active (difference between deadline date and launch date) compared to their outcomes. A line graph can be created to visualize this.
      - This would help determine which fundraising campaign lenghts were most successful, versus failed and canceled.  
    - A table to hold the countries of theater campaigns compared to their outcomes.  A line graph can be created to visualize this.
      - This would help deteremine which countries were most successful, versus failed and canceled for theater/play campaigns.  

