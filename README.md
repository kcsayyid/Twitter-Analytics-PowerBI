# Twitter-Analytics-PowerBI
Twitter Analytics Dashboard built with Power BI | DAX | Power Query | Data Visualization
INTERNSHIP REPORT

1. Introduction

This internship project focused on analyzing a Twitter social-media dataset using Microsoft Power BI. The primary objective was to transform raw tweet-level data into meaningful visualizations and analytical insights related to user engagement, media interactions, app opens, replies, retweets, likes, and engagement rates.

The project provided practical experience in data preparation, data transformation, DAX calculated columns and measures, filtering, conditional visualization logic, and dashboard development.

A total of six analytical tasks were undertaken based on predefined business requirements. The tasks ranged from basic engagement analysis to more advanced filtering, time-based visualization, trend analysis, and Top-10 tweet identification.

The project helped develop practical data-analysis skills and demonstrated how Power BI can be used to convert raw social-media data into information that can support business and content-strategy decisions.

2. Background

Social-media platforms generate large amounts of data containing information about tweets, impressions, clicks, likes, retweets, replies, media views, media engagements, and other user interactions.

Analyzing these metrics can help organizations understand audience behavior, measure content performance, identify engagement patterns, and support data-driven social-media strategies.

For this internship project, a Twitter dataset was analyzed using Microsoft Power BI. The dataset contained approximately 1,181 records and 21 columns, with tweet data primarily covering the period from June to October 2020.

The project required the application of both basic and intermediate Power BI techniques, including:

Data import and preparation
Data validation and transformation
Power Query
DAX calculated columns
DAX measures
Conditional filtering
Time-based filtering
Even/odd numerical filtering
Text-based filtering
Top-N analysis
Interactive data visualization
Trend and comparative analysis

The project therefore provided practical exposure to the workflow followed in business-oriented data analytics: data → transformation → analysis → visualization → insight.

3. Learning Objectives

The main learning objectives of the internship project were:

To understand how to import and prepare datasets in Power BI.
To develop calculated columns and measures using DAX.
To create appropriate visualizations for social-media analytics.
To apply multiple business rules and filtering conditions.
To analyze engagement metrics such as likes, retweets, replies, and engagement rate.
To compare the performance of tweets with and without media content.
To identify trends and spikes in media interactions.
To perform Top-10 analysis using Power BI.
To implement time-based visualization conditions.
To convert raw data into meaningful and actionable business insights.
To improve practical understanding of Power BI dashboard development.
To develop problem-solving skills while handling complex filtering requirements.
4. Activities and Tasks

During the internship, six major analytical tasks were completed using the social-media dataset.

4.1 Task 1 — Tweet Interaction Breakdown by Category

The first task involved creating a clustered bar chart comparing:

URL Clicks
User Profile Clicks
Hashtag Clicks

These interactions were grouped according to tweet categories such as:

Media
Links
Hashtags

Several business conditions were applied:

At least one interaction must exist.
Tweet date must be an even number.
Tweet word count must be greater than 40.
Visualization should be active only between 3:00 PM and 5:00 PM IST.

A calculated field called Has Interaction was created to identify tweets having at least one of the specified interactions.

An Even Tweet Date condition was also created using DAX.

During validation, it was found that the maximum tweet word count in the dataset was 36. Therefore, the condition Tweet Word Count > 40 resulted in no qualifying records. This demonstrated the importance of validating dataset characteristics before applying strict business rules.

4.2 Task 2 — Engagement Rate Comparison

The second task focused on comparing the engagement rate of:

Tweets with App Opens
Tweets without App Opens

The following conditions were applied:

Weekdays only
Tweet posting time between 9:00 AM and 5:00 PM
Visualization active during 7:00–11:00 AM and 12:00–6:00 PM
Even tweet impressions
Odd tweet dates
Tweet character count greater than 30
Tweets containing uppercase D excluded

After progressively applying the filters:

Filtering Stage	Remaining Tweets
Total dataset	1,181
Weekday + 9 AM–5 PM	71
Visualization active	71
Even impressions	32
Odd tweet date	14
Character count > 30	14
Exclude uppercase D	14

The final eligible dataset contained 14 tweets.

All 14 eligible tweets belonged to the App Opens category, while there were zero tweets in the No App Opens category. Therefore, a statistically meaningful comparison between the two categories could not be made under the exact filtering conditions.

4.3 Task 3 — Media Interaction by Day of Week

