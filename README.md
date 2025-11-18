# bike-store-customer-segmentation
Understanding your customers is one of the most valuable things a business can do, especially in retail where buying behavior varies a lot from person to person. This project focuses on an Australian bike store that has a mix of casual riders, regular customers, and high-spending loyal buyers. Instead of treating all customers the same, the goal was to group them into meaningful segments so the business can communicate more effectively, design better promotions, and focus on the right people at the right time.

The store already collects useful data — transaction history, demographics, address details, and purchase patterns — but these raw tables don’t tell a clear story on their own. To make the data usable, I combined everything into a single customer-level dataset, cleaned inconsistent fields, added new features like recency and tenure, and then applied machine learning to uncover natural groupings.

The end result is a practical segmentation model that highlights who spends the most, who is at risk of dropping off, and which customers might become more valuable with the right marketing support. These insights can help the store improve retention, personalize recommendations, and make smarter decisions on how to allocate marketing effort and budget.

## Project Overview 
The project moves through a full end-to-end analytics pipeline: SQL → Python → Tableau.

I take customer data from several sources and turns it into actionable segmentation that the store can use right away. The dataset includes four main components:

- Transactions: purchase amounts, product info, and dates
- Customer Demographics: gender, age, wealth segment, job industry
- Address Information: state, country, and property valuation
- New Customer List: details about recent sign-ups

These tables were cleaned and merged using SQL, then processed further in Python. I engineered several features that help describe each customer’s shopping behavior, such as:

- total dollars spent
- number of purchases
- days since last purchase
- how long they’ve been a customer
- number of bike-related purchases in the past 3 years

After preparing the data, I used K-Means clustering to find groups of customers with similar behaviors. To choose the number of clusters, I compared the Elbow Curve and Silhouette Scores, which both pointed to three main segments.

Once the model was trained, I used PCA to visualize the clusters and exported everything to Tableau, where I built a dashboard showing each segment’s size, spending patterns, demographics, geographic breakdown, and more.

The final result is a clear breakdown of three customer types:
- High-value buyers who shop often
- Mid-value, steady customers
- At-risk or low-engagement customers

This segmentation can help the store prioritize the people who matter most while also identifying customers who may need re-engagement strategies. Overall, the project demonstrates a full machine-learning workflow built to solve a real business problem in retail analytics.


