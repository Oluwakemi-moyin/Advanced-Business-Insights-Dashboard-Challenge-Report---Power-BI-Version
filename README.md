# Advanced-Business-Insights-Dashboard-Challenge-Report---Power-BI-Version
Tools used: Python, PowerBI
Introduction

The mobile app market is rapidly evolving, and platforms like the Google Play Store are continuously striving to maintain their leadership position in a highly competitive and dynamic environment. To ensure sustainable growth and adapt to ever-changing market conditions, leveraging data-driven insights has become a crucial strategy. In this context, the role of data analytics is paramount, enabling businesses to make informed, proactive decisions that drive performance, user engagement, and revenue optimization.

As a Senior Data Analyst of Google, my mission was to create an interactive dashboard using Power BI that would provide the Google Play Store leadership team with actionable insights to enhance app performance, user engagement, and revenue generation. The dashboard integrates multiple data sources, including internal Google Play Store metrics, external market trends, and sentiment analysis, offering a comprehensive view of app performance in the context of broader industry dynamics. Through this solution, our aim is to empower senior executives with the tools necessary to make data-backed decisions that foster continued success in a competitive market.

## Objective
This report outlines the process of developing the Advanced Business Insights Dashboard, from initial dataset exploration and cleaning to the creation of a dynamic, interactive Power BI dashboard. It highlights the key performance indicators (KPIs) that were defined, predictive analytics techniques used, and the valuable business insights that were derived. Additionally, actionable strategic recommendations are provided, designed to help the leadership team optimize their app portfolio, increase user satisfaction, and drive revenue growth.


1. Dataset Exploration & Understanding

1.1 Google Play Store Dataset

The first step involved downloading and analyzing the Google Play Store dataset, which provides key metrics such as ratings, reviews, install count, price, and category for each app. 

The following important data points were identified for analysis:

● App Ratings: Indicates app quality and user satisfaction.

● Number of Installs: Reflects app reach and user base.

● Price: Impacts app revenue and market positioning.

● Category: Allows for segmentation of the app market for comparison.

● Reviews: Provides qualitative data on user experience and sentiment.

These features serve as the foundation for generating actionable insights into app performance, market positioning, and user engagement.

1.2 Data Exploration & Cleaning

● Handling Missing Values: Imputation techniques were applied to fill missing data, such as using median imputation for numerical fields like app ratings and installs.

● Removing Duplicates: Duplicates were identified and removed to ensure each app entry was unique.

● Standardizing Data: Consistency was ensured by standardizing columns like ratings and prices.

1.3 Key Findings

Early analysis revealed several important insights:

● The majority of top-performing apps are free-to-download, generating revenue primarily through in-app purchases and ads.

● Apps in the Games category exhibit the highest install counts and ratings.

● Higher ratings tend to correlate with increased user engagement metrics (e.g., more reviews and higher ratings).

2. Integration of External Data

2.1 External Dataset: Sentiment Analysis of User Reviews

To enhance our insights, we incorporated an external dataset appledataset that includes sentiment analysis of user reviews across apps. This qualitative data provided us with:

● User Satisfaction Assessment: Apps with a higher positive sentiment tend to have better ratings and stronger user engagement.

● Identification of Areas for Improvement: Negative sentiment in reviews signals issues impacting app performance that need addressing.

2.2 External Dataset: Market Trends and Competitor Analysis

An external dataset apple dataset was integrated containing market trends and competitor performance. This dataset helped to:

● Benchmark Performance: Compare Google Play Store apps with competitors to identify strengths and weaknesses.

● Identify Growth Opportunities: Pinpoint underperforming categories or apps that could be targeted for growth.

3. Advanced Data Cleaning & Preparation

3.1 Handling Complex Data Issues

● Missing Values: For time-based data like revenue trends, we used forward filling, while median imputation was applied to numerical fields.

● Outliers: detected and addressed outliers that could skew predictive models, such as excessively high install counts for a small subset of apps.

3.2 Data Standardization

Standardized data across datasets to align timeframes and categorizations. For instance, external market growth data was aggregated quarterly to match the Google Play Store dataset’s time intervals.

4. Defining KPIs & Predictive Analytics

4.1 Defining KPIs

Identified 12 critical KPIs to provide valuable insights into app performance and market positioning:

1. Average Rating Score:

● Why it Matters: The average rating score is a direct reflection of the app's quality and user satisfaction. A higher rating suggests that users are generally happy with the app’s functionality and performance. It can influence potential users' decisions to download the app and is often considered a key indicator of the app’s overall success. Tracking this helps developers and businesses understand how well their app is meeting user expectations and where improvements are needed.