The third task involved creating a dual-axis visualization comparing:

Media Views
Media Engagements

The analysis was grouped by day of the week and used the available Q4 2020 data.

The required conditions included:

Even tweet impressions
Odd tweet dates
Tweet character count greater than 30
Exclusion of tweets containing H/h
Visualization active between 7:00–11:00 AM and 3:00–5:00 PM IST

The available dataset contained records from 1 October to 19 October 2020, rather than the complete Q4 quarter.

After filtering, 22 records remained.

Day	Media Views	Media Engagements
Monday	111	5
Tuesday	0	0
Wednesday	443	191
Thursday	120	104
Friday	19	19
Saturday	0	0
Sunday	6	0

Wednesday was identified as the strongest interaction day, with 443 media views and 191 media engagements. Thursday was the second-highest performing day.

4.4 Task 4 — Replies, Retweets and Likes Comparison

The fourth task focused on basic engagement analysis.

A bar chart was developed to compare the total:

Replies
Retweets
Likes

for tweets posted between June and August 2020.

A date filter was applied to include only the required period. Basic SUM aggregation was used.

The analysis included 740 tweets.

Engagement Metric	Total
Likes	5,640
Replies	657
Retweets	359

Likes were the dominant engagement metric, followed by replies and retweets.

This task provided practical experience with basic Power BI aggregation and date filtering.

4.5 Task 5 — Monthly Engagement Rate Trend

The fifth task involved creating a line chart to compare the monthly average engagement rate of:

Tweets with Media
Tweets without Media

The chart used:

Month as the time dimension
Average Engagement Rate as the metric
Media Content as the legend

The approximate results were:

Month	With Media	Without Media
June	5.7%	2.5%
July	5.4%	2.8%
August	5.3%	1.9%
September	4.3%	3.5%
October	5.3%	3.0%

Tweets containing media recorded a higher average engagement rate than non-media tweets throughout the displayed period.

Media tweets reached their highest approximate engagement rate in June at 5.7%. Their performance declined through September before recovering to approximately 5.3% in October.

Non-media tweets showed greater variation, reaching their highest level of approximately 3.5% in September.

The analysis suggested that media content was associated with stronger engagement, although other factors such as content topic, posting time, audience interest, campaign activity, tweet frequency, and seasonal effects may also influence engagement.

4.6 Task 6 — Top 10 Tweets by Engagement

The sixth task focused on identifying the Top 10 tweets based on total engagement, where:

Total Engagement = Retweets + Likes

The following conditions were applied:

Weekdays only
Odd tweet dates
Even impressions
Tweet word count less than 30
Visualization active between 3:00 PM and 5:00 PM IST
Top 10 tweets based on total engagement

The user profile associated with each qualifying tweet was included in the visualization.

This analysis provided a focused method for identifying high-performing tweets and understanding which content generated greater audience interaction.

5. Skills and Competencies

The internship project helped develop the following technical and analytical competencies.

5.1 Power BI

Practical experience was gained in:

Importing datasets
Creating charts and dashboards
Applying visual-level and page-level filters
Creating interactive reports
Configuring chart axes and legends
Sorting categories
Creating Top-N visualizations
5.2 DAX

The project provided practical experience in creating:

Calculated columns
Measures
Conditional logic
Time-based conditions
Even/odd classification
Text-based classification
Engagement calculations
Visualization visibility logic
5.3 Power Query

Power Query was used for data preparation and transformation before analysis.

5.4 Data Analysis

The project developed the ability to:

Identify engagement patterns
Compare different engagement metrics
Analyze time-based trends
Identify high-performing days
Compare media and non-media content
Identify high-performing tweets
5.5 Problem Solving

The project required troubleshooting situations where multiple filters produced few or zero records. Instead of assuming that the Power BI visualization was incorrect, the underlying dataset was examined to identify the reason.

5.6 Business Intelligence

The project improved understanding of how technical data-analysis results can be converted into business-oriented insights that may support social-media content strategies.

6. Feedback and Evidence

Evidence of the internship work includes the Power BI visualizations, DAX calculations, calculated columns, filtering configurations, and analytical results developed during the project.

The report demonstrates practical implementation of the following Power BI features:

Clustered bar charts
Clustered column charts
Line charts
Line and clustered column charts
Top-N analysis
DAX calculated columns
DAX measures
Visual-level filters
Date and time filters
Conditional visualization logic

The analytical results provide measurable evidence of the work performed.

