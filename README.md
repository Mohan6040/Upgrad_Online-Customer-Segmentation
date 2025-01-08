# Customer Segmentation Using RFM Model

## Introduction

Businesses across the globe are expanding rapidly, driven by technological advancements that open up broader markets and increase customer reach. One of the most effective ways businesses can increase their revenue and improve customer service is through customer segmentation. Customer segmentation refers to the process of categorizing customers into distinct groups based on shared characteristics, behaviors, or needs. By identifying different customer segments, businesses can personalize their offerings, enhance customer experience, and improve marketing strategies.

This project aims to identify major customer segments within a transactional dataset for a UK-based online retailer that specializes in unique gifts for all occasions. This will enable the business to optimize their marketing efforts and target specific groups effectively.

---

## Problem Description

The objective of this project is to analyze a transactional dataset containing all transactions that occurred between December 1, 2010, and December 9, 2011, for a UK-based non-store online retail business. This company primarily sells unique, all-occasion gifts and has a wide range of customers, including individual consumers and wholesale buyers.

The dataset includes the details of each transaction, including customer information and the purchased products. Using this dataset, the goal is to identify key customer segments based on their purchasing behavior, which can help in targeting the right audience for marketing campaigns, optimizing product offerings, and improving customer retention.

---

## The Need for Customer Segmentation

Different customer groups exhibit variations in behaviors, demographics, geographical locations, and preferences. These differences can be harnessed for effective marketing strategies and decision-making. Segmenting customers allows businesses to focus on distinct groups with tailored strategies, maximizing customer value and business outcomes. Identifying customer segments can benefit the business in several ways:

1. **Targeted Marketing**: 
   - Businesses can create personalized campaigns for each customer segment based on their purchasing behavior and preferences, leading to higher engagement and conversion rates.

2. **Client Understanding**: 
   - Gaining insights into different customer types helps businesses understand their needs, which can enhance service quality, improve product offerings, and drive better customer satisfaction.

3. **Optimal Product Placement**: 
   - Identifying which segments are most interested in specific products allows businesses to place products strategically, reducing marketing costs and increasing sales.

4. **Revenue Growth**: 
   - Tailoring services and promotions to specific segments ensures that businesses can engage with customers in a way that increases their loyalty and lifetime value.

---

## Recency-Frequency-Monetary (RFM) Model to Determine Customer Value

The **Recency-Frequency-Monetary (RFM) Model** is a well-established method used in retail customer segmentation. It uses three key dimensions to assess the value of customers based on their past transaction history:

1. **Recency**: 
   - How recently did the customer make a purchase? More recent purchases indicate a higher likelihood of future purchases.
   
2. **Frequency**: 
   - How often does the customer make purchases? A higher frequency suggests a loyal customer who repeatedly engages with the business.
   
3. **Monetary Value**: 
   - How much money does the customer spend on average? High monetary value indicates a customer who contributes significantly to the business's revenue.

By combining these three dimensions, businesses can assign a quantitative score to each customer. For example, a customer who frequently buys high-value products and makes recent purchases is considered a high-value customer and should be prioritized in marketing campaigns.

---

## Approach Taken

The following steps were taken to prepare the data and create the customer segmentation model:

1. **Data Inspection**: 
   - The dataset was thoroughly inspected for completeness and accuracy. Basic checks like reviewing the dataset structure, column names, and sample records were done.

2. **Exploratory Data Analysis (EDA)**: 
   - Various techniques were applied to identify patterns, trends, and anomalies in the dataset. This includes generating statistical summaries, visualizing distributions, and identifying outliers.
   - Identified and handled missing values, duplicate entries, and inconsistencies in the dataset.

3. **Data Preparation**: 
   - Cleaned and preprocessed the data by handling missing values, removing duplicate entries, and transforming data into a suitable format for modeling.
   - Also, handled the necessary data types and encoded categorical variables to ensure proper processing.

4. **Create RFM Model**: 
   - The RFM model was built by computing the Recency, Frequency, and Monetary values for each customer based on their transaction history. These values were then normalized and scaled for consistency.

5. **Clustering Models Implementation**: 
   - Using the RFM scores, customer data was segmented using clustering algorithms like K-means, which allowed us to group customers into meaningful clusters based on their purchasing behavior.

6. **Model Validation**: 
   - The results of the clustering were analyzed to evaluate the quality and effectiveness of the customer segments. Methods like the elbow method were used to identify the optimal number of clusters.
   
---

## Conclusions

### Descriptive Analysis

- **Missing and Duplicate Values**: 
  - Some missing and duplicate entries were identified and addressed. These were handled by either filling the missing values with appropriate defaults or removing duplicates to ensure accuracy.

- **Geography**: 
  - The majority of the customers are from the United Kingdom, with smaller segments from other countries. This suggests a strong local customer base, which could be useful for targeted regional promotions.

- **Purchase Days**: 
  - Peak purchase days were Thursday, Wednesday, and Tuesday, suggesting these are the most active days for customers. This information can help in planning marketing campaigns and optimizing website traffic on these days.

- **Purchase Months**: 
  - Most purchases occurred in November, October, and December, with fewer purchases in January, February, and April. This pattern could be related to holiday shopping and year-end sales.

- **Purchase Time**: 
  - Customers predominantly made purchases in the afternoon, indicating a potential peak in browsing behavior during these hours.

Using the RFM model, customers were grouped into various segments based on their RFM scores. The application of clustering algorithms, including K-means, revealed that the optimal number of customer segments is **3**.

### Business Implications

- **Targeted Campaigns**: Based on the segmentation, the business can now develop specific marketing strategies for each of the three customer segments. For example, high-value customers can be targeted with loyalty rewards, while low-value customers can be encouraged to make more frequent purchases.
  
- **Improved Customer Retention**: The segmentation helps identify at-risk customers who have not purchased recently. Retargeting these customers with personalized offers could help retain them.

- **Revenue Optimization**: By aligning product placement and promotional efforts with the needs of specific segments, the business can maximize its sales and profitability.

By focusing on these distinct customer clusters, the company can improve customer satisfaction, increase retention, and enhance overall business performance.
