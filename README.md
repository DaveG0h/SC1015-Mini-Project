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
-- U

- Use order_date_time to add Order_made
- Made use of Order_made and order id to remove any row that has NULL order ID and ordermade = 0
- Added remarks_length to measure the length of customer remarks
- Remove the column of customer city as no relation to CSAT score
- Remove the column of "connected_handling_time" as majority are NULL values
- Added and cleaned response_time = issue_responded - issue_reported
- Split the datset into 3 categories: 1. both 2. with order made 3. without order made
### 3. [Exploratory Data Analysis (EDA)](edatest.ipynb)
add description
### 4. [Machine Learning](mltest.ipynb)
add description
### 5. Data Driven Insights & Conclusion
### 6. References 
- https://www.kaggle.com/datasets/ddosad/ecommerce-customer-service-satisfaction/data
- https://www.superoffice.com/blog/customer-experience-statistics/


