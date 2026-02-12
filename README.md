# marketing-performance-powerbi-dashboard (Power BI + DAX)

**Executive Summary**

This project presents a Power BI dashboard designed to analyze multi-dimensional sales and customer performance data for a cookie distribution business. The dashboard integrates transactional order data with customer and product dimensions to deliver executive-level visibility into revenue drivers, product mix performance, customer contribution, and temporal demand patterns.

The objective was to design a scalable analytical framework that supports performance monitoring, profitability assessment, and data-driven marketing decisions.

**Business Problem**

-Marketing and sales teams require visibility into:
-Which products drive revenue and profit
-Which customers contribute the highest lifetime value
-How demand fluctuates across time (day-of-week trends)
-Geographic distribution of customers
-Order volume and unit velocity

Without a structured BI layer, performance analysis remains fragmented and reactive.
This dashboard consolidates transactional data into an integrated analytical model to enable proactive performance optimization.

**Data Model Architecture**

A star-schema-inspired relational model was implemented:

*Fact Table*
-Orders-
Order ID
Customer ID
Date
Product
Units Sold
Revenue
Cost
Derived Day of Week column

*Dimension Tables*
-Customers-
Customer ID
Name
City
State
Country

*Cookie Types*
-Cookie Type-
Revenue per Cookie
Cost per Cookie
Units Sold

**Relationships:**
Customers (1) → Orders (*)
Cookie Types (1) → Orders (*)

This structure enables efficient aggregation and filter propagation across customer, product, and time dimensions.

**Technical Stack**

1. Power BI Desktop
2. DAX (Data Analysis Expressions)
3. Relational Data Modeling
4. KPI Design & Executive Dashboarding
5. Business Intelligence Reporting

**How to Use**
Download the .pbix file and open it in Power BI Desktop to explore interactive filtering, cross-segmentation, and drill-down capabilities.
