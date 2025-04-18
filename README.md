# Customer-Segmentation-in-E-commerce
Customer Segmentation in E-commerce: Identify customer clusters based on purchasing
This project focuses on customer segmentation using RFM (Recency, Frequency, Monetary) analysis followed by K-Means clustering. The dataset was first uploaded and cleaned by removing entries with missing CustomerID values and calculating the total spending per transaction. A reference snapshot date was selected to compute RFM metrics for each customer: Recency (days since last purchase), Frequency (number of transactions), and Monetary (total spending). These features were then standardized using a scaler to prepare them for clustering. The Elbow Method was used to identify the optimal number of customer segments, which was determined to be 4 based on the WCSS (Within-Cluster Sum of Squares) plot. Using K-Means clustering with k=4, customers were grouped into distinct clusters. Visualization through pair plots helped interpret the segmentation, revealing different patterns in purchasing behavior such as high-value loyal customers, frequent but low spenders, recent shoppers, and dormant users. This segmentation can be used for targeted marketing strategies, personalized communication, and better customer retention planning.

🔍 Results
After applying K-Means clustering with k=4, the customers were grouped into the following distinct segments based on their RFM scores:

Cluster 0 – The Lost Customers
High Recency, Low Frequency, Low Monetary

These customers haven’t shopped in a long time and didn’t make many purchases even when they did.

Business Strategy: Reactivation campaigns such as win-back offers, email reminders, or personalized discounts may help re-engage this group.

Cluster 1 – The Loyal Champions
Low Recency, High Frequency, High Monetary

This is the most valuable segment. These customers buy frequently, spend a lot, and have shopped recently.

Business Strategy: Focus on retention and reward strategies. Offer loyalty programs, exclusive previews, and VIP benefits to maintain their loyalty.

Cluster 2 – The At-Risk Customers
Very High Recency, Moderate Frequency, Moderate Monetary

These customers used to shop but haven’t returned recently. They spent a reasonable amount in the past.

Business Strategy: Send personalized "We miss you" messages, limited-time offers, or surveys to understand why they stopped engaging.

Cluster 3 – The Potential Loyalists
Low Recency, Moderate Frequency, Moderate Monetary

These are recent shoppers who buy occasionally. With the right nurturing, they could be converted into loyal customers.

Business Strategy: Promote related products, offer incentives for increased purchases, or guide them into a loyalty program.

Cluster | Recency | Frequency | Monetary | Segment Name | Description | Recommended Strategy
0 | High | Low | Low | Lost Customers | Inactive customers who haven’t purchased recently and didn’t spend much | Reactivation emails, special discounts, retargeting ads
1 | Low | High | High | Loyal Champions | Most valuable segment — frequent, high-spending, recent buyers | Loyalty rewards, VIP programs, early access to products
2 | Very High | Moderate | Moderate | At-Risk Customers | Previously active, but haven’t purchased in a long time | “We miss you” campaigns, personalized offers, feedback surveys
3 | Low | Moderate | Moderate | Potential Loyalists | Recently active with potential to become loyal | Product recommendations, loyalty programs, incentives for increased frequency