![Screenshot 2025-03-22 042002](https://github.com/user-attachments/assets/b6ae839a-5e61-42fb-b349-27edbc466ebc)

2. Average Rating Score by Category:
● Why it Matters: By analyzing average ratings across different app categories, we can compare performance within specific niches (e.g., games, utilities, productivity). Somecategories may have more competitive environments, which makes it harder to achieve high ratings. This KPI provides context for how an app is performing relative to others in the same space, offering valuable insights for identifying areas of improvement or areas where an app is excelling.

![Screenshot 2025-03-22 042019](https://github.com/user-attachments/assets/3b1c1049-8830-4b41-852c-7d3d4ecfca86)

3. Total Downloads:
● Why it Matters: The total number of downloads serves as an indicator of an app’s reach and popularity. Higher download numbers often correlate with higher visibility, more user engagement, and stronger revenue potential. This KPI is crucial for understanding how well an app is being adopted by users and is especially important for evaluating the app's market penetration.

![Screenshot 2025-03-22 042027](https://github.com/user-attachments/assets/52e4eb49-34e8-4418-b751-aeb7a77145d9)

4. Average User Rating:
● Why it Matters: While the average rating score offers a snapshot of overall app performance, the average user rating (based specifically on user reviews) provides a closer look at how users feel about the app. User feedback often includes valuable qualitative insights that reveal specific features users appreciate or issues that need addressing. Tracking this helps app developers improve user experience and optimize
app features to enhance user satisfaction.
![Screenshot 2025-03-22 042046](https://github.com/user-attachments/assets/5dd576fd-c638-436d-81f8-4460a8151ac6)

5. Count of Apps:
● Why it Matters: The total number of apps on the Google Play Store offers a broad overview of market saturation. By understanding how many apps are available in various categories, you can evaluate the level of competition for a given type of app. This helps app developers and marketers position their products effectively and identify whether there is room for new apps in underserved categories or areas with lower competition.
![Screenshot 2025-03-22 042054](https://github.com/user-attachments/assets/dc7da894-f4d1-4198-ac32-6715fd0c2ea2)

6. Count of Content Rating:
● Why it Matters: The number of distinct content rating classifications (e.g., E for Everyone, M for Mature, etc.) provides insights into the types of audiences targeted by apps. Analyzing this KPI helps app developers understand what content is most popular among different demographic groups and aids in developing new apps or modifying existing ones to cater to specific user needs or market trends.
![Screenshot 2025-03-22 042103](https://github.com/user-attachments/assets/cf3bcaac-08bb-4a4c-a97e-a90200f7cb62)

7. Count of Categories:
● Why it Matters: The number of app categories reflects the diversity within the Google Play Store ecosystem. Apps can be categorized into multiple groups, and this KPI helps assess how fragmented or broad the market is. A larger number of categories may indicate a greater diversity of apps and target audiences, while a lower number may suggest room for new specialized apps. This information is useful for identifying market gaps and new opportunities for app development.
![Screenshot 2025-03-22 042110](https://github.com/user-attachments/assets/4d962fdb-5ae7-448f-804e-85b30852f266)

8. Maximum Byte Size:
● Why it Matters: The app with the highest installation size (measured in bytes) indicates the heavy-duty applications that may require more storage space and resources on users' devices. Knowing this helps developers optimize their apps to balance feature richness with efficient use of storage. Apps with excessively large sizes might deter users from downloading, especially in markets where storage is limited. This KPI can guide developers to optimize app size while maintaining functionality.
![Screenshot 2025-03-22 042117](https://github.com/user-attachments/assets/b740e484-8af3-4d01-8fb1-74b4a5532015)

9. Category by Minimum/Maximum Install:
● Why it Matters: This KPI compares categories that have the highest and lowest install counts. It helps identify which types of apps are experiencing the most and least popularity. Apps in categories with high install counts may have a larger user base and more opportunities for monetization, while categories with low installs could present untapped potential for growth. This data helps stakeholders make informed decisions about where to focus development efforts and marketing strategies.
![Screenshot 2025-03-22 042125](https://github.com/user-attachments/assets/ec47cb37-b730-4ef4-a53d-3eb74d223a10)

10. Price of Apple and Google by Category:
● Why it Matters: Comparing the prices of paid apps across both the Google Play Store and Apple App Store is crucial for competitive benchmarking. By understanding how apps are priced in each store and by category, developers can adjust their pricing strategies to remain competitive. This KPI also sheds light on pricing trends within each category, helping developers identify opportunities for pricing adjustments or value propositions to attract users.
![Screenshot 2025-03-22 042135](https://github.com/user-attachments/assets/7f7470de-7b5a-43cf-b306-5e836a45dadb)

11. Sum of Price and Rating by App:

● Why it Matters: This KPI analyzes the correlation between an app’s price and its rating. Higher prices can sometimes deter users, while lower prices may attract more downloads but lead to less revenue per download. By examining this relationship,developers can adjust their pricing strategies to optimize revenue while maintaining a competitive rating. It helps to identify whether users are willing to pay a premium for a higher-quality app or if pricing should be adjusted to boost ratings.
![Screenshot 2025-03-22 042146](https://github.com/user-attachments/assets/5023b951-68c6-43ed-881e-441261500106)

12. Avg User Rating (Apple vs. Google) by Category:

● Why it Matters: Comparing user ratings for apps across both the Google Play Store andApple App Store within the same category provides insights into platform-specific userpreferences and satisfaction. It highlights potential differences in user experiences across the two major app stores, helping developers tailor their apps for specific platforms. Additionally, this comparison can help determine whether certain types of apps perform better on one platform over the other, influencing future app development and marketing decisions.

![Screenshot 2025-03-22 042157](https://github.com/user-attachments/assets/5a3055ab-3581-42cf-ba7f-66bd686250b4)
![Screenshot 2025-03-22 042205](https://github.com/user-attachments/assets/649744fe-6563-49dd-9eb9-8b4d9c711801)

4.2 Predictive Analytics

We used several predictive techniques to forecast future app performance:
● Forecasting: Time-series analysis predicted app growth rates and revenue trends for upcoming quarters.
● Regression Analysis: We assessed how factors like app ratings, sentiment, and price impact installs and revenue.
● Sentiment Analysis: Using NLP, we predicted future trends in app sentiment, helping us forecast the effect of potential changes on user satisfaction.

5. Dashboard Development

5.1 Tool Selection

The interactive dashboard was developed using Power BI, which offers powerful datavisualization, seamless integration with large datasets, and intuitive reporting features.
![Screenshot 2025-03-22 045208](https://github.com/user-attachments/assets/8d37e7e8-bdc8-4498-b969-fee41d7a0c53)

5.2 Key Features of the Dashboard
The dashboard includes the following components:
● App Performance Overview: Visualizations that display key metrics such as installs, revenue, and ratings trends.
● Predictive Insights: Interactive elements to explore forecasted app performance.
● Regression Analysis: We assessed how factors like app ratings, sentiment, and price impact installs and revenue.
![Screenshot 2025-03-22 042222](https://github.com/user-attachments/assets/4868c63b-eaeb-4ea7-87a0-c57498739783)

![Screenshot 2025-03-22 042232](https://github.com/user-attachments/assets/9a40637f-8cf1-4055-8e3f-aca424f4cd0f)

## Insights:

This means the average rating is 2.069 when the Maximum Installs for apps is equal to zero.From the model coeffiecient of – 0.0000000128 shows there is a negative relationship between Rating and Maximum Installs. An increased app rating does not really lead to a higher installation.

● Sentiment Analysis: A section that correlates user sentiment with app ratings.

● Market Comparison: A competitive benchmarking feature to compare app performance against key competitors.

5.3 Interactivity

Power BI’s interactivity allows executives to drill down into specific categories, time periods, or KPIs. This feature enables deeper exploration of trends and performance metrics, supporting dynamic decision-making.

6 Key Findings and Insights

6.1 Strategic Recommendations

● Enhance User Retention: Focus on improving features that users love, based on sentiment and reviews.

● Diversify Revenue Streams: Particularly for free apps, explore in-app purchases and advertisements as potential revenue sources.

● Strengthen Competitive Benchmarking: Continue to monitor competitors to stay ahead in terms of market share and innovation.

7. Conclusion

The development of the Advanced Business Insights Dashboard using Power BI marks a pivotal step toward enabling senior executives at Google Play Store to make data-driven, strategic decisions. By integrating various data sources—such as the Google Play Store dataset, sentiment analysis of user reviews, and market trends—into an interactive and comprehensive dashboard, we have equipped leadership with the tools necessary to gain deeper insights into app performance, user engagement, and competitive positioning.

The inclusion of 12 critical KPIs offers a robust framework to track app success and user satisfaction, while predictive analytics, including time-series forecasting, regression analysis, and sentiment prediction, allows executives to anticipate market trends and future app performance. This foresight is invaluable for proactively addressing challenges and seizing opportunities for growth.

With a user-friendly Power BI dashboard, decision-makers now have access to dynamic and customizable reports, allowing them to drill down into key metrics and explore performance across categories, timeframes, and app types. The ability to interact with the data enhances the decision-making process, ensuring that insights are tailored to the specific needs of the business.

## Strategic recommendations such as ;
- Enhancing user retention,
- Diversifying revenue streams and
- Strengthening competitive benchmarking are derived from the dashboard's findings.
These actions, informed by real-time data, will help the Google Play Store maintain its leadership in the highly competitive mobile app market and foster sustainable growth moving forward.

## Conclusion 
The Advanced Business Insights Dashboard serves as a vital tool for empowering the leadership team at Google Play Store with actionable insights, enabling them to drive better business outcomes, optimize app performance, and adapt to ever-changing market dynamics. The dashboard’s comprehensive analytics, combined with predictive insights, positions the Google Play Store to remain at the forefront of the mobile app ecosystem.

