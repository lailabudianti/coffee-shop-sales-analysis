# Coffee Shop Sales Analysis Dashboard

An end-to-end sales analytics project using **MySQL, Microsoft Power BI, Power Query, DAX, and Microsoft Excel** to analyze coffee shop sales performance, monitor business KPIs, and identify operational patterns from transactional data.

## 1. Project Overview

The **Coffee Shop Sales Analysis Dashboard** is a Business Intelligence project designed to help coffee shop management monitor sales performance and understand operational trends through interactive data visualization.

The project analyzes six months of transactional data, from **January 1 to June 30, 2023**, transforming raw sales records into meaningful business insights.

Using MySQL for initial data processing and Power BI for data modeling, calculations, and visualization, this project provides an interactive reporting solution to monitor key performance indicators (KPIs), evaluate Month-over-Month (MoM) performance, compare store locations, identify top-performing products, and explore sales patterns by day and hour.

## 2. Business Problem

Coffee shop management needs an efficient way to monitor sales performance and operational activities across different locations and time periods.

Without an integrated reporting dashboard, analyzing sales trends, comparing monthly performance, identifying high-performing products, and understanding peak transaction hours may require repetitive manual queries and reporting processes.

This project addresses these challenges by developing an interactive dashboard that transforms transactional data into accessible business information to support data-driven decision-making.

## 3. Project Objectives

The main objectives of this project are:

- Monitor key business performance indicators, including Total Sales, Total Orders, and Total Quantity Sold.
- Analyze monthly sales performance and identify Month-over-Month (MoM) growth or decline.
- Identify transaction patterns based on weekdays, weekends, and operating hours.
- Compare sales performance across different coffee shop locations.
- Evaluate revenue contributions by product category and individual products.
- Identify peak transaction periods to support operational planning and inventory management.

## 4. Dataset Overview

| Description | Details |
| --- | --- |
| Dataset | Coffee Shop Sales Transactions |
| Data Period | January 1 – June 30, 2023 |
| Data Domain | Food & Beverage – Retail Sales |
| Total Sales | **$698,812** |
| Total Orders | **149,116** |
| Total Quantity Sold | **214,470 units** |

#### Key Data Attributes

The dataset contains transactional information, including:

- Transaction ID
- Transaction date and time
- Store ID
- Store location
- Product ID
- Product category
- Product type
- Unit price
- Transaction quantity

The dataset supports analysis of sales performance across time, locations, and product dimensions.

## 5. Tools & Technologies

| Tool | Purpose |
| --- | --- |
| MySQL | Initial data processing, SQL queries, and business metric extraction |
| Microsoft Power BI | Interactive dashboard development and data visualization |
| Power Query | Data cleaning and data preparation |
| DAX | KPI calculations and Month-over-Month analysis |
| Microsoft Excel | Supporting data preparation and management |

## 6. Methodology

The project follows a structured data analytics workflow:

### 6.1 Data Preparation & Cleaning

- Reviewed the raw transactional dataset and its structure.
- Performed data quality checks and data cleaning using Power Query.
- Standardized date and time formats.
- Adjusted data types to support accurate calculations and analysis.

### 6.2 SQL Data Processing & Analysis

Used MySQL to process transactional data and extract business metrics through SQL queries.

Key SQL techniques included:

- Data type conversion using `STR_TO_DATE()`.
- Aggregation using `SUM()`, `COUNT()`, and `AVG()`.
- Data grouping and filtering using `GROUP BY` and `WHERE`.
- Subqueries for daily sales analysis.
- Window functions, particularly `LAG()`, for Month-over-Month comparisons.

### 6.3 Data Modeling & DAX Calculations

- Developed data relationships between the transaction table and the date/calendar table.
- Created business measures using DAX.
- Implemented `CALCULATE()` and `DATEADD()` for time-based calculations.
- Developed MoM sales comparisons, including percentage changes and absolute differences.

### 6.4 Dashboard Development

Designed an interactive Power BI dashboard with KPI cards, sparklines, calendar heatmaps, bar charts, sales trends, and time-based analysis.

An interactive month slicer allows users to explore sales performance across different reporting periods.

## 7. Dashboard Preview

### Dashboard Components

