# 📊 Retail Sales Analytics Dashboard | Power BI Business Intelligence Project

An interactive Business Intelligence dashboard developed using **Power BI** to analyze retail sales performance across products, customers, stores, payment methods, and geographic regions. The project leverages **Power Query**, **DAX**, **Star Schema Data Modeling**, and interactive visualizations to transform raw transactional data into actionable business insights, enabling stakeholders to monitor KPIs, evaluate sales performance, identify growth opportunities, and support data-driven decision-making.
## 📖 Project Overview

The **Retail Sales Analytics Dashboard** is an interactive Business Intelligence solution developed using **Power BI** to transform raw retail transaction data into meaningful business insights. The dashboard enables users to monitor key performance indicators (KPIs), analyze sales trends, evaluate product performance, understand customer purchasing behavior, and compare regional sales performance through dynamic and interactive visualizations.

The project follows a complete Business Intelligence workflow, including **data cleaning and transformation using Power Query**, **Star Schema data modeling**, **Date Dimension creation**, and **DAX-based calculations** to deliver accurate and scalable analytics. Interactive slicers and cross-filtering capabilities allow users to explore the data from multiple business perspectives, making the dashboard suitable for executive reporting and operational decision-making.

Designed with business users in mind, this dashboard provides decision-makers with a centralized view of retail performance, helping identify sales opportunities, monitor profitability, compare store performance, evaluate payment trends, and support data-driven strategic planning.
# 🛠️ Tech Stack

The **Retail Sales Analytics Dashboard** was developed using a modern Business Intelligence workflow, leveraging Power BI's data transformation, modeling, and visualization capabilities to deliver an interactive and scalable analytics solution.

### 📊 Power BI Desktop

* Primary Business Intelligence platform used to design and develop the interactive dashboard.
* Created KPI cards, charts, slicers, and executive-level visualizations for retail sales analysis.

### 📂 Power Query

* Imported and transformed raw retail datasets.
* Performed data cleaning, data type conversion, and query transformations.
* Prepared structured datasets before loading them into the Power BI data model.

### 🧠 DAX (Data Analysis Expressions)

* Developed dynamic measures and business calculations, including:

  * Total Sales
  * Net Sales
  * Total Profit
  * Total Orders
  * Total Customers
  * Total Quantity Sold
  * Profit Margin (%)
  * Average Order Value
  * Discount Analysis
* Enabled dynamic KPI reporting and interactive business insights.

### 🗂️ Data Modeling

* Designed a **Star Schema** data model consisting of:

  * Sales (Fact Table)
  * Customers (Dimension Table)
  * Products (Dimension Table)
  * Stores (Dimension Table)
  * Date Table (Dimension Table)
* Established one-to-many relationships to ensure accurate filtering and aggregation across the dashboard.

### 📅 Date Dimension

* Created a dedicated Date Table using DAX.
* Generated additional date attributes such as:

  * Year
  * Month Number
  * Month Name
  * Quarter
  * Week Number
  * Day Name
* Enabled time-based analysis and supported future enhancements like Month-over-Month (MoM) and Year-over-Year (YoY) reporting.

### 📈 Data Visualization

* Built interactive visualizations to analyze:

  * Sales Performance
  * Profitability
  * Regional Sales Distribution
  * Product Performance
  * Customer Metrics
  * Store Type Analysis
  * Payment Mode Distribution
* Implemented slicers and cross-filtering to provide an intuitive user experience.

### 📁 Dataset

* Multi-table retail sales dataset consisting of:

  * Customers
  * Products
  * Sales
  * Stores
* Structured and modeled to support enterprise-style Business Intelligence reporting.

### 💾 File Formats

* **.pbix** – Power BI project file
* **.xlsx** – Source datasets
* **.png** – Dashboard preview images for documentation and GitHub repository
  
  # 📂 Data Source

