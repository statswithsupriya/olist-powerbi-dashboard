# Olist E-Commerce Analytics Dashboard

## Project Overview

Designed and developed an interactive Business Intelligence dashboard using the Olist E-Commerce dataset. The project focuses on analyzing revenue performance, customer behavior, seller performance, product category trends, and operational metrics through interactive visualizations and KPI reporting.

The dashboard was built using Power BI and DAX, enabling business users to monitor key performance indicators and derive actionable insights through self-service analytics.

---

## Tools & Technologies

- Power BI
- DAX
- Power Query
- Data Modeling
- Business Intelligence
- Data Visualization

---

## Dataset Overview

The Olist E-Commerce dataset contains information related to:

- Customers
- Orders
- Order Items
- Products
- Sellers
- Payments
- Reviews
- Product Categories

The dataset was used to perform revenue analysis, customer analysis, seller analysis, and business performance reporting.

---

## Dashboard Pages

### Executive Dashboard

#### KPI Cards

- Total Revenue
- Total Orders
- Total Customers
- Average Order Value (AOV)

#### Visualizations

- Revenue Trend Analysis
- Top 10 Product Categories by Revenue
- Revenue by State
- Orders by Status

#### Filters

- State Slicer

---

### Seller Analysis

#### KPI Cards

- Total Sellers
- Revenue per Seller

#### Visualizations

- Top 10 Sellers by Revenue
- Top 10 Sellers by Order Count

---

### Customer Analysis

#### KPI Cards

- Customer Count
- Revenue per Customer

#### Visualizations

- Customers by State
- Revenue by State
- Revenue per Customer by State

#### Filters

- State Slicer

---

## Data Modeling

### Fact Tables

- Orders
- Order_Items

### Dimension Tables

- Customers
- Products
- Sellers
- Product Category Translation

### Data Modeling Concepts Applied

- Star Schema
- One-to-Many Relationships
- Primary Keys
- Foreign Keys
- Filter Context
- Interactive Cross Filtering

---

## Key DAX Measures

```DAX
Total Revenue =
SUM(Order_Items[price])

Total Orders =
DISTINCTCOUNT(Orders[order_id])

Total Customers =
DISTINCTCOUNT(Customers[customer_unique_id])

AOV =
DIVIDE([Total Revenue],[Total Orders])

Order Count =
COUNTROWS(Orders)

Revenue per Customer =
DIVIDE([Total Revenue],[Total Customers])

Total Sellers =
DISTINCTCOUNT(Sellers[seller_id])

Revenue per Seller =
DIVIDE([Total Revenue],[Total Sellers])
```

---

## Business Questions Answered

- How much revenue did the business generate?
- How many orders were placed?
- How many customers made purchases?
- What is the Average Order Value?
- How has revenue changed over time?
- Which product categories generate the highest revenue?
- Which states contribute most to revenue?
- Which sellers are the top performers?
- Where are customers concentrated geographically?
- How are orders distributed across different statuses?

---

## Business Insights Generated

- Identified top revenue-generating product categories.
- Evaluated seller contribution to overall revenue.
- Analyzed geographic revenue distribution across states.
- Monitored order fulfillment through order status analysis.
- Measured Average Order Value (AOV) as a key KPI.
- Assessed customer concentration and customer value across different regions.
- Created an interactive reporting solution enabling business users to explore data through filters and slicers.

---

## Skills Demonstrated

### Power BI

- Dashboard Development
- Interactive Reporting
- KPI Reporting
- Data Visualization
- Dashboard Storytelling

### Data Modeling

- Star Schema
- Fact & Dimension Modeling
- Relationship Management
- Cardinality Management

### DAX

- Measures
- Aggregations
- DISTINCTCOUNT
- COUNTROWS
- DIVIDE
- Filter Context

### Analytics

- Revenue Analysis
- Customer Analysis
- Seller Analysis
- Product Performance Analysis
- Geographic Analysis

---
## Key Learning Outcomes

- Performed data transformation using Power Query.
- Applied data quality validation and profiling techniques.
- Implemented a Star Schema data model.
- Created and managed table relationships.
- Developed DAX measures for KPI reporting.
- Understood and applied Filter Context concepts.
- Built interactive dashboards using slicers and filters.
- Conducted revenue, customer, seller, and product analysis.
- Designed business-focused visualizations and reports.


## Data Flow

1. Imported Olist CSV files into Power BI.
2. Performed data cleaning and validation using Power Query.
3. Built a Star Schema data model using fact and dimension tables.
4. Established relationships between tables.
5. Created DAX measures for KPI calculations.
6. Developed interactive dashboards and reports.
7. Generated business insights through visual analytics.


## Project Outcome

Developed a multi-page Power BI dashboard providing executive-level visibility into revenue, customer, seller, and product performance. The dashboard enables business users to monitor KPIs, identify performance trends, and make data-driven decisions through interactive analytics and visual storytelling.