For example:

The original dataset contained approximately 1,181 tweets.
Task 2 resulted in 14 final eligible tweets.
Task 3 resulted in 22 filtered records.
Task 4 analyzed 740 tweets from June–August 2020.
Task 4 recorded 5,640 likes, 657 replies, and 359 retweets.
Task 3 identified Wednesday as the strongest media-interaction day.
Task 5 demonstrated higher average engagement for media tweets across the displayed months.

These results demonstrate the application of Power BI techniques to a real analytical dataset.

7. Challenges and Solutions

Several challenges were encountered during the project.

Challenge 1 — Multiple Filtering Conditions

Some tasks required several conditions to be applied simultaneously, including date, time, numerical, text, and categorical filters.

Solution

The filters were implemented progressively and validated at each stage. This helped identify which condition caused the reduction in available records.

Challenge 2 — Blank Visualization

In Task 1, the condition Tweet Word Count > 40 resulted in a blank visualization.

Solution

The maximum word count in the dataset was checked. It was found to be 36, meaning that no tweet could satisfy the requirement of more than 40 words.

This demonstrated the importance of checking the underlying data before assuming that a visualization or DAX calculation is incorrect.

Challenge 3 — No Comparison Group

In Task 2, all 14 final eligible tweets had app opens, while there were no tweets without app opens.

Solution

The result was treated as a dataset limitation rather than artificially modifying the data. The report clearly documented that a direct statistical comparison could not be made because the No App Opens category contained zero observations.

Challenge 4 — Time-Based Visualization

Several tasks required visualizations to be displayed only during specific IST time windows.

Solution

DAX-based time logic and visualization visibility measures were developed and applied as visual-level filters.

Challenge 5 — Incomplete Quarter Data

For Task 3, the dataset did not contain the complete Q4 2020 period. The available records covered only 1 October to 19 October 2020.

Solution

The analysis was clearly documented as being based on the available Q4 records rather than representing the complete calendar quarter.

8. Outcomes and Impact

The internship project successfully provided practical experience in Power BI-based data analytics and business intelligence.

The major outcomes were:

Technical Outcomes
Developed multiple Power BI visualizations.
Created DAX calculated columns and measures.
Applied complex filtering conditions.
Implemented time-based visualization logic.
Performed Top-N analysis.
Used Power Query for data preparation.
Created comparative and trend-based visualizations.
Analytical Outcomes

The project produced several useful insights:

Likes were the dominant engagement metric during June–August 2020, with 5,640 total likes.
Wednesday recorded the highest media interaction in the filtered Q4 data, with 443 media views and 191 media engagements.
Tweets containing media showed higher average engagement rates than tweets without media throughout the displayed June–October period.
The Task 2 filtering conditions produced 14 eligible tweets, all of which had app opens.
The Top-10 analysis established a framework for identifying high-performing tweets using retweets and likes.
Strict business filters can significantly reduce the available dataset, making data validation an essential part of the analytical process.
Professional Impact

The internship improved practical readiness for a Data Analyst / Business Intelligence role by providing experience with the complete analytical workflow:

Raw Data → Data Preparation → DAX → Filtering → Visualization → Analysis → Business Insight

The project also strengthened problem-solving skills and demonstrated the importance of validating analytical results against the underlying dataset.

9. Conclusion

The Power BI Social Media Analytics internship project provided valuable practical experience in data preparation, data visualization, DAX, filtering, dashboard development, and analytical interpretation.

The six tasks covered different levels of Power BI analysis, from simple SUM-based engagement comparisons to more advanced time-based filtering, text filtering, Top-N analysis, and trend analysis.

The project demonstrated how raw social-media data can be transformed into meaningful insights. The analysis identified important engagement patterns, including the dominance of likes, strong media interaction on Wednesday, and higher engagement rates for tweets containing media.

The project also demonstrated the importance of understanding data limitations. For example, some business requirements produced no qualifying records or no comparison group because of the characteristics of the supplied dataset. These situations were analyzed and documented rather than being ignored.

Overall, the internship strengthened my practical knowledge of Microsoft Power BI, Power Query, DAX, data visualization, data analysis, filtering, and business intelligence. It also improved my ability to investigate data problems, communicate analytical findings, and convert business requirements into practical analytical solutions.

The experience has provided a strong foundation for pursuing opportunities in Data Analytics and Business Intelligence, particularly roles involving Power BI, SQL, Excel, data visualization, and business reporting.