The dashboard is built using a **multi-table retail sales dataset** that simulates the day-to-day operations of a retail business. The dataset captures transactional, customer, product, and store information, enabling comprehensive business performance analysis from multiple perspectives.

The project follows a **Star Schema** data model, where the **Sales** table acts as the central **Fact Table**, while the remaining tables serve as **Dimension Tables**. This modeling approach improves query performance, simplifies report development, and supports accurate filtering across the dashboard.

### Dataset Structure

#### 🛒 Sales (Fact Table)

Contains transactional data for every customer purchase.

**Key Attributes:**

* Sales ID
* Order Date
* Product ID
* Customer ID
* Store ID
* Quantity
* Sales Amount
* Discount
* Net Sales
* Cost
* Profit
* Payment Mode

---

#### 👥 Customers (Dimension Table)

Stores customer demographic and membership information.

**Key Attributes:**

* Customer ID
* Customer Name
* Gender
* Age
* City
* State
* Region
* Membership Type
* Customer Segment

---

#### 📦 Products (Dimension Table)

Contains detailed information about products available for sale.

**Key Attributes:**

* Product ID
* Product Name
* Brand
* Category
* Sub Category
* Selling Price

---

#### 🏪 Stores (Dimension Table)

Stores geographical and operational information for retail stores.

**Key Attributes:**

* Store ID
* Store Name
* City
* State
* Region
* Store Type

---

#### 📅 Date Table (Dimension Table)

A dedicated calendar table created using **DAX** to support time-based analysis and reporting.

**Generated Attributes:**

* Year
* Month Number
* Month Name
* Month-Year
* Quarter
* Week Number
* Day Name

This table enables chronological reporting and provides the foundation for advanced time intelligence calculations such as Month-over-Month (MoM) and Year-over-Year (YoY) analysis.

---

### Data Modeling Approach

The project follows the **Star Schema** modeling technique, establishing one-to-many relationships between the Sales table and each dimension table.

```
Customers
      │
Products ─── Sales ─── Stores
      │
  Date Table
```

This structure enables efficient filtering, accurate aggregations, improved report performance, and scalable Business Intelligence reporting.

# ✨ Features & Highlights

## 📌 Business Problem

Retail businesses generate large volumes of transactional data every day. However, raw sales records alone do not provide meaningful insights for business leaders. Decision-makers often struggle to answer critical business questions such as:

* Which regions generate the highest sales and profit?
* Which product categories contribute the most revenue?
* How many customers are making purchases?
* Which payment methods are most frequently used?
* How are sales performing over time?
* Which stores are delivering the best performance?

Without an interactive reporting system, identifying trends, monitoring KPIs, and making informed business decisions becomes time-consuming and inefficient.

---

## 🎯 Goal of the Dashboard

The primary objective of this project is to build an interactive **Business Intelligence Dashboard** that transforms raw retail sales data into meaningful business insights.

The dashboard is designed to:

* Monitor overall business performance through executive KPIs.
* Analyze sales trends across different time periods.
* Compare sales performance across regions, stores, and product categories.
* Evaluate customer purchasing behavior.
* Analyze payment method distribution.
* Enable interactive exploration using dynamic slicers and cross-filtering.
* Support business decision-making through visual analytics.

---

# 📊 Dashboard Walkthrough

## 📈 Executive KPI Cards

The dashboard provides a high-level overview of business performance through key performance indicators, including:

* Total Sales
* Net Sales
* Total Profit
* Total Orders
* Total Customers

These KPIs allow stakeholders to quickly evaluate overall business health without navigating through detailed reports.

---

## 📅 Monthly Sales Trend

A line chart visualizes monthly sales performance over time, helping users identify:

* Seasonal trends
* Business growth patterns
* High-performing months
* Sales fluctuations

This visualization enables decision-makers to monitor business performance throughout the year.

---

## 🌍 Regional Sales Analysis

A bar chart compares sales across different regions.

This helps businesses identify:

