# Kickstarter Challenge

# Kickstarting with Excel

## Project Overview
### Purpose and Goal
The purpose of this analysis is to understand the relationship between campaign launch timing and funding outcomes for theater kickstarter campaigns. In addition, we look closer at theater kickstarter campaigns specifically for plays to understand the relationship between the size of the funding goal and the outcome of the campaign. 

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In order to understand the relationship between campaign launch timing and funding outcomes, we analyzed data for the theater category. This analysis was completed using data on 1,369 completed or cancelled theater kickstarter campaigns that launched between July 2010 and February 2017. Analysis was limited to consider the month of the launch without consideration to the year and included all subcategories within the theater category. The analysis was conducted using a simple pivot table and line chart that organized the number of successful, failed and cancelled campaigns based on the month each was launched. The resulting pivot table is shown 

### Analysis of Outcomes Based on Goals
The second analysis focused on the subcategory of theater campaigns that were plays. This analysis was completed by focusing on 1,047 kickstarter campaigns for projects in the play subcategory that outcomes of successful, failed or cancelled. In order to do this the kickstarter campaigns were grouped based on ranges of goal amounts beginning with those that were Less Than 1000, 1000 To 4999, and then proceeding in increasing ranges of 5000 up to the final range of 50000 or More. These groupings were achieved using the Countifs function in Microsoft Excell (MS). An example of this formula is one used to obtain the number of successful campains for plays with a goal from 1000 to 4999: 
>=COUNTIFS('Kickstarter Data'!$R:$R,"plays",'Kickstarter Data'!$F:$F,"successful",'Kickstarter Data'!$D:$D,">=1000",'Kickstarter Data'!$D:$D,"<5000")>
Once the relevant total counts for each range and outcome were identified, arithmetic formulas were used to determine the percentage of campaigns within each range that were successful, failed or cancelled. This resulted in the following 



### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?




## Analysis and Challenges


## Results
