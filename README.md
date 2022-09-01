# Kickstarter Challenge

# Kickstarting with Excel

## Project Overview
### Purpose and Goal
The purpose of this analysis is to understand the relationship between campaign launch timing and funding outcomes for theater kickstarter campaigns. In addition, we look closer at theater kickstarter campaigns specifically for plays to understand the relationship between the size of the funding goal and the outcome of the campaign.
 
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In order to understand the relationship between campaign launch timing and funding outcomes, we analyzed data for the theater category. This analysis was completed using data on 1,369 completed or cancelled theater kickstarter campaigns that launched between July 2010 and February 2017. Analysis was limited to consider the month of the launch without consideration to the year and included all subcategories within the theater category. The analysis was conducted using a simple pivot table and line chart that organized the number of successful, failed and cancelled campaigns based on the month each was launched. An image of the pivot table can be reached using the following link.

![Launch Month and Outcomes Pivot Table](https://github.com/jessica1258/kickstarter_challenge/blob/main/Outcomes_vs_Launch_pivot.png)

### Analysis of Outcomes Based on Goals
The second analysis focused on the subcategory of theater campaigns that were plays. This analysis was completed by focusing on 1,047 kickstarter campaigns for projects in the play subcategory that outcomes of successful, failed or cancelled. To do this, the kickstarter campaigns were grouped based on ranges of goal amounts beginning with those that were Less Than 1000, 1000 To 4999, and then proceeding in increasing ranges of 5000 up to the final range of 50000 or More. These groupings were achieved using the Countifs function in Microsoft Excell (MS). An example of this formula is one used to obtain the number of successful campains for plays with a goal from 1000 to 4999:
>=COUNTIFS('Kickstarter Data'!$R:$R,"plays",'Kickstarter Data'!$F:$F,"successful",'Kickstarter Data'!$D:$D,">=1000",'Kickstarter Data'!$D:$D,"<5000")
Once the relevant total counts for each range and outcome were identified, arithmetic formulas were used to determine the percentage of campaigns within each range that were successful, failed or cancelled. An image of the table is shown below.

![Goals and Outcomes Pivot Table](https://github.com/jessica1258/kickstarter_challenge/blob/main/Outcomes_vs_Goals_Table.png)

### Challenges and Difficulties Encountered
The analysis conducted is a simplified approach focused on two potential factors that may contribute to the success of theater campaigns similar to Louise’s play Fever. In conducting the analysis, there were three challenges that impacted the outcome of our analysis. First, we had too much date relative to the analysis. The data set included data elements (columns) far beyond the scope of the intended analysis and campaigns in other categories and subcategories that were not used (rows). Without additional information, it is a challenge to determine whether that data should have been considered. Second, the data available did not include a data dictionary or other reference material that would ensure we interpreted and analyzed data correctly in the context of how that data was created. Third, the data was not normalized to ensure comparability of the data across the sample of kickstarter campaigns. For the purpose of this analysis, the most problematic issue impacted the analysis of Goals versus Outcomes, where we used the goal amount to establish ranges. Across the kickstarted campaigns, there were 12 different currencies used with a wide range of foreign exchange rates relative to USD. As a result, our assignment of individual kickstarter campaigns may not be reasonable groupings.

## Results
Based on the analysis of Outcomes based on Launch Date, we see that the highest number of successful theater kickstarter campaigns are launched in the months of May and June. This is in part because these months have highest number of total launches and in part because more of the launches that occur are successful. In addition, we see that May and July large number of failed campaigns in months with a very high number of campaign launches while October and December have a high rate of failure, with the number of failed campaigns nearly matching that of successful campaigns in those months. A graphical representation of is shown below.

![Launch Month and Outcomes Graph](https://github.com/jessica1258/kickstarter_challenge/blob/main/Theater_Outcomes_vs_Launch.png)

The analysis of Outcomes based on Goals, we see that play campaigns with relatively small goals (Less Than 1000 and 1000 to 4999) have a higher rate (greater than 60%) as do the ranges 35000 to 39999 and 40000 to 44999. This implies that goals in those ranges have a greater ability to be successful relative to the other ranges. A graphical representation of is shown below.

![Goal and Outcomes Graph](https://github.com/jessica1258/kickstarter_challenge/blob/main/Outcomes_vs_Goals.png)

There are several limitations in this dataset, some of which have been addressed as challenges in earlier sections of these materials. In addition to those items, the data set has larger representation from 2014 through 2016 compared to the other years in the data set (2009-2013 and 2017). It is not clear whether that is representative of an overall higher number of kickstarted campaigns or of the adoption of kickstarter as a fundraising tool or if that means this sample may not be representative for use in informing successful campaign design for plays.
Overall we used a small amount of data for analysis. To improve our understanding of the data, we could have looked at other factors that may have contributed to campaign success, such as the duration of a campaign or the timing of when it closed and applied similar data techniques and graphs to understand if there were trends that may inform campaign design in the future.