* Best-performing regions
* Underperforming markets
* Regional revenue distribution
* Sales opportunities across geographic locations

---

## 📦 Product Category Analysis

Category-wise analysis provides insights into which product categories generate the highest revenue and profitability.

This enables businesses to:

* Optimize product strategies
* Identify high-performing categories
* Improve inventory planning
* Focus marketing efforts on profitable segments

---

## 🏪 Store Type Analysis

The dashboard analyzes sales performance based on different store types.

Business users can evaluate:

* Store distribution
* Performance by store format
* Operational contribution of each store category

---

## 💳 Payment Mode Analysis

The payment distribution visualization highlights customer payment preferences.

This allows businesses to:

* Understand customer transaction behavior
* Evaluate adoption of digital payment methods
* Support payment infrastructure planning

---

## 🎛 Interactive Filters

The dashboard includes dynamic slicers that allow users to filter the entire report by:

* Year
* Month
* Region
* Payment Mode

These filters provide an interactive experience and enable users to perform detailed analysis without modifying the underlying data.

---

# 💼 Business Impact & Insights

The dashboard empowers business stakeholders to make faster and more informed decisions by providing a centralized analytical view of retail performance.

### Key Business Benefits

### 📈 Performance Monitoring

Track important KPIs including Sales, Profit, Orders, and Customers in real time.

---

### 🌍 Regional Decision Making

Identify high-performing and low-performing regions to optimize marketing strategies and business expansion.

---

### 📦 Product Performance Analysis

Recognize profitable product categories and support inventory optimization.

---

### 👥 Customer Insights

Monitor customer purchasing activity and evaluate business reach.

---

### 💳 Payment Behavior Analysis

Understand customer payment preferences and support digital payment adoption strategies.

---

### 📊 Executive Reporting

Provide management teams with an easy-to-understand dashboard for strategic planning, operational monitoring, and business performance evaluation.

# 📸 Dashboard Preview

## Executive Dashboard

> **Interactive Retail Sales Analytics Dashboard**

The dashboard provides a centralized view of retail business performance by combining executive KPIs, sales trends, regional comparisons, product analysis, and customer insights into a single interactive report.

### Dashboard Highlights

* 📈 Executive KPI Cards

  * Total Sales
  * Net Sales
  * Total Profit
  * Total Orders
  * Total Customers

* 📅 Monthly Sales Trend Analysis

* 🌍 Regional Sales Performance

* 📦 Product Category Analysis

* 🏪 Store Type Distribution

* 💳 Payment Mode Analysis

* 🎛 Interactive Slicers

  * Year
  * Month
  * Region
  * Payment Mode

---

## 📷 Dashboard Screenshot

> Replace the image below with your dashboard screenshot.

```text
Images/
└── Dashboard.png
```

<img src="Images/Dashboard.png" width="100%" alt="Retail Sales Analytics Dashboard">

---

# 🗂️ Data Model

The project follows a **Star Schema** data model, where the **Sales** table acts as the central Fact Table and all other tables function as Dimension Tables.

### Data Model Screenshot

```text
Images/
└── Data_Model.png
```

<img src="Images/Data_Model.png" width="85%" alt="Power BI Data Model">

---

# 🔄 Power Query

Power Query was used to prepare the raw datasets before loading them into the Power BI model.

The transformation process included:

* Data Import
* Data Cleaning
* Data Type Conversion
* Query Transformation
* Multi-table Preparation

### Power Query Screenshot

```text
Images/
└── Power_Query.png
```

<img src="Images/Power_Query.png" width="90%" alt="Power Query">

---

# 🧠 DAX Measures

The dashboard uses multiple DAX measures to calculate business KPIs dynamically.

### Measures Implemented

* Total Sales
* Total Net Sales
* Total Profit
* Total Quantity
* Total Orders
* Total Customers
* Total Discount
* Discount %
* Profit Margin %
* Average Order Value

These measures enable dynamic reporting and support interactive dashboard filtering.
