# E-Commerce Sales Analytics | Power BI

An end-to-end e-commerce analytics project built in Power BI to analyze sales performance, products, customers, and key business trends.

The project covers the full analytics workflow — from raw ODS data preparation and data modeling to DAX measures, interactive dashboards, and business insights.

## Dashboard Preview

![Executive Performance Overview](screenshots/1%20Executive%20Performance%20Overview.png)
---

## Project Overview

The goal of the project was to build an interactive analytical dashboard that helps understand:

- overall sales and order performance
- revenue trends over time
- product and category performance
- customer contribution and behavior
- geographical distribution of sales
- month-over-month business performance
- key drivers behind revenue changes

The dashboard is organized into four analytical areas:

**Executive Performance Overview → Product Analytics → Customer Analytics → Business Insights**

---

## Data & Preparation

### Source Data

The initial dataset was provided as a raw **ODS file** containing e-commerce sales data.

**Source file:** `data/e-commerce-sales-data.ods`

### Data Preparation

The raw data was imported into **Power BI** and prepared using **Power Query**.

The preparation process included:

- data type correction
- cleaning and standardizing fields
- handling missing values
- preparing revenue and discount-related fields
- creating calculated fields required for analysis
- preparing the dataset for data modeling

---

## Data Model

The analytical model was built using a relational structure in Power BI.

Main tables:

- `orders`
- `products`
- `customers`
- `Calendar`

The model connects transactional order data with product, customer, and calendar dimensions.

![Data Model](screenshots/7%20Data%20Model.png)

---

## DAX & Measures

A dedicated `_Measures` table was created to organize analytical measures.

The project includes measures for:

- Total Revenue
- Total Orders
- Customers
- Average Order Value
- Average Product Revenue
- Average Revenue per Customer
- Average Orders per Customer
- Revenue MoM %
- Orders MoM %
- Customers MoM %
- Average Order Value MoM %
- Previous Month Revenue
- Revenue Change
- Customer and product performance
- Discount analysis
- High-value orders and customers
- Revenue driver analysis

Time-based calculations were implemented using the dedicated `Calendar` table.

---

# Dashboard

## 1. Executive Performance Overview

Provides a high-level view of overall business performance.

### Key metrics

- Total Revenue
- Total Orders
- Customers
- Average Order Value

### Visualizations

- Revenue by Month
- Orders by Payment Status
- Revenue by Category
- Top 5 Countries by Revenue
- Top 10 Customers by Revenue
- Top 10 Products by Revenue

![Executive Performance Overview](screenshots/1%20Executive%20Performance%20Overview.png)

---

## 2. Product Analytics

Focuses on product and category performance.

### Key metrics

- Top Product
- Top Category
- Products Sold
- Average Product Revenue

### Visualizations

- Revenue by Category
- Category Revenue Share
- Top 10 Products by Revenue
- Top 10 Products Details

The product details table includes:

- Revenue
- Units Sold
- Average Order Value

![Product Analytics](screenshots/2%20Product%20Analytics.png)

---

## 3. Customer Analytics

Provides insights into customer contribution and geographical performance.

### Key metrics

- Total Customers
- Average Revenue per Customer
- Average Orders per Customer
- Top Customer Revenue

### Visualizations

- Revenue by Country
- Customer Share by Country
- Top 10 Customers by Orders
- Customer Performance by Country

The customer performance table allows comparison of:

- Revenue
- Orders
- Average Revenue per Customer

![Customer Analytics](screenshots/3%20Customer%20Analytics.png)

---

## 4. Business Insights

Focuses on trends, month-over-month performance, and revenue drivers.

### Key metrics

- Revenue MoM %
- Orders MoM %
- Customers MoM %
- Average Order Value MoM %

### Visualizations

- Revenue Trend
- Revenue Driver Analysis
- Key Metrics MoM Change
- Current Month Revenue
- Previous Month Revenue
- Revenue Change
- Average Order Value

The Revenue Driver Analysis provides an interactive breakdown of revenue by:

**Category → Country → Product**

![Business Insights](screenshots/4%20Business%20Insights.png)

---

## Interactive Features

The dashboard includes several interactive elements:

- slicers for Month, Country, Category, and Payment Status
- page navigation between analytical sections
- Top N filtering
- interactive visual cross-filtering
- dynamic DAX measures
- drill-down analysis
- custom report tooltips

### Interactive Tooltip

A custom tooltip was created for the Revenue Trend visualization.

When hovering over a data point, the tooltip provides additional context such as:

- Revenue MoM %
- Total Orders
- Average Order Value

This allows users to explore monthly performance without leaving the main dashboard.

![Revenue Trend Tooltip](screenshots/5%20Tooltip%20Revenue%20Trend%201.png)

![Revenue Trend Tooltip Details](screenshots/6%20Tooltip%20Revenue%20Trend%202.png)

---

## Key Business Insights

The dashboard highlights several important patterns in the dataset:

- Electronics is the leading revenue category.
- Wireless Headphones generate the highest product revenue.
- Germany and Ukraine are among the strongest markets by revenue.
- Revenue shows significant month-to-month fluctuations throughout the year.
- Customer and product performance varies considerably across markets.
- Month-over-month analysis helps identify changes in revenue, orders, customers, and average order value.

---

## Tools & Technologies

- **Power BI**
- **Power Query**
- **DAX**
- **Data Modeling**
- **Interactive Data Visualization**
- **ODS**

---
