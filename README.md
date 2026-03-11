# Power BI Retail Sales Performance Dashboard

An interactive Power BI dashboard analyzing retail transactions, profitability, product brand performance, and regional store operations using the Maven Market dataset.

## Dashboard Preview

<img width="1425" height="801" alt="image" src="https://github.com/user-attachments/assets/c0e1f771-d692-4c1f-9e57-e5acddc82783" /> <br/>

## Project Highlights

- One-page executive retail performance dashboard

- Hybrid **star + snowflake data model**

- DAX-based KPIs for transactions, profit, margin, and returns

- Regional store performance analysis using geographic visualization

- Product brand performance analysis

- Bookmark-based quick filtering for focused store analysis

## Project Overview

Retail businesses generate large volumes of transaction data across stores, products, and regions. Managers need a consolidated view to monitor sales performance, profitability, and operational trends across locations.

This Power BI dashboard provides an executive-level overview of retail operations using the Maven Market dataset, helping stakeholders quickly identify performance trends and profitability drivers.

## Business Problem

Retail managers need to track sales performance, profit margins, and returns across stores and product brands. Without consolidated analytics, it becomes difficult to determine:

- Whether stores are meeting performance targets

- Which product brands generate the highest profitability

- Which regions contribute the most to overall revenue

- Whether returns are affecting overall business performance

A centralized dashboard allows decision-makers to quickly evaluate operational performance and identify improvement opportunities.

## Analytical Approach

The dashboard was developed using the Maven Market dataset to provide a clear view of retail sales and operational performance.

The solution includes:

- A hybrid star + snowflake data model connecting transaction and return fact tables with dimension tables for customers, products, stores, regions, and calendar.
- DAX measures used to calculate key KPIs including total transactions, profit, profit margin, and returns.
- Geographic visualization to analyze regional store performance.
- Brand-level analysis to identify high-performing product brands.
- Bookmark-based filtering enabling quick focus on specific store segments.

## Outcome

The dashboard enables stakeholders to:

- Monitor **current month retail performance**
- Compare **profit against business targets**
- Identify **top-performing product brands**
- Analyze **regional store performance**
- Track **return volumes affecting profitability**

## Tools & Technologies

- Power BI
- DAX
- Data Modeling
- Power Query
- Data Visualization

## Data Model

The dashboard uses a **hybrid star + snowflake schema**.

Fact Tables
- Transactions_Data
- Returns

Dimension Tables
- Customers
- Products
- Stores
- Regions
- Calendar

The geographic hierarchy is normalized where **Stores connect to Regions**, creating a snowflake structure for regional analysis.

### Data Model Diagram

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/551e8867-121e-4c61-b80a-1d8049f113fb" /> <br/>

## Key DAX Measures

**Total Transactions:**

```Total Transactions = COUNTROWS(Transactions_Data)```

Counts the total number of retail transactions recorded in the dataset.

**Total Profit:**

```Total Profit = [Total Revenue] - [Total Cost]```

Calculates total profit generated from product sales across all transactions.

**Profit Margin:**

```Profit Margin = DIVIDE([Total Profit],[Total Revenue])```

Measures overall business profitability relative to revenue.

**Quantity Returned:**

```Quantity Returned = SUM(Returns[quantity])```

Calculates the total number of returned items across stores.

## Dashboard Overview

The dashboard provides a consolidated view of retail sales performance and operational insights.

### Executive KPI Section

Displays key performance indicators including:

- Current Month Transactions
- Current Month Profit
- Current Month Returns

These metrics help managers monitor business performance against targets.

### Brand Performance Analysis

A product brand table highlights:

- Total transactions per brand
- Total profit generated
- Profit margin performance
- Return rate

This helps identify the most profitable product brands.

### Geographic Store Analysis

A geographic map visualizes store activity across regions, helping stakeholders understand the distribution of retail operations.

### Revenue Trend Analysis

A time-series chart tracks weekly revenue trends, enabling managers to observe sales patterns and seasonal performance.

### Revenue vs Target

A gauge visual compares actual revenue against predefined business targets.

### Bookmark-Based Filtering

A bookmark feature allows quick filtering to analyze performance for specific store groups, such as Portland store sales, improving analytical exploration.

## Business Insights

- Portland reached 1000 sales in December to close out the year.
- High Top product return rate doubled in all three marketplaces (9 to 18 overall), at a return rate of 1.01%.
- Plato products drove the strongest overall profit margin (63.55%) in 1998.

## Skills Demonstrated

- Data Modeling (Star + Snowflake Schema)
- DAX Measure Development
- Business KPI Design
- Retail Sales Analytics
- Geographic Data Visualization
- Executive Dashboard Design

## Screenshots
### Dashboard Preview

<img width="1425" height="801" alt="image" src="https://github.com/user-attachments/assets/c0e1f771-d692-4c1f-9e57-e5acddc82783" /> <br/>

### Data Model

<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/1c7d5283-6212-432d-b298-81da75cbdc25" /> <br/>


### Author

**Vishal K**

Data Analyst | SQL | Power BI | Business Intelligence

LinkedIn: www.linkedin.com/in/vishal-io