| Visualization | Business Purpose |
| --- | --- |
| KPI Cards & Sparklines | Monitor Total Sales, Total Orders, Total Quantity Sold, and MoM performance |
| Calendar Heatmap | Explore daily sales performance through an interactive calendar |
| Sales by Weekday / Weekend | Compare revenue contribution between weekdays and weekends |
| Sales by Store Location | Evaluate sales performance across Hell's Kitchen, Lower Manhattan, and Astoria |
| Daily Sales Trend | Monitor daily revenue trends and compare them with average sales |
| Sales by Product Category | Identify product categories with the highest revenue contribution |
| Top 10 Products by Sales | Identify the highest revenue-generating products |
| Sales by Days & Hours | Analyze transaction patterns and identify peak operating periods |

## 8. Key Findings

*Insights derived from the February 2023 dashboard analysis.*

- **Sales Performance Decline:** Sales decreased by **6.8% MoM**, accompanied by declines in orders (-5.5%) and quantity sold (-5.3%). This indicates that the revenue decline coincided with lower transaction volume and product demand, highlighting the need to investigate changes in customer purchasing activity.
- **Revenue Dependency:** Coffee and tea together accounted for approximately 67% of total sales, totaling $51,000. This concentration underscores the significance of maintaining product availability and prioritising inventory planning for these two major revenue-generating categories.
- **Operational Demand Patterns:** The 08:00–10:00 period generated **$27.74K (36.4% of monthly sales)**. This suggests that morning operations represent a critical revenue period, where staff allocation and inventory readiness should be prioritized.
- **Store Performance Balance:** Sales across the three locations ranged from **$25.11K to $25.72K**, indicating relatively balanced revenue distribution. Management can focus on improving individual store productivity rather than relying solely on location-based revenue comparisons.
- **Product Revenue Concentration:** Barista Espresso generated **$10.03K**, representing approximately **13.2% of monthly sales**. Its substantial revenue contribution makes it a priority product for inventory monitoring and further evaluation of sales and profitability.
- **Weekday vs. Weekend Performance:** Weekdays contributed **71% of total revenue**, compared with 29% on weekends. However, after accounting for the number of days in February, average daily sales were approximately $2.70K on weekdays and $2.77K on weekends. This suggests that weekend sales performance should be evaluated using daily averages rather than total revenue alone.

## 9. Business Recommendations

Based on the analytical findings, several business recommendations can be considered:

1. **Investigate Sales Decline:** Evaluate changes in order volume, product demand, and average order value to understand the factors contributing to the monthly sales decline.
2. **Optimize Morning Operations:** Review staff scheduling and inventory preparation during the 08:00–10:00 period to support operational efficiency during high-revenue hours.
3. **Prioritize High-Contributing Categories:** Maintain appropriate inventory levels for Coffee and Tea, which collectively account for approximately 67% of February revenue.
4. **Evaluate Store Productivity:** Compare sales, order volume, and average order value across locations to identify operational improvement opportunities.
5. **Develop Data-Driven Weekend Strategies:** Use normalized daily performance metrics to assess weekend demand before introducing targeted promotional campaigns.

## 10. Business Impact

Developed an interactive Power BI dashboard that consolidates sales KPIs, Month-over-Month comparisons, product performance, store-level revenue, and time-based sales patterns.

The dashboard transforms transactional data into actionable business insights by enabling management to:

- Monitor monthly sales performance and identify potential declines.
- Understand revenue contribution across product categories and individual products.
- Identify high-revenue operating periods for staff and inventory planning.
- Compare store performance to support operational evaluation.
- Explore sales patterns interactively without relying on repetitive manual reporting queries.

The project demonstrates how SQL-based data processing and Power BI visualization can support structured business performance monitoring and data-driven operational decision-making.

## 11. Skills Demonstrated

- **SQL & Database Analysis:** MySQL, data cleaning, data aggregation, subqueries, and window functions.
- **Business Intelligence:** Power BI, dashboard development, KPI monitoring, and reporting.
- **Data Modeling:** Date table relationships and time-based analysis.
- **Data Analysis:** Exploratory Data Analysis (EDA), sales trend analysis, and business performance evaluation.
- **Data Visualization:** KPI cards, sparklines, bar charts, calendar heatmaps, and time-based heatmaps.
- **Business Acumen:** Business problem identification, insight generation, and operational recommendations.
