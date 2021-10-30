# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this project is to analyze Kickstarter Campaign data to make recommendations to my client, Louise, for future fundraising initiatives. Louise's fundraising campaign for her play, Fever, came close to her goal in a short amount of time. For her next campaign, Louise is interested to learn if and how the launch date of a campaign affects the outcome of its fundraising goal. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
- In order to analyze fundraising campaign outcomes by launch date, I created a pivot table to organize and dynamically filter the data.  The pivot table can be viewed in the **Theater Outcomes by Launch Date tab** in the [Kickstarter Challenge Deliverables spreadsheet](/Kickstarter_Challenge_Deliverables.xlsx)
- My observations included:
  - Even though there was data between 2009 and 2017, the majority was within years 2014, 2015 and 2016.
  - The data for 2017 didn't include a full year of data, ending in mid-March 2017.
  - When looking at the data across all years versus the years 2014 through 2016, the outcomes were not significantly different. Therefore, I used all the years of data in my analysis.
  - When looking at the data across all the years: ![Theater Outcomes by Launch Date - All Years](/Theater_Outcomes_vs_Launch_All_Years.png)
     - The months of May, June and July had the highest number of total campaigns (166, 153 and 138 respectively).
     - The months of May, June and July had the highest number of successful campaigns (111, 100 and 87 respectively).
     - The months of December, January and November had the lowest number of total campaigns (71, 77, 84 respectively)
     - The months of December, January and November had the lowest number of successful campaigns (33, 44, 50 respectively)
     - The month of January had the highest number of canceled campaigns (7).
     - The months of May and June were the only two months that had more than double the amount of successful campaigns to failed campaigns. May had 111 successful campaigns to 52 failed and June had 100 successful campaigns to 49 failed. 
     - The month of December had almost as many failed campaigns as it did successful campaigns. December had 37 successful campaigns and 35 failed.


### Analysis of Outcomes Based on Goals
- In order to analyze theater/play campaign outcomes by fundraising goal
  - I created a new table of data to summarize the total number of successful, failed and canceled play campaigns for each fundraising goal. In addition, the table summarized the percentage of projects for each goal that were successful, failed and canceled. The table can be viewed in the **Outcomes Based on Goals tab** in the [Kickstarter Challenge Deliverables spreadsheet](/Kickstarter_Challenge_Deliverables.xlsx)
  - From the new table, I created a line graph to visualize the percentage of each outcome (successful, failed and canceled) for each goal: ![Play Outcomes by Goal](/Outcomes_vs_Goals_datalabels.png)  
- My observations included:
  - There were a total of 1,047 play campaigns analyzed. 
  - None of the campaigns were canceled. They either had an outcome of successful or failed. 
  - Of all of the fundraising goals, the ones that were selected the most included
    - 534 play campaigns chose the goal of $1,000 to $4,999
    - 186 play campaigns chose the goal of less than $1,000
    - 169 play campaigns chose the goal of $5,000 to $9,999
  - The fundraising goals with the highest percentage of success included
    - The goal of less than $1,000 had the highest percentage of success at seventy-six percent (76%).
    - The goal of $1,000 to $4,999 had the second highest percentage of success at seventy-three percent (73%)
    - The goals of $35,000 to $39,999 and $40,000 to $44,999 had the third highest percentage of success at sixty-seven percent (67%). However, the total number of campaigns that chose these goals were low. Only a total of 6 campaigns out of 1,047 chose the goal of $35,000 to $39,999 and only 3 campaigns out of 1,047 chose $40,000 to $44,999. 


### Challenges and Difficulties Encountered
- One of the challenges I faced when creating the 'Theater Outcomes by Launch Date' deliverable was converting the launched_at column into a user-friendly formatted date value.
  - I overcame this challenge by creating two new columns – one to hold the full converted date and one to hold only the converted year. I applied the Unix to Date conversion    formula within the first new column and then used the @Year function for the second. While I could have just created one new column, I wanted to visually see the full date for possible further analysis. 
- One of the challenges I faced when creating the 'Outcomes Based on Goals' deliverable was when I attempted to create the visual line graph.
  - When I created the line graph off of the table I created, the Y axis displayed a different data point than the one I wanted (percentages). 
  - I overcame this by right-clicking on the line graph and choosing Select Data to edit what displays on the Y axis.  

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - I can conclude that May is the best month for Louise to start a fundraising campaign in terms of highest chance of success.
  - I can conclude that December is the worst month for Louise to start a fundraising campaign in terms of highest chance of failure. 

- What can you conclude about the Outcomes based on Goals?
  - I can conclude that the two best goals for Louise to make for her fundraising campaign are either less than $1,000 or between $1,000 and $4,999. These two goals not only had the highest percentage of success, but they were the most popular selections in terms of chosen fundraising goal.
 
- What are some limitations of this dataset?
  - Not having data on how many people the fundraising campaign information was sent to
  - Not having data on the demographics of the recipients of the fundraising campaign information 
  - Not having data on what forms of communications were used to perform fundraising (email notifications, advertisements, phone calls, flyers, etc.)
  - Not having data on how often communications were sent (which days of the week, time of the day, how many times)
  - The year 2017 only had data through mid-March, not the full year

- What are some other possible tables and/or graphs that we could create?
  - A table to hold the percentage of successful, failed and canceled theater outcomes by launched date, for each month. I can then create a Stacked Column chart to visualize the percentages for each outcome in each month.
  - A table to calculate various statistics for theater outcomes by launched date, such as mean, median, standard deviation, upper quartile, lower quartile and IQR. Once I had this table, I can create a Box and Whisker chart to visualize the data outliers. I can then analyze the data again with outliers removed.
  - A table for 'Outcomes Based on Days Active', which would hold the number of days the campaigns were active (difference between deadline date and launch date) compared to their outcomes. A line graph can be created to visualize this. This would help determine which fundraising campaign lengths were most successful, versus failed and canceled.  
  - A table to hold the countries of theater campaigns compared to their outcomes.  A line graph can be created to visualize this. This would help determine which countries were most successful, versus failed and canceled for theater/play campaigns.  

