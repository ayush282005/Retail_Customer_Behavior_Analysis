# 🛍️ Retail Customer Behavior Analysis

## End-to-end Data Analytics Portfolio Project | Python • PostgreSQL/SQL • Power BI • DAX
# 📌 Project Overview

This project analyzes retail customer shopping behavior to understand
**sales performance, customer engagement, product performance, and purchasing patterns.**

The workflow follows a complete analytics pipeline:

**Raw Data → Python Data Cleaning & Feature Engineering → PostgreSQL →
SQL Business Analysis → Power BI & DAX → Interactive Dashboard →
Business Insights**

The goal is not only to report what happened, but to identify
**actionable business insights** that can support decisions around
products, customers, subscriptions, discounts, and sales performance.

# Dataset Summary - 
- Rows: 3,900
- Columns: 18
-  Key Features:
   -  Customer demographics (Age, Gender, Location, Subscription Status)
   -   Purchase details (Item Purchased, Category, Purchase Amount, Season, Size, Color)
   -    Shopping behavior (Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type) 

# 🎯 Business Objectives

This analysis focuses on questions such as:

-Which categories generate the most revenue and sales volume?<br>
-Which products are driving the highest revenue?<br>
-Which customer age group has the highest average purchase value?<br>
-Do subscribed customers spend more?<br>
-Which products have both high sales volume and high customer
ratings?<br>
-How does discount usage relate to customer spending?<br>
-Which customer segments contribute most to revenue?<br>
-What purchasing and payment behaviors can help improve customer
engagement?<br>

# 🧰 Tools & Technologies

| Area | Tools |
|-------|----------|
 |Data Cleaning | Python, Pandas|
 |Database | PostgreSQL|
| Data Analysis | SQL |
| Business Intelligence | Power BI |
| Calculations | DAX |
| Visualization |Power BI |

# 🐍 1.Exploratory Data Analysis using Python 

We began with data preparation and cleaning in Python:

  - **Data Loading:** Imported the dataset using pandas.
    
  - **Initial Exploration:** Used df.info() to check structure and .describe() for 
summary statistics.

- **Missing Data Handling:** Checked for null values and imputed missing values in the 
Review Rating column using the median rating of each product category.
 
- **Column Standardization:** Renamed columns to snake case for better readability and 
documentation.

- **Feature Engineering:**
   ○ Created age_group column by binning customer ages. 
   ○ Created purchase_frequency_days column from purchase data.
  
- **Data Consistency Check:** Verified if discount_applied and promo_code_used 
were redundant; dropped promo_code_used.

- **Database Integration:** Connected Python script to PostgreSQL and loaded the cleaned 
DataFrame into the database for SQL analysis.

# 🗄️ 2. SQL Business Analysis

After cleaning, the data was analyzed in PostgreSQL using SQL.

The analysis included:

- Aggregations
- GROUP BY
- HAVING
- Subqueries
- CASE WHEN
- CTEs
- Window functions
- Ranking
- Customer segmentation
- Product performance analysis


# 📊 3. Power BI Dashboard

The cleaned and analyzed data was brought into Power BI to create an
interactive **Retail Customer Behavior Dashboard.**

**Dashboard KPIs**

The dashboard highlights four key metrics:

**👥 Number of Customers**

Approximately **3.9K**

**💰 Total Revenue**

Approximately **$233K**

**🛒 Average Purchase Amount**

**$59.76**

**⭐ Average Review Rating**

**3.75**

The dashboard also provides interactive slicers for:

- Subscription Status
- Gender
- Category
- Shipping Type

