# AB-Testing-Marketing-Campaign-Analysis
Marketing Campaign Analysis: A/B Testing
Introduction
In the world of marketing, making informed decisions is crucial for success. This project uses A/B Testing to evaluate the effectiveness of a marketing campaign, focusing on the conversion rates of two groups: users exposed to advertisements (Ad group) and those shown public service announcements (PSA group).

Objective
The primary objectives of this analysis are:

Assess whether the marketing campaign effectively drives conversions.
Compare conversion rates between the Ad group and the PSA group.
Dataset
The dataset consists of 588,101 entries with the following columns:

User ID: A unique identifier for each user.
Test Group: Specifies whether the user was in the Ad group (saw advertisements) or the PSA group (saw public service announcements).
Converted: A boolean field indicating whether the user purchased a product (True for purchase, False otherwise).
Total Ads: The number of ads the user saw.
Most Ads Day: The day the user saw the highest number of ads.
Most Ads Hour: The hour of the day the user saw the most ads.
Exploratory Data Analysis (EDA)
Distribution of Test Groups
564,577 unique users in the Ad group.
23,524 unique users in the PSA group.
Conversion Rates
Out of all the users:

14,843 users converted (made a purchase).
573,258 users did not convert.
This results in an overall conversion rate of 2.52%.

Group-Level Performance
We further broke down the dataset into two groups and calculated the following purchase rates:

Ad Group: 2.55%
PSA Group: 1.79%
The results indicate that users in the Ad group converted at a higher rate than those in the PSA group.

Statistical Analysis: Z-Test
To ensure that the difference in conversion rates is statistically significant, we performed a Z-test:

Hypotheses
Null Hypothesis (𝐻0): There is no significant difference between the conversion rates of the Ad group and the PSA group.
Alternative Hypothesis (𝐻1): The conversion rate of the Ad group is significantly higher than that of the PSA group.
Results
Z-Score: 7.37
P-Value: 8.53e-14
Since the P-Value is much lower than our significance level (0.05), we can reject the null hypothesis and conclude that the Ad group has a significantly higher conversion rate than the PSA group.

Conclusion
The A/B test reveals that the Ad group outperformed the PSA group, with a significantly higher conversion rate. This suggests that the marketing campaign using advertisements is more effective at driving conversions.

Key Insights:
Ads result in higher conversions compared to PSAs.
Statistical evidence supports the claim that the difference in conversion rates is significant.
