# AI-ML-INTERNSHIP
# E-Commerce Customer Behavior & Delivery Analytics
A foundational data analytics project focused on understanding e-commerce customer behavior, delivery performance, return patterns, discount impact, and revenue using Python, NumPy, Pandas, and Matplotlib.

##  Project Overview

SwiftKart is a high-growth multi-category e-commerce platform operating across Tier 1, Tier 2, and Tier 3 Indian markets.

Although the platform's Gross Merchandise Value (GMV) has increased, operating margins have been affected by three major challenges:

- Increasing product return rates
- Delivery and logistics delays
- Heavy dependence on discounts

This project analyzes transactional e-commerce data to identify operational bottlenecks, customer behavior patterns, and revenue-impacting factors.

---
##  Objectives

The main objectives of this project are:

- Clean and validate raw e-commerce transaction data
- Handle duplicate records and missing values
- Standardize inconsistent categorical data
- Calculate delivery delays
- Classify fulfillment performance
- Calculate net realized revenue after discounts
- Analyze category-wise revenue and return rates
- Compare logistics performance across city tiers
- Analyze the relationship between delivery delays and customer ratings
- Segment customers using rule-based business logic
- Create meaningful visualizations for business decision-making

---
##  Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

##  Dataset

The project uses an e-commerce transactional dataset named:

`ecommerce_orders.csv`

The dataset contains information about:

- Order ID
- Customer ID
- Product Category
- Payment Method
- Order Value
- Discount Percentage
- Estimated Delivery Days
- Actual Delivery Days
- Customer Rating
- Return Status
- City Tier

The original dataset contains 1,000 baseline records, with additional duplicate records and missing values intentionally introduced to simulate real-world data quality problems.

##  Data Cleaning

The following data-cleaning operations were performed:

### 1. Data Inspection
- Checked dataset dimensions using `df.shape`
- Checked data types using `df.dtypes`
- Identified missing values using `df.isnull().sum()`

### 2. Duplicate Removal
Duplicate orders were identified using `Order_ID` and removed while keeping the first occurrence.

### 3. Payment Method Standardization
Inconsistent values such as:

`upi`

were standardized to:

`UPI`

Whitespace and casing inconsistencies were also handled.

### 4. Missing Order Value Imputation

Missing `Order_Value` values were filled using the median order value of their respective product category.

### 5. Customer Rating Handling

Missing customer ratings were handled using an appropriate analytical strategy and documented with justification.

##  Feature Engineering

Several new analytical features were created.

### Delivery Delay

```text
Delivery_Delay = Actual_Delivery_Days - Est_Delivery_Days[ecommerce_customer_behavior_and_delivery_analytics.pdf](https://github.com/user-attachments/files/32430342/ecommerce_customer_behavior_and_delivery_analytics.pdf)


[Uploading Ecommerce_Cleaned_Data.csv…]()
[Ecommerce_Cleaned_Data.csv](https://github.com/singh484/AI-ML-INTERNSHIP/blob/main/Ecommerce_Cleaned_Data.csv)

[code.ipynb](https://github.com/user-attachments/files/32430998/code.ipynb)




