# Retail Sales & Profitability Dashboard | Power BI

## Project Overview

This project presents an interactive Power BI dashboard developed to analyse retail sales performance, profitability, customer behaviour and product performance using the Superstore dataset.

The dashboard is designed to support business decision-making by transforming transactional sales data into clear KPIs, trends and actionable insights.

## Business Questions

The analysis focuses on answering the following questions:

- How are overall sales and profitability performing?
- How have sales changed over time?
- Which regions and product categories generate the highest sales?
- Which sub-categories contribute most to profit and which generate losses?
- Who are the highest-value customers?
- Which products generate the highest sales?
- How are sales distributed across customer segments?
- How does discounting relate to profitability?

## Dashboard Pages

### 1. Retail Sales & Profitability Dashboard

![Retail Sales & Profitability Dashboard](Retail%20Sales%20and%20Profitability%20Dashboard.png)

Provides an executive overview of business performance, including:

- Total Sales: **$2.33M**
- Total Profit: **$292.30K**
- Profit Margin: **12.6%**
- Total Orders: **5K**
- Average Order Value: **$455.20**
- Monthly sales trends
- Regional sales performance
- Profitability by sub-category
- Sales and profit comparison by category

### 2. Product & Customer Analysis

![Product & Customer Analysis](Product%20and%20Customer%20Analysis.png)

Provides deeper analysis of customers and products, including:

- **804** unique customers
- Approximately **2K** products sold
- **39K** units sold
- Top 10 customers by sales
- Top 10 products by sales
- Sales by customer segment
- Profit margin by category
- Discount impact on profitability

## Key Insights
- Total sales reached **$2.33M**, generating approximately **$292.3K in profit** at a **12.6% profit margin**.
- Sales show an overall upward trend across the reporting period.
- The **West** region generates the highest sales.
- **Technology** is a major contributor to overall business performance.
- **Copiers and Phones** are among the strongest profit-generating sub-categories.
- **Tables and Bookcases** generate losses and may require pricing, discount or cost review.
- The Consumer segment accounts for approximately **50% of total sales**.
- Discount analysis highlights products where higher discount levels coincide with weak or negative profitability.

## Power BI Features Used
- Power Query data preparation
- DAX measures
- KPI cards
- Slicers and synchronized slicers
- Top N filtering
- Cross-filtering and interactive visuals
- Line, bar, column, donut, combo and scatter charts
- Conditional visual formatting
- Custom tooltips
- Multi-page dashboard design

## DAX Measures
Key measures created for the analysis include:

```DAX
Total Sales = SUM(Orders[Sales])

Total Profit = SUM(Orders[Profit])

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)

Total Orders = DISTINCTCOUNT(Orders[Order ID])

Total Quantity = SUM(Orders[Quantity])

Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Unique Customers = DISTINCTCOUNT(Orders[Customer ID])

Products Sold = DISTINCTCOUNT(Orders[Product ID])
```

## Tools
- Microsoft Power BI Desktop
- Power Query
- DAX
- GitHub

## Interactive Filters
Both dashboard pages include synchronized filters for:

**Year | Region | Category**
These allow users to explore performance across different periods, geographical regions and product categories.

## Project File
The complete Power BI report is available in this repository:

`Retail_Sales_Performance_Dashboard.pbix`

## Author
**Swathi Murali**

MSc Business Analytics  