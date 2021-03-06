# Kickstarting with Excel

## Overview of Project

In this project we assess how Kickstarter campaigns of the theater parent category performed relative to the month of the campaign launch date as well as how campaigns in the play subcategory performed relative to their funding goals.

### Purpose

The objective is to ascertain trends for successful Kickstarter campaigns for by visualizing data for similar campaigns to assess which months of the year have the highest success for theater campaigns and what funding goals are most attainable by plays.

## Analysis and Challenges

To perform the analysis of theater Kickstarter campaigns by the month they were launched we needed to parse the dates and group campaigns by month. Within each grouping we segregate successful, failed, canceled, and total campaigns. There were no challenges in doing so, however there are things to consider when reviewing such data. The theater category itself comprises only 1393 line items, of which 1066 are plays. If we were interested in a subset other than plays there may not be enough data to make correlations with. Even as such, there's no guaranteeing that plays comprising the bulk of the data aren't skewing the results for the broader category. Such an assessment wouldn't be difficult to make by individually visualizing data for musicals and theater spaces and comparing it with play data. Considering the request is predicated on an active campaign in the play category it would make more sense to assess only plays relative to launch date. 

The analysis of campaign success based on funding goal of plays was done by grouping all plays into goal categoriees. Within each grouping campaign success, failure, and cancelation are tabulated. While not a challenge, manually entering values in each of the formulas presents repeated opportunity for error which could easily introduce errors into the visualization of campaign outcomes. Additionally we assess campaign cancelation when there were no instances in 1066 campaigns of such happening. This isn't problematic for data analysis but does pique questions about the campaigns that failed and how they initially performed prior to the funding deadline. This could be indicative that they appeared to be on track funding but then failed, but without additional data not provided we are unable to do further analysis to see whether these campaigns appeared like they might fund early on or if the campaign owners simply chose not to cancel and relaunch the campaigns later are revising them as is a common occurence in other types of campaigns.

### Analysis of Outcomes Based on Launch Date

[Outcomes Based on Launch Date](Resources/Theater_Outcomes_vs_Launch.png)

Theater campaigns launched in May and June have noticeably higher success rates than the average camaign with that success rate declining over the summer months, whereas campaigns launched in December have noticeably lower success rates than the average campaign.

### Analysis of Outcomes Based on Goals

[Outcomes Based on Goals](Resources/Outcomes_vs_Goals.png)

Plays with a low funding goal have a much higher chance of success declining as the funding goal increases. There's a marked increase in success of plays in the $35000 to $40000 funding goal range, however not shown by the visualization is that there were only a few campaigns in this range which makes those results uncertain. 

### Challenges and Difficulties Encountered

The dataset provides only a limited view of the failures/successes of Kickstarter campaigns. In the case that a campaign fails it would be beneficial to receive a daily or weekly breakdown of progress toward the funding goal so we can analyze why a particular campaign failed or whether it looked like it might succeed initially but pledge momentum declined. It would be interesting to see how all campaigns fared at 1/4 intervals through a campaign and might provide us another meaningful data point to assess to determine what % funded a campaign needs to be through each week(or appropriate interval) through a campaign, what the average decline in pledges are the longer a campaign runs, etc. Additionally, we have the pledged amount and the total number of backers but we don't have a more detailed breakdown of pledge contributions. A larger dataset with a granular look at the funding would allow us to make a more detailed look at campaigns and assess probability of success or failure if reliant upon a specific target funding level per expected number of backers. As noted above some aspects of the data are rather limited and the visualizations are potentially misleading, specifically for plays in the $35000 to $40000 funding goal range. There wasn't enough campaigns to be able to determine any trends based on such a small sample size.

## Results

To optimize a campaign for success in the theater category the best time to launch a campaign is May/June. For a play campaign to be successful a pledge goal over 5000 has a steep impact on whether a campaign will fund or not with the best results being those with a goal of less than $5000. 

To get a more complete look at the success rates of campaigns we could look at factors such as the impact of Staff Pick or Spotlight and if such attributes skew the data in any particular direction. And while we assessed specific markets before (US vs. GB) we didn't review that in this look at the data. Analyzing such things could give us a more realistic look at the expected outcome in the relevant market.
