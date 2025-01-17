# Analyzing the Outcomes of Kickstarter Campaigns

## Overview of Project
Kickstarter is a crowdfunding platform that enables people around the world to donate to organizations and causes. Our client wishes to organize a play caled **Fever**, and aims to raise $10,000 on Kickstarter to accomplish this. In order to advise the client on how to organize the campaign, the Kickstarter outcomes of different theater campaigns were analyzed across different variables, such as the campagin launch date and monetary goal. Visualizations of the data suggest that our client should start their fundraising in the early summer, especially May, since theater campaigns have the highest success rate during this time of the year. As for finances, plays with a fundraising goal between $10,000-$14,999 have a success rate of roughly 55%, and those between $5,000-$9,999 were roughly 55% as well. From these rates, it would normally be advised that the cient avoid lowering the goal much below $10,000 because there will not be a higher success rate between $5,000 and $9,999. However, the average successful campaign goal for all campaigns of all categories is $5,050, in contrast to $10,550 for failed campaigns. Therefore, a goal between $5,000-$9,999 is advised. Overall, theater campaigns have been more successful in the U.S. compared to other cateogries, so fundraising for a play is a viable option.

![Kickstarter-Challenge](Kickstarter_Challenge.xlsx.zip)

### Purpose
To understand what makes a successful campaign, an analysis was performed on Kickstarter data from 2009 - 2017 for over 4,000 campaigns in a variety of categories, e.g. theater, concerts, and television. Our client, Louise, plans to launch a Kickstarter for her play, **Fever**, with a budget of $10,000, but would like information on the factors that dictate the success or failure of a campaign. The analysis revealed that the outcome of campaigns correlated strongly with their launch date, funding goals, and fundraising cateogry. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The month of the launch date dictated the success and fail rates for plays in the U.S. As seen in the line chart below, the month with the higest success rate was May, so this would be the best time to launch the kickstarter. The line chart for theater outcomes suggests that June and July are also viable options if the month of May is not possible. In other words, early summer is the best time to start a campaign. It is advised to avoid launching a campaign in October or November since the success rate between Summer and Fall decreases sharply. The failure rate is steady over the course of the year, so the fail rate need not be addressed when comparing success rates.

![Theater_Outcomes_vs_Launch](images/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
As seen in the line chart below, the theater campaigns that succeeded the most frequently were those that set their goal less than $5,000 - the success rate was roughly 65%. Nevertheless, theater campaigns that set a goal between $5,000 and $15,000 had success rate of roughly 55%. Beyond $15,000, the sucess rate plummets and the failure rate sharply rises, and these changes only reverse at a goal of roughly $30,000, which is out of range of our client's budget. It should be noted that the fail rate steadily increases from $1,000 to $5,000 but then levels off from $5000 to $15,000. However, this line chart does not take into account that the average failed campaign across all categories had a goal of $10,550 (see **Results** section). Therefore, lowering the goal between $5,000 and $9,999 would be the safest option.

![Outcomes-vs-Goals](images/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

Making a final decision on the recomended budget proved difficult because of the graph showing outcomes based on goals. The success rate and fail rate remain stagnant from $5,000 to $15,000, so it was difficult deciding wether to advice Louise to simply maintain the goal at $10,000 or to try for more. The range $5,000-$9,999 was decided upon because the average goal for failed campaigns across all categories was $10,550, so lowering Louise's goal closer to the average goal of successful campaigns, $5,050, seemed like the safest option. These means were skewed to higher values due to outliers, which makes this statistic less reliable than at it noramlly would be. Using the median may prove to be more reliable due to its resistance to outliers, but the median for succesful campaigns was roughly $3,000, which is too low for Louise's budget. Thus, the range $5,000-$9,999 is the a suitable recomendation because it does not suggest that Louise has to lower her budget by an unrealistic amount while also advising her to avoid going over $10,000.

As previously mentioned, outliers in the dataset increased the average goal and average pledge amounts, inhibiting data analysis. For example, some campaigns had outlandishly high percent funding rates - the campaign would set a goal of $1, likely because they needed a goal recorded on paper, and when they received a small donation of, say, $100, the percent funding would amount to 10,000%. As a result, the outliers misrepresented the color scaling for the percent funding column. 

An analysis was to be performed on the blurb column, but some characters were not translated correctly from the csv file to the Excel file. Manually editing these errors would be time-consuming. Even without this issue, it would be difficult to turn the words into a variable that could be analyzed against the play outcomes. As a result, the wording of the fundraising blurbs were not analyzed. Using Machine Learning, however, an analysis of the wording could be possible, and could be an idea for a future project.

Another issue arrises when analyzing monetary data across different countries. Although the dataset is in dollars, the actually currency must be taken into account. For example, $100 in GBP is $126 in USD. In this project, there was no analysis of financial data among countries, but if Louise wished to compare the success of plays between Great Britain and the U.S., as she mentioned previously, then the currency would have to be accounted for. 

## Results

In the U.S. from 2009-2017, fundraising for theaters experienced a higher success rate than that of any other category. Among musicals, plays and spaces, plays had the highest success rate, as seen in the second bar graph. This means a fundraising for a play would likely succeed in the U.S.

![US-Stacked-Bar-Chart](images/US-Stacked-Bar-Chart.png)
![US-Subcat-theater-stacked-bar-chart](images/US-Subcat-theater-stacked-bar-chart.png)

A majority of the U.S. campaigns that failed set their funding goals far higher than the successful campaigns. The average goal was $5,050 for successful US kickstarters, but $10,550 for the failed fundraisers. However, the average pledge was $5,600 for those that succeded versus $560 for those that failed, meaning the unsuccessful kickstarters failed due to factors other than setting the price range too high. 

The client has set their fundraising goal to be $10,000, but the average failed campaign has a goal of $10,550. Therefore, it is advised that the client avoid raising the price beyond $10,000, and keeping the goal between $5,000 and $9,999, which still has a similar success rate to a goal of $10,000 as seen in the time series graph in a previous section.

Our client also expressed an interest in fundraising a musical in GB with a goal of 5,000 pounds. The box plot shows the distribution of musicals in Great Britain. Half the pledges ranged from 0.00-1,800.00 pounds. Therefore, a goal closer to 2,000 pounds would be a safer option for fundraising a musical in GB. However, of the 5 plays that the client preferred, all succeeded, and monetary goal ranged from 1,000-4,000 pounds, with the pledges exceeding their goals by 1% more up to 172% more. Therefore, if the client fundraised for one of these 5 musicals, she could safely set a goal near 4,000 pounds. 

![Box-Plot-John-Hendricks](images/Box-Plot.png)

### Final Thoughts

Initiating a kickstarter for a play in the early summer, especially the month of May, would likely be successful in the U.S, as long as the funding goal is not much larger than $10,000. A fundraising goal of $5,000-$9,999 is advised because this value is closer to the average and median goals for successful campaigns while maintaining a relatively high success rate. Launching in June would be a viable second option, but the winter months should be avoided.    
