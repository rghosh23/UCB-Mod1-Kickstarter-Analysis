# An Analysis of Kickstarter Campaigns

## Overview of Project
Kickstarter is a crowd-funding platform that uses public funding to fund individual or group creative projects. This project examines global kickstarter campaigns from 2009 to 2017 and it aims to uncover trends related to these projects.
### Purpose
The objective of this analysis is to compare various kickstarter campaign outcomes based on their launch dates and funding goals. From our analysis we will help Louise visualize various trends for theater-specific kickstarter projects so she can make better decisions for her own project.

## Analysis and Challenges
The following analysis is performed on a large dataset on Excel comprising of various kickstarter projects in multiple countries. The data provided is organized by many different sub-headings, including the description, status and goal of the campaign, amount pledged, average amount of donation, category and subcategory type, and the dates in which the campaigns began and ended. Our analysis for Louise focuses on the **theater** category, specifically on the subcategory **plays**, since Louise's campaign is for her play, *Fever*. 

### Analysis of Outcomes Based on Launch Date
Before delving into the analysis, first the table was formatted to convert the Unix launch date and end dates to conventional dates. Next the Years() function was used to extract the year from these dates. To analyze the outcomes based on launch date, a pivot table was generated. The pivot table is filtered on the Parent Category **theater**. There is an additional filter for Years so we can see any differences through the years. The columns displays the outcomes: successful, failed, or canceled. Any "live" campaigns were filtered out. The data is organized by months. The pivot table is displayed below:

<img width="350" alt="Pivot Table with Outcome Analysis" src="https://user-images.githubusercontent.com/102441140/163650739-96127d4a-603a-49b4-8548-51af9d715d7e.png">
To visualize the data from the pivot table, a line graph was generated to show the Outcomes based on the Launch Date (organized by months).

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/102441140/163649309-afbb7b28-1d78-4829-b208-b6ad7e0f3b16.png)

### Analysis of Outcomes Based on Goals
To analyze the outcomes based on the campaign goal, a table was generated. Using a COUNTIF statements, data for the the number of successful, failed and canceled projects were retrieved from the main dataset. The data retrived is also filtered to only include plays. This data is organized by various goal ranges. Next the total number of projects was calculated for each goal range. Using that information, the percentage of each outcome is calculated. Below is the tabulated data:

<img width="721" alt="Table for Outcome vs Goal" src="https://user-images.githubusercontent.com/102441140/163651007-e4d54631-1c89-4205-8685-33da56980849.png">

Using the table generated, a line graph was generated to show the Outcomes based on Goals.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/102441140/163649329-87df6010-cedf-4c7c-9710-6438b2a8fe1b.png)

### Challenges and Difficulties Encountered

The biggest challenge was trying to figure out how to organize the pivot table. However, through trial-and-error, I was able to organize the table in the proper order. We should be able to visualize the data before generating the table so that it is easier to generate the pivot table. The next roadblock was to display the months on the rows. The next challenge I faced was trying to call data from a different sheet in a workbook. A simple google search helped answer my question.

## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?

Based on the data for the Outcomes based on Launch Date, we can conclude that the most successful campaigns are launched in the summer between the  months of April - August, where the most success is found in the months of May. We can also conclude that winter months have the least succesful campaigns  since we see a drop in succesful campaigns starting in the month of October with the lowest being in December. 

- What can you conclude about the Outcomes based on Goals?

Based on the campaign goals, the most successful campaigns are below $5000. However, campaign goals between $35000-45000 have a surprisingly high success rate. Goals that went past $45000 had really low success rates.

- What are some limitations of this dataset?

The main limitation of this dataset is the fact that it is an older dataset (2009-2017). In the face of the recent pandemic, recent data from the past 5 years (2016-2021) would be a better dataset to analyze for trends. Moreover, we did not filter our dataset by the country that Louise is launching her campaign in. Trends might vary by the country of origin. 

- What are some other possible tables and/or graphs that we could create?

A pivot chart filtering the outcomes vs goals by the country of origin would be helpful to visualize what goal range would be the most sucessful in  Louise's campaign's country of origin. Similar analysis by filtering the country of origin should be done on the Outcomes based on Launch Date Analysis as well to identify any differing trends. We should also do a Box-and-Whisker plot to visualize any outliers in our dataset. 

