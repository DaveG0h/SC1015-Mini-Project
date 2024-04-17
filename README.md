# SC1015-Mini-Project - eCommerce Customer Service Satisfaction
Lab : FDAB\
Group : 5

Members 
--
1. CHUA JIA HON
2. LIM YU CHENG, BRYAN
3. DAVE GOH YU LONG

Description
--
The primary objective of this notebook is to analyze the CSAT trends and patterns within an e-commerce dataset. Specifically, we aim to:
- Analyze CSAT trends and patterns in e-commerce data.
- Visualize relationships between factors and CSAT scores.
- Analyze scores across agents, supervisors, categories, etc.
- Explore CSAT score trends for recurring patterns.
- Identify factors influencing CSAT scores.
- Provide recommendations to enhance customer satisfaction.

Relevancy
--
[link](https://www.superoffice.com/blog/customer-experience-statistics/) “In their future of CX report, PwC surveyed 15,000 consumers and found that 1 in 3 customers will leave a brand they love after just one bad experience, while 92% would completely abandon a company after two or three negative interactions.”


Content
--
### 1. Problem Formulation
Dataset : https://www.kaggle.com/datasets/ddosad/ecommerce-customer-service-satisfaction/data \
Our Question : How do we improve customer service in e-commerce websites in order to improve reputability and thus profit?

### 2. [Data Cleaning](cleantest.ipynb)
- Added "Order_made" based on value of "order_date_time"
- Used new "Order_made" and "order id" to remove and row that NULL order ID and "Order_made" = 0
- Remove the columns of "Customer_City" as no relation to CSAT
- Remove the column of "connected_handling_time" as majority are NULL
- Added and cleaned response_time_minutes = issue_responded - issue_reported
- Added "remarks_length" to get the length of customer remarks, for later use in EDA/ML
- Split the dataset into 3 categories 1. both with/without order made 2. with order made 3. without order made

### 3. [Exploratory Data Analysis (EDA)](edatest.ipynb)
From the data cleaning portion, this will be the categories that we will be using for EDA \
Categorical nominal attributes : "channel_name", "category", "Sub-category", "Agent shift"\
Categorical ordinal attributes : "Tenure Bucket"\
Numerical continuous attributes : "remarks_length", "response_time_minutes", "Item_price"\
Response variable : CSAT Score\

- Utilise the variables and visualise trends against the CSAT score
- Use LabelEncoder on categorical attribute
- Use SelectKBest to measure correlation with the response variable

### 4. [Machine Learning](mltest.ipynb)
- Clean and use "Customer Remarks" for sentiment analysis instead of "remarks_length"
- Used classification tree to determine the relevant categories with relation to the response variable


### 5. Data Driven Insights & Conclusion

### 6. References 
- https://www.kaggle.com/datasets/ddosad/ecommerce-customer-service-satisfaction/data
- https://www.superoffice.com/blog/customer-experience-statistics/


