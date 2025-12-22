# Customer-Shopping-Behavior-Analysis
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to support strategic, data-driven business decisions.

The project covers the complete analytics lifecycle: data loading and cleaning in Python, business analysis using SQL, visualization with Power BI, and insight communication.

#### Power BI Dashboard Screenshot

![Power BI Dashboard]([power_bi_dashboard.png](https://github.com/abhay01pandey/Customer-Shopping-Behavior-Analysis/blob/333963aa5746e71627952fbd40206e5d85c78d45/power_bi_dashboard.png))

---

## Dataset

### Dataset Summary
- *Rows:* 3,900  
- *Columns:* 18  

### Key Features
- *Customer Demographics:* Age, Gender, Location, Subscription Status  
- *Purchase Details:* Item Purchased, Category, Purchase Amount, Season, Size, Color  
- *Shopping Behavior:* Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type  

### Data Quality
- *Missing Data:* 37 missing values in the review_rating column  
- *Handling:* Missing values were imputed using the *median rating of each product category*

---

## Tools & Technologies
- *Python:* Pandas, NumPy (EDA, data cleaning, feature engineering)  
- *SQL:* MySQL (business analysis queries)  
- *Power BI:* Interactive dashboard  
- *Jupyter Notebook:* Development environment  

---

## Project Steps

### 1. Exploratory Data Analysis & Data Cleaning (Python)
- Loaded the dataset using Pandas  
- Performed initial exploration using df.info() and df.describe()  
- Identified and handled missing values in review_rating  
- Standardized column names to snake_case for consistency  
- Feature engineering:
  - Created age_group by binning customer ages  
  - Created purchase_frequency_days  
- Checked data consistency between discount_applied and promo_code_used  
- Dropped redundant promo_code_used column  
- Loaded the cleaned dataset into MySQL for SQL analysis  

---

### 2. Data Analysis (SQL – Business Transactions)
Structured SQL queries were used to answer key business questions:

- Revenue comparison by gender  
- Identification of high spending customers who used discounts  
- Top 5 products by average review rating  
- Comparison of average purchase amount by shipping type  
- Subscriber vs non subscriber revenue and spending analysis  
- Products most dependent on discounts  
- Customer segmentation into New, Returning and Loyal groups  
- Top 3 products within each category  
- Subscription likelihood among repeat buyers  
- Revenue contribution by age group  

---

## Project Dashboard

### Dashboard Overview
An interactive dashboard was built to present insights clearly for business stakeholders and decision makers.

#### Power BI
- Revenue trends and customer segmentation  
- Product and category performance  
- Subscription and discount behavior  
- Impact of shipping type on spending  
- Filters for category, gender, subscription status, and age group  

---

## Results & Insights
- Subscribers generate higher average spend than non subscribers  
- Loyal customers contribute a significant share of total revenue  
- Certain products rely heavily on discounts to drive sales  
- Express shipping users tend to have higher purchase values  
- Specific age groups contribute the majority of revenue  

---

## Business Recommendations
- *Boost Subscriptions:* Promote exclusive benefits for subscribers  
- *Customer Loyalty Programs:* Reward repeat buyers to move them into the “Loyal” segment  
- *Review Discount Policy:* Balance sales growth with margin control  
- *Product Positioning:* Highlight top rated and best selling products  
- *Targeted Marketing:* Focus efforts on high revenue age groups and express shipping users  

---

## How to Run the Project
1. Clone the repository  
2. Install required Python libraries  
3.   pip install pandas numpy
4. Run the Jupyter notebook for EDA and data cleaning
5. Load the cleaned dataset into MySQL
6. Execute SQL queries for analysis
7. Open the Power BI dashboard
