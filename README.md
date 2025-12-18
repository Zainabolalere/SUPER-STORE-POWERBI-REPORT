# SUPER-STORE-POWERBI-REPORT
Power BI report with custom DAX measures and 4 interactive dashboards analyzing sales, customers, regions, and profitability for retail operations.


## TABLE OF CONTENTS
- [Description](#description)
- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Tools](#tools)
- [Data Preparation](#data-preparation)
- [Dataset](#dataset)
- [Dashboard](#dashboard)
- [Insights](#insights)
- [Recommendations](#recommendations)
- [Contact](#contact)

## Description
This project leverages Power BI to analyze retail operations for a Super Store, providing actionable insights into sales performance, regional efficiency, customer behavior, and product profitability.

**Developed as part of the DSN AI+ Microsoft-supported Power BI Associate training program.**

## Overview
The dataset contains 5,009 orders generating $2.3M in revenue across 793 customers, covering sales transactions, product categories, customer segments, regional performance, and profitability metrics.

The report provides an interactive view of business performance with filters for Year, Region, and Category across 4 comprehensive dashboard pages.

## Problem Statement
The business lacks clear visibility into which products are profitable, which regions are underperforming, and how customer segments contribute to the bottom line. Without data-driven insights, it's difficult to identify loss-making products, optimize regional strategies, and maximize customer lifetime value. A comprehensive analytical report is required to drive strategic decision-making.

## Objectives

1️⃣ Track total revenue, profit, orders, and customer metrics across all operations.

2️⃣ Identify profitable vs. loss-making product categories and subcategories.

3️⃣ Compare regional performance and uncover growth opportunities.

4️⃣ Analyze customer loyalty, segmentation, and purchasing behavior.

5️⃣ Provide data-driven recommendations to optimize profitability and growth.

## Tools
**Power Query** → For data transformation and preparation

**Power BI** → For data modeling, DAX measures, and visualization

**DAX** → For custom calculations (profit margin, customer metrics, order analysis)

## Data Preparation
The following data preparation steps were performed:

✅ Promoted first row as headers in Power Query

✅ Verified and corrected data types for all columns (dates, numbers, text, decimals)

✅ Built star schema data model connecting 6 normalized tables (Orders, Customers, Locations, States, Products, Product Pricing Tiers)

✅ Established proper table relationships (one-to-many)

✅ Created 6 custom DAX measures for key business metrics

## Dataset
The dataset used for this project includes:

- **Orders Table:** Transaction details (Order ID, sales, profit, discount, quantity)
- **Customers Table:** Customer information (Customer ID, name, segment)
- **Locations Table:** Geographic data (City, state, postal code)
- **States Table:** Regional assignments (State, region)
- **Products Table:** Product metadata (Product ID, category, subcategory)
- **Product Pricing Tiers Table:** Segment-based pricing per product

**Total Records:** 5,009 orders | 793 customers | 49 states

## Dashboard

### 1. Sales & Performance Overview
![Sales & Performance Overview](Sales%20&%20Performance%20Insights.png)

### 2. Customer Insights
![Customer Insights](Customer%20Insights.png)

### 3. Regional & States Insights
![Regional & States Insights](Regional%20and%20States%20Insights.png)

### 4. Profitability Analysis
![Profitability Analysis](Profitability%20analysis.png)

## Insights

### 1️⃣ Overall Performance

The business generated **$2.3M in total revenue** with **$286.4K in profit** across 5,009 orders, averaging a **12.47% profit margin**.

This shows solid revenue generation, but profitability needs optimization.

### 2️⃣ Critical Finding: Loss-Making Products

**Bookcases** (-3% margin) and **Tables** (-9% margin) are operating at a loss.

Despite contributing to top-line revenue, these categories drain profits on every sale, costing the business approximately **$15K-20K annually**.

### 3️⃣ Regional Performance Gap

**West** region leads with **$725.5K in sales**, outperforming **South** ($391.7K) by **85%**.

Both **West and East** regions achieve **$67.30 profit per order**, while **Central** lags at **$33.8** per order.

The South and Central regions represent **$334K in untapped potential** if they match top-performing regions.

### 4️⃣ Exceptional Customer Loyalty

**98.49% of customers are repeat buyers**, with only 12 one-time customers out of 793 total.

Average sales per customer is **$2.9K**, with the top customer generating **$25K+**.

This exceptional retention rate indicates strong product-market fit and customer satisfaction.

### 5️⃣ Customer Segment Distribution

**Consumer segment** dominates with **50.6%** of customers and contributes **$134.1K in profit**.

**Corporate** (30.4%) and **Home Office** (19%) segments remain underutilized, representing B2B growth opportunities.

### 6️⃣ Category Profitability

**Technology** drives **$145.5K in profit** with strong margins.

**Labels** (44%) and **Paper** (43%) show the highest profit margins.

Meanwhile, **Furniture** category contains the loss-making products dragging down overall profitability.

### 7️⃣ Seasonal Trends

**November and December** consistently show peak performance, indicating strong Q4 seasonality.

This provides a clear opportunity for targeted Q4 inventory and marketing optimization.

## Recommendations

### 1️⃣ Fix Loss-Making Products Immediately

Conduct pricing analysis on **Bookcases and Tables**—either increase prices, reduce supplier costs, or phase out unprofitable SKUs.

**Impact:** Recover **$15K-20K annually** in losses.

### 2️⃣ Replicate Top Regional Strategies

Analyze what drives **West and East** success ($67.30 profit per order) and apply those strategies (logistics, pricing, product mix) to **Central and South** regions.

**Impact:** Unlock **$334K** in untapped regional potential.

### 3️⃣ Leverage Customer Loyalty

With **98.49% repeat rate**, launch a loyalty rewards program targeting high-value customers. Even a **5% increase** in average customer spend could be achieved through strategic upselling.

**Impact:** Generate **$115K** in additional revenue.

### 4️⃣ Expand B2B Market Share

Develop targeted campaigns for **Corporate and Home Office** segments, which are currently underutilized. Consider enterprise pricing and bulk purchase incentives.

**Impact:** Capture untapped B2B market share in profitable Technology category.

### 5️⃣ Optimize for Q4 Seasonality

Front-load inventory procurement and increase marketing budget allocation for **November-December** to maximize high-season returns.

**Impact:** Maximize revenue during peak selling period.

---


## DAX Measures Created
```dax
Total Sales = SUM(Orders[Sales])

Total Profit = SUM(Orders[Profit])

Order Count = DISTINCTCOUNT(Orders[Order ID])

Average Discount = AVERAGE(Orders[Discount])

Customer Count = DISTINCTCOUNT(Customers[Customer ID])

Profit Margin = DIVIDE([Total Profit], [Total Sales])
```


## Contact

Created by **Zainab Olalere**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/zainab-olalere-6424091a4/)

![Thank you](Thank%20you.png)



