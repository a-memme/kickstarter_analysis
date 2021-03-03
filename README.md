# Kickstarting with Excel
## Overview of Project 
Performing analysis on crowdfunding data, with specific interest in theatre and/or play campaign outcomes in relation to their launch dates and funding goals.
### Purpose 
To discover and provide insight on how the financial goals of play campaigns and launch dates of theatre campaigns affect their success,failure, and cancel rates. 
## Analysis and Challenges 
### Analysis of Outcomes Based on Launch Date 
In order to perform analysis on theatre outcomes based on their launch dates, a number of variables were isolated from the dataset using a Pivot Table in Excel. Before this could be done, a new column of data needed to be created using the YEAR function in Excel to formulate data for the year in which respective campaigns' launch dates took place. (picture below).

<img width="691" alt="YEAR_function" src="https://user-images.githubusercontent.com/79600550/109407019-a6a0db80-794b-11eb-903a-f074e78b98f6.png">

In the Pivot Table, the parent category of theatres and years were filtered. Outcomes were placed in the columns field to display all possible outcome categorizations, as well as in the sum of values field in order to display the data of interest. The date created conversion data was placed in the rows field to show all months in the table, relative to the number of successful, failed, canceled, live, and grand total theatre campaigns.

<img width="1219" alt="Pivot_table_theatre" src="https://user-images.githubusercontent.com/79600550/109407007-8bce6700-794b-11eb-9312-23a7a462a383.png">

Outcomes were then filtered to display only successful, failed, and canceled campaigns (foregoing live), and sorted in descending order.

<img width="440" alt="filtering_outcomes" src="https://user-images.githubusercontent.com/79600550/109406972-5295f700-794b-11eb-9909-299ff5f158f4.png">

From here, the sorted data was visualized using a line graph with markers (see Resources folder).

### Analysis of Outcomes Based on Goals
In performing analysis on outcomes based on financial goals, a number of steps were taken to isolate for the data of interest. A new table was created, depicting the financial goals of theatre campaigns into twelve categorizations (see picture below). Columns for the new table were created based on the outcome categorizatons of interest (foregoing live as in the previous analysis), with the inclusion of total projects and percentages for each outcome categorization. 

<img width="767" alt="outcomes_goals_table" src="https://user-images.githubusercontent.com/79600550/109437509-1c13b700-79f3-11eb-8673-5286176b7a38.png">

In order to fill the table with the correct data, the COUNTIFS function on excel was used to sort specifically for plays, the respective outcome categorization (successful, failed, or canceled), as well as the respective financial goal categorization (pictured below).

<img width="788" alt="COUNTIFS function" src="https://user-images.githubusercontent.com/79600550/109437564-68f78d80-79f3-11eb-906c-455e99da3d8e.png">

Using the SUM function, the total number of projects were calculated for each financial goal categorization. Based of these totals, percentages of successful, failed, and canceled play campaigns were calculated by dividing the respective outcome value by the total number of projects. The data was then formatted as percentages. 

<img width="789" alt="SUM_outcomes_goals" src="https://user-images.githubusercontent.com/79600550/109437606-acea9280-79f3-11eb-92b2-20d26b7b1c93.png">
<img width="853" alt="%_goals_outcomes" src="https://user-images.githubusercontent.com/79600550/109437642-de635e00-79f3-11eb-931e-33f596491dd9.png">

To visualize the data, a line graph was created based on the curated financial goal categorizations and the percentage of successful, failed, and canceled campaigns (see Resources folder).
### Challenges and Difficulties Encountered
In sorting and analysing data to depict theatre outcomes vs launch date, steps were fairly straightforward and simple with use of the Pivot Table feature in Excel, and didn't provide many challenges. A difficulty one may have encountered during this analysis could be overcoming a number of extra categorization elements when adding the date created conversion option to the rows field: here, two extra categorizations are automatically added to the field of question, sorting the data in years and quarters in addition to the month created (see picture below). To overcome this, one would simply need to remove these extra categorizations to display the data solely in reference to months.

<img width="1090" alt="removing_categorizations" src="https://user-images.githubusercontent.com/79600550/109835822-93bf2d00-7c11-11eb-9e6c-cfc869425d0a.png">

Performing analysis on outcomes based on goals, however, presented a couple of challenges through a longer series of steps. 
The first challenge was the small executional error of using the COUNTIF function rather than COUNTIFS - without the plural form of the function, Excel will not allow more than one argument and thus, one cannot sort for multiple factors when applying the filter. This led to the second error of sorting data through filters on the original Kickstarter Data sheet (sorting for the subcategory "plays" and sorting outcomes into decending order so specific cells could be referenced - see picture below). The COUNTIF function was then used to only filter for the financial goal categorizations, referencing the respective cells from the Kickstarter data sheet that had been previously sorted. 

