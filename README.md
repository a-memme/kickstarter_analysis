# Kickstarting with Excel
## Overview of Project 
Performing analysis on kickstarter data, with specific interest in campaign outcomes in relation to their launch dates and funding goals.
### Purpose 
To discover and provide insight on how the financial goals and launch dates of theatre campaigns affect their success,failure, and cancel rates. 
## Analysis and Challenges 
### Analysis of Outcomes Based on Launch Date 
In order to perform analysis on theatre outcomes based on their launch dates, I isolated a number of variables from the dataset using a Pivot Table in Excel. Before this could be done, a new column of data needed to be created using the YEAR function in Excel to create data for the general year of the campaigns' respective launch dates (picture below).
![YEAR_function](macintosh hd/users/memme11/desktop/resources/YEAR_function.png)
In creating a Pivot Table, I filtered for Parent Category - specifying only theatres - and for Years. Outcomes were placed in the columns field to display all the possible outcomes to be analyzed as well as in the sum of values field in order to display the data we're interested in regarding these outcomes. The date created conversion data was placed in the rows field to show all months in the table, relative to the number of successful, failed, canceled, and grand total theatre campaigns.
![Pivot_table_theatre](macintosh hd/users/memme11/desktop/resources/Pivot_table_theatre.png)
The outcomes were then filtered to display only successful, failed, and canceled campaigns (foregoing live), and sorted in descending order.
![filtering_outcomes](macintosh hd/users/memme11/desktop/resources/filtering_outcomes.png)
From here, I was able to visualize the sorted data by inserting a line graph with markers.
![theater_outcomes_vs_launch](macintosh hd/users/memme11/desktop/resources/theater_outcomes_vs_launch.png)
### Analysis of Outcomes Based on Goals






![outcomes_based_on_launchdate](path/to/outcomes_based_on_launchdate.png)

