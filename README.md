# Kickstarting with Excel

## Overview of Project
Kickstarter is a platform, which uses crowdfunding to fund creative projects. This project examines global Kickstarter campaigns from 2009 to 2017 and aims to uncover trends related to theater projects, specifically plays. 

### Purpose
The purpose of this project is gain insights on how different campaigns, specific to plays, fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges
Prior to delving into the analysis, the Kickstarter dataset needed to be further organized by breaking down the “category and subcategory” column in the worksheet, which groups the parent category of theater with its subcategory of plays. By creating separate columns for theater and plays, a more detailed analysis could be conducted.

[Kickstarter Challenge](https://github.com/cmmgw/kickstarter-analysis/blob/main/Kickstarter_Challenge.zip)

### Analysis of Outcomes Based on Launch Date
The focus of this analysis is to analyze the outcomes (successful, failed and canceled) of theater campaigns, based on their launch date. In order to do this, the following steps needed to be taken prior to conducting the analysis. First, the Kickstarter dataset needed to be further organized by creating a “years” column, in order to extract the year from the “date created conversion” column, which provides further clarity into when the campaign was launched. Next, a pivot table was created with the entire data set, by customizing the fields to include filters with “parent category” and “years,” rows with “date created conversion” and columns and values with “outcomes”. By setting up these fields, the pivot chart can then be further filtered by removing the outcomes of live campaigns, modifying the rows to only show the months of the year and filtering the parent category to show data for “theater” only. To visualize the data from the pivot table, a line chart was created to show the relationship between theater campaign outcomes based on their launch month. 

![Resources/Theater_Outcomes_vs_Launch](/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The focus of this analysis is to analyze the percentage of successful, failed and canceled plays based on the funding goal amount. In order to do this, the following steps needed to be taken prior to conducting the analysis. First, a table needed to be created on a new sheet, within the Kickstarter MS Excel workbook. The table aims to capture the outcomes based on campaign funding goals, which are broken down in to 12 groupings, ranging from less than $1,000 up to greater than $50,000. The COUNTIFS function was then utilized to capture the outcome and goal data for the “plays” subcategory, to determine the number of successful, failed and canceled campaigns based off the corresponding funding goal. Based off this data, the total number of successful, failed and canceled projects could easily be calculated by using the SUM function. Upon calculating the percentage of successful, failed and canceled projects, a line chart was created to visualize the data. 

![Resources/Outcomes_vs_Goals](/Resources/Outcomes_vs_Goals.png)



### Challenges and Difficulties Encountered
The main challenge I encountered while working on this project pertained to setting up the Pivot Table fields in MS Excel. Determining how to best visualize the data, based off selecting the most appropriate filter, column, row and value fields is essential. I was able to overcome this through trial and error, until I was able to appropriately visualize the needed data. Prior to creating a Pivot Table, it is necessary to have a sense of which data needs to be summarized, along with how the data should be presented. 

The main challenge encountered with this project overall, was not having a complete dataset which captures current data to effectively analyze trends. Although the dataset captures data points on global campaigns ranging from 2009 – 2017, the data shows that campaigns, specific to plays, were only funded from 2010 to 2017. Incorporating data from 2018 – to date would allow for a deeper and more up to date analysis. 

## Results
-	What are two conclusions you can draw about the Theater Outcomes based on Launch Date?
In analyzing the data, it can be concluded that the success rate of launching a theater campaign is highest in May, followed by June. In May a total of 111 successful campaigns launched, while 52 failed and 3 were cancelled. It can also be concluded that the months of October, November and December prove to have a steady decline in the overall success rate of launching campaigns, with a relative increase in failed campaigns during that period, while not having campaigns canceled in October and about a 50% success/fail rate in December. 

-	What can you conclude about the Outcomes based on Goals?
In analyzing the data, it can be concluded that the rate of success is higher for campaigns with a funding goal that is less than $5,000. Campaigns with a funding goal of less than a $1,000 up to $4,999 had a success rate ranging from 76% - 73%, while campaigns with higher funding goals didn’t have nearly as high of a success rate.  

-	What are some limitations of this dataset?
The main limitation with this dataset is the lack of data pertaining to related to theater projects, specifically plays. The global dataset contains a total of 4,113 data points, of which only 1,065 data points pertain to plays. By increasing the data points across all categories and subcategories, not just the theater category and plays subcategory, the results will be more statistically relevant. Due to the lack of data, it is difficult to assess the full scope of the success of the campaigns. This dataset is also only inclusive of Kickstarter crowdfunding campaigns. In order to truly have a better understanding of the success of theater projects, pertaining to plays, it would be helpful to gather data from a variety of other crowdsourcing platforms.

-	What are some other possible tables and/or graphs that we could create?
Further analysis of the Kickstarter campaigns can be made by generating additional tables and graphs. Conducting a comparative analysis of theater campaigns, as it relates to the 8 other parent categories would be helpful. A deeper dive into the subcategory data under the parent category of theater would also prove to be useful to determine the overall success of plays in comparison to the 36 other subcategories. By following the steps for analysis, referenced above, tables and pivot tables can be generated to help visualize the data and ultimately organize it by utilizing a graph. 



