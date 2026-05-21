# 🛍️ Customer Shopping Behavior Analysis
## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data (~3,900 records) across multiple product categories. The goal is to uncover insights into customer spending patterns, product preferences, and subscription trends to support data-driven business decisions.
------
## 📊 Dataset Summary
* Total Records: 3,900
* Features: 18 columns

### Key Data Includes:
* Customer Information: Age, Gender, Location, Subscription Status
* Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color
* Behavioral Data: Discount Usage, Purchase Frequency, Previous Purchases, Review Ratings, Shipping Type

* ⚠️ Missing values: 37 entries in Review Rating column (handled during preprocessing)
----

## 🧹 Data Cleaning & Preparation (Python)
### Performed using Pandas:
* Loaded and explored data using df.info() and describe()
* Handled missing values using median imputation by category
* Renamed columns to snake_case for consistency
* Removed redundant column (promo_code_used)

### 🔧 Feature Engineering:
* Created age_group for customer segmentation
* Derived purchase_frequency_days for behavioral analysis
* Final cleaned dataset stored in PostgreSQL for further querying

---

## 🗄️ Data Analysis (SQL)
#### Used PostgreSQL to answer key business questions:
### Key Analyses:
* 💰 Revenue comparison by gender
* 🛒 High-spending customers using discounts
* ⭐ Top-rated products
* 🚚 Impact of shipping type on spending
* 👥 Subscriber vs non-subscriber behavior
* 🏷️ Discount-heavy products
* 🔁 Customer segmentation (New, Returning, Loyal)
* 🏆 Top 3 products per category
* 📈 Repeat buyers vs subscription trends
* 👶 Revenue contribution by age group
### 📌 Sample Insights:
* Male customers generated higher total revenue �
Customer Shopping Behavior Analysis.pdf
* Express shipping users had slightly higher average purchase value (page 4) �
Customer Shopping Behavior Analysis.pdf
* Young adults contributed the highest revenue among all age groups (page 7) �
Customer Shopping Behavior Analysis.pdf
* Products like hats and sneakers showed high dependency on discounts (page 5) �
Customer Shopping Behavior Analysis.pdf
## 📊 Dashboard (Power BI)
An interactive dashboard was built to visualize insights:
### Key Metrics:
* Total Customers
* Average Purchase Amount
* Average Review Rating
### Visualizations:
* Revenue by Category
* Sales by Age Group
* Subscription Distribution
* Customer Segmentation
## 💡 Business Recommendations
* 🎯 Promote subscriptions with exclusive benefits
* 🔁 Strengthen loyalty programs for repeat customers
* 💰 Optimize discount strategies to protect margins
* 🛍️ Highlight top-performing and highly rated products
* 📍 Target high-value segments like young adults and frequent buyers
## 🛠️ Tech Stack
* Python (Pandas) – Data cleaning & preprocessing
* PostgreSQL – Data analysis
* Power BI – Data visualization & dashboarding
## 🚀 How to Run This Project
* Load dataset into Python (Pandas)
* Perform data cleaning & feature engineering
* Push cleaned data to PostgreSQL
* Run SQL queries for analysis
* Connect Power BI to PostgreSQL for dashboard
