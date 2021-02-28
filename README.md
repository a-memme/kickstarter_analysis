# Kickstarting with Excel
## Overview of Project 
Performing analysis on crowdfunding data, with specific interest in theatre campaign outcomes in relation to their launch dates and funding goals.
### Purpose 
To discover and provide insight on how the financial goals and specific launch dates of theatre campaigns affect their success,failure, and cancel rates. 
## Analysis and Challenges 
### Analysis of Outcomes Based on Launch Date 
In order to perform analysis on theatre outcomes based on their launch dates, a number of variables were isolated from the dataset using a Pivot Table in Excel. Before this could be done, a new column of data needed to be created using the YEAR function in Excel to formulate data for the year in which respective campaigns' launch dates took place. (picture below).

<img width="691" alt="YEAR_function" src="https://user-images.githubusercontent.com/79600550/109407019-a6a0db80-794b-11eb-903a-f074e78b98f6.png">

In the Pivot Table, the parent category of theatres, and years were filtered. Outcomes were placed in the columns field to display all possible outcome categorizations, as well as in the sum of values field in order to display the data of interest. The date created conversion data was placed in the rows field to show all months in the table, relative to the number of successful, failed, canceled, live, and grand total theatre campaigns.

<img width="1219" alt="Pivot_table_theatre" src="https://user-images.githubusercontent.com/79600550/109407007-8bce6700-794b-11eb-9312-23a7a462a383.png">

Outcomes were then filtered to display only successful, failed, and canceled campaigns (foregoing live), and sorted in descending order.

<img width="440" alt="filtering_outcomes" src="https://user-images.githubusercontent.com/79600550/109406972-5295f700-794b-11eb-9909-299ff5f158f4.png">

From here, the sorted data was visualized using a line graph with markers.

### Analysis of Outcomes Based on Goals
In performing analysis on outcomes based on financial goals, a number of steps were taken to isolate for the data of interest. A new table was created, depicting the financial goals of theatre campaigns into twelve categorizations (see picture below). Columns for the new table were created based on the outcome categorizatons of interest (foregoing live, as in the previous analysis), with the inclusion of total projects, and percentages for each outcome categorization. 

<img width="767" alt="outcomes_goals_table" src="https://user-images.githubusercontent.com/79600550/109437509-1c13b700-79f3-11eb-8673-5286176b7a38.png">

In order to fill the table with the correct data, the COUNTIFS function on excel was used to sort specifically for plays, the respective outcome categorization (successful, failed, or canceled), as well as the respective financial goal categorization (picture below)

<img width="788" alt="COUNTIFS function" src="https://user-images.githubusercontent.com/79600550/109437564-68f78d80-79f3-11eb-906c-455e99da3d8e.png">

Using the SUM function, the total number of projects were calculated for each financial goal categorization. Based of these totals, percentages of successful, failed, and canceled play campaigns were calculated by dividing the respective outcome categorization value with the total number of projects, and formatting the data as percentages.

<img width="789" alt="SUM_outcomes_goals" src="https://user-images.githubusercontent.com/79600550/109437606-acea9280-79f3-11eb-92b2-20d26b7b1c93.png">
<img width="853" alt="%_goals_outcomes" src="https://user-images.githubusercontent.com/79600550/109437642-de635e00-79f3-11eb-931e-33f596491dd9.png">

To visualize the data, a line graph was created based on the created financial goal categorizations, and the percentage of successful, failed, and canceled campaigns.


![outcomes_based_on_launchdate](path/to/outcomes_based_on_launchdate.png)

