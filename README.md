# Analysis of Kickstarter Campaigns for Plays

## Overview of Project
### Purpose
This project was focused on ascertaining whether or not the start date and overall fundraising goal has a direct correlation with success rates. It is in taking a deeper look at these key criteria that I can then advise the client on the following: how much of a fundraising goal is reasonable and what time of year is most appropriate to launch a campaign?

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
To start, I focused on what effect, if any, the launch date of a Kickstarter campaign had on its success. By filtering for 'theater' campaigns as well as the launch month in a pivot table, I was able to visualize how many theater campaigns were successful, failed, or canceled based on their launch month. This visualization is found in Figure 1 below.
![(https://github.com/rankx034/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png?)]

As Figure 1 shows, there were significantly more successful theater campaigns that began in the month of may than any other month. The rest of summer comes with a drop-off in successful launches, but is still higher than the rest of the year. Failed campaigns do not appear to follow a similar trend, however there is a noted increase in the incidence of failed campaigns in mid-Autumn. The increase in successful summer launches can likely be attributed to the cyclicality of the theater season, or the period of the year in which theaters will perform before going on hiatus. This is typically between September and May, but can certainly vary based on the size and popularity of the production company. 

There is also a gap in the number of canceled campaigns during the month of October, although this could be a result of the overall low number of canceled campaigns. 

A challenging aspect of this portion of the analysis appears to have been an error in the dataset causing the data presented in the pivot table to be unreliable. The number of successful campaigns in each month was much lower than it should normally be, and most data was in a 'blank' tab. This was remedied by reverting to a previous save of the dataset and re-running the filters and date conversions. Once this was accomplished, I was able to produce a clean visualization for Figure 1.

### Analysis of Outcomes Based on Goals

To begin analysis of theater campaigns' outcomes based on the fundraising goals, statistical analysis was run on each of the following categories: successful, failed, and canceled campaigns. Twelve ranges were identified in order to separate campaigns into discrete categories based on their goal. From there, I calculated the success/fail/cancel rate within each range. After that, I created a line chart to visualize the date. See Figure 2. 
![Figure 2(https://github.com/rankx034/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png?raw=true)]

What we can see from the chart is that as the fundraising goal increases, the likelihood of success decreases. In other words, most successful campaigns have goals of below $9,999. Unless a campaign is very high profile or already has a significant level of interest, it is recommended to keep fundraising goals to a modest level. 

## Results

The results of the analysis help to understand key aspects of previous campaigns that may help those looking to start one in the future, but the dataset does not really give us affirmative insight as to why in particular summer campaigns are more successful. We can certainly use that information to our advantage, but as for why it occurs, we can only infer. Regarding future analysis that the dataset can offer, it would likely be in the client's best interest to look specifically at outcomes within the campaign's target country. Additionally, it might be worth taking a look at 'backers count' vs. outcomes. Specifically, did the successful campaigns with large fundraising goals have a small number of backers, indicating donations by large organizations? Or perhaps they had many more backers than small campaigns as a result of successful outreach? 