<img width="686" alt="sorting_plays" src="https://user-images.githubusercontent.com/79600550/109438723-29cc3b00-79f9-11eb-8916-b5d31012a17d.png">

<img width="850" alt="descending_outcomes" src="https://user-images.githubusercontent.com/79600550/109438767-4b2d2700-79f9-11eb-8570-837b8fefedf2.png">

<img width="786" alt="COUNTIF_notIFS" src="https://user-images.githubusercontent.com/79600550/109438776-5718e900-79f9-11eb-8f7c-79dbb47ddebb.png">

Although seemingly an alternative way to sort the same data, this process yielded incorrect results. The series of challenges created here through one small oversight of execution was overcome simply by going back to the Module material, exploring the "show hint" resources, and catching the error in functional execution.
## Results 
### Conclusions 
From the data analysed regarding theatre outcomes and their respective launch dates, a number of conclusions can be made. First, there are a greater number of successful theatre campaigns across all months of the year in comparison to failed and canceled, indicating that theatre campaigns are generally successful. 
Second, there is an increase in both successful and failed theatre campaigns approaching the spring months - peaking in May - and tapering off through the rest of the summer. This trend perhaps could be impacted by the fact that most theatre campaigns are launched during these months. However, as the trend is much more exaggerated in successful campaigns than in failed ones, there is indication that launching theatre campaigns through the months of roughly April-August - but more specifically in May - lends to an overall greater rate of success. 
In regard to canceled campaigns, the greatest number occur in January, but remain generally stagnant through the rest of the year, with zero cancellations in October. 
Finally, one can observe a spike in both successful and failed campaigns in October, but, with a larger increase in failed campaigns vs successful ones, there is suggestion that the month of October may be a less reliable month to launch a theatre campaign. With the data displaying the lowest number of successful campaigns in December as well as the highest number of cancellations in the following month of January, one could also note that these specific winter months may be the least desirable when planning to launch a respective crowdfunding campaign.

Data sorted and analysed for play outcomes based on their financial goals also yielded some interesting results. 
As the percentage of canceled play campaign projects was zero across all categories, the percentage of successful and failed campaigns naturally form an inverse relationship in regard to their financial goals. The predominate find here is that the highest percentage of successful campaigns occur at the lowest range of financial goals, while the highest percentage of failed campaigns occur at the highest range of financial goals. With this, there is indication that a more modest fundraising goal is likely to yield a greater rate of success. It is worth noting, however, that as the financial goal ranges increase, the percentage of successful campaigns decrease, until reaching the range of $25000-$29999, to where the success rate increases and then decreases drastically again. The percentage of failed campaigns displays the inverse of this relationship. This would be an interesting area to conduct further investigation on to determine why the trend breaks in this specific goal range, and whether the second half of the data pertaining to these ranges (i.e > $30 000) is as representative as the first half, noting that there is a comparatively lower number of total projects for these goal ranges. 
### Limitations 
There are a number of limitations to note when considering this dataset and its relevance to the topic of interest. First, although the data at hand has been collected from the past 10 years, the most recent year in which it was collected was 2017, which amounts to a relatively small dataset in comparison to other stand-alone years. A more recently updated and representative dataset could provide for more accurate information, and perhaps reveal any changes in trends within the recent years that may be of greater relevance and interest to Louise's particular situation.
Another limitation is the lack of information regarding who was specifically conducting these crowdfunding campaigns. Presenting information on what type of individual, insititution, company, etc. that was hosting these crowdfunding campaigns could provide valuable insights on how size and influence of the host may effect success/failure rates, especially with relation to campaign launch dates and financial goals.
### Suggestions for Further Analysis 
In addition to the current analysis performed, a couple of changes/additions to the data could be made to provide some clearer insights. One change to the theatre outcomes by launch date analysis could be to first filter for the subcategory of "plays" in the Pivot Table rather than the parent category of "theater", as our client Louise is specifically interested in plays. Although providing a similar plot of data, the information provided through this filter will be more accurate for the research topic at hand - small changes between the theatre-filtered dataset and play-filtered dataset could provide valuable confirming or disconfirming inferences. From here, a new table could be created, calculating the percentages of outcomes rather than raw values, and visualized using a stacked column chart to easily represent what percentage of total campaigns in each month were successful, unsuccessful (failed), and canceled. Conversely, the same process could be done with other filters to further specify the data, such as filtering for the country of interest.

In regard to the outcomes based on goals analysis, the same data collected in the table could be used to visualize the raw number of outcomes in a bar chart to compliment the line graph previously made based on percentages. This could provide an easier understanding of where crowdfunding campaigns are most popular regarding financial goal range, and perhaps lend a valuable visual resource to aid in understanding
the "whys" behind any contradictions in trend observed in the previous analysis.






