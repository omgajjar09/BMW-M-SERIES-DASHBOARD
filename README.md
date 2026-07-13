# 🚗 BMW M Series Sales Performance Dashboard | Power BI

## 📌 Project Overview

The **BMW M Series Sales Performance Dashboard** is an interactive Business Intelligence (BI) solution developed using **Microsoft Power BI**. This dashboard analyzes BMW M Series vehicle sales, customer behavior, dealership performance, and regional sales trends to help management make data-driven business decisions.

The project combines multiple datasets into a star schema data model and provides interactive reports using KPIs, charts, slicers, maps, and drill-through features.

---

# 🎯 Project Objectives

The main objectives of this dashboard are:

* Analyze overall BMW M Series sales performance.
* Monitor revenue and units sold across different regions.
* Compare performance by vehicle model and body type.
* Understand customer purchasing behavior.
* Evaluate dealership and sales representative performance.
* Identify top-selling BMW M Series models.
* Track sales trends over time.
* Improve decision-making using interactive visualizations.

---

# 🛠 Tools & Technologies Used

| Tool                            | Purpose                        |
| ------------------------------- | ------------------------------ |
| Microsoft Power BI Desktop      | Dashboard Development          |
| Power Query                     | Data Cleaning & Transformation |
| DAX (Data Analysis Expressions) | Measures & Calculations        |
| CSV Files                       | Data Source                    |
| Data Modeling                   | Relationship Creation          |
| Interactive Visualizations      | Business Reporting             |

---

# 📂 Project Files

```
BMW M Series Dashboard.pbix
│
├── Sales.csv
├── Car Detail.csv
├── Customer.csv
├── Date.csv
└── README.md
```

---

# 📊 Dataset Information

## 1. Sales Table

This is the primary fact table that stores every vehicle sale.

### Columns

* Order ID
* Order Date
* Delivery Date
* Delivery Days
* Car ID
* Customer ID
* Region
* Country
* Dealer
* Sales Representative
* Customer Type
* Order Channel
* Payment Method
* Discount %
* Final Price (USD)
* Certified Pre-Owned
* Mileage at Sale
* Warranty Years
* Customer Satisfaction Score
* Units Sold

Total Records: **5,000**

---

## 2. Car Detail Table

Contains complete information about BMW M Series vehicles.

### Columns

* Car ID
* Model
* Variant
* Model Year
* Body Type
* Engine
* Cylinders
* Transmission
* Drivetrain
* Fuel Type
* Color
* Horsepower
* 0–100 km/h Time
* Top Speed
* MSRP

Total Records: **2,128**

---

## 3. Customer Table

Contains customer profile information.

### Columns

* Customer ID
* Customer Name
* Customer Segment
* Email
* Phone
* Customer Since
* Loyalty Tier

Total Records: **3,900**

---

## 4. Date Table

Provides a complete calendar table for time intelligence.

### Columns

* Date ID
* Date
* Year
* Quarter
* Quarter Label
* Month
* Month Name
* Month Label
* Day
* Day Name
* Week of Year
* Weekend Indicator

Total Records: **1,812**

---

# ⭐ Data Model

The dashboard follows a **Star Schema** design.

## Relationships

| From                 | To                    | Relationship |
| -------------------- | --------------------- | ------------ |
| Sales[Car_ID]        | Car Detail[Car_ID]    | Many-to-One  |
| Sales[Customer_ID]   | Customer[Customer_ID] | Many-to-One  |
| Sales[Order_Date_ID] | Date[Date_ID]         | Many-to-One  |

This structure improves query performance and simplifies DAX calculations.

---

# 📈 Dashboard Features

## Executive Overview

Provides a complete summary of business performance using KPI cards.

### KPIs

* Total Revenue
* Total Orders
* Units Sold
* Average Selling Price
* Average Discount
* Customer Satisfaction
* Delivery Time
* Revenue Growth

---

## Sales Analysis

Shows overall sales trends.

Visuals include:

* Monthly Sales Trend
* Revenue by Year
* Orders by Month
* Revenue by Quarter
* Sales Growth

---

## Vehicle Performance

Analyzes BMW M Series models.

Visualizations include:

* Sales by Model
* Revenue by Body Type
* Horsepower Analysis
* Engine Distribution
* Fuel Type Analysis
* Top Speed Comparison

---

## Customer Analysis

Provides customer insights.

Includes:

* Customer Segments
* Loyalty Tier
* Customer Type
* Purchase Frequency
* Customer Satisfaction

---

## Regional Analysis

Displays geographic sales performance.

Includes:

* Revenue by Region
* Revenue by Country
* Dealer Performance
* Sales Representative Performance
* Interactive Map

---

## Performance Dashboard

Shows business KPIs.

Includes:

* Gauge Charts
* KPI Cards
* Trend Indicators
* Growth Percentage
* Revenue Comparison

---

# 📊 Interactive Features

The dashboard contains:

* Dynamic Slicers
* Cross Filtering
* Drill Down
* Drill Through
* Tooltips
* Bookmarks
* Interactive Navigation Buttons
* Dynamic Titles

---

# 📐 DAX Measures Used

Examples of important measures:

```
Total Revenue

Total Orders

Units Sold

Average Selling Price

Revenue Growth %

Previous Year Revenue

Average Discount

Customer Satisfaction

Total Customers

Average Delivery Days

Top Selling Model

Revenue by Region
```

---

# 📉 Business Insights

The dashboard helps answer important business questions such as:

* Which BMW M Series model generates the highest revenue?
* Which region has the highest sales?
* Which dealer performs best?
* Which customer segment contributes the most revenue?
* What is the average selling price?
* Which payment method is most preferred?
* How much discount is provided on average?
* Which sales representative generates the highest revenue?
* How has revenue changed over time?
* Which vehicle body type sells the most?

---

# 🎨 Dashboard Design

Design Features:

* Premium BMW-inspired Theme
* Dark Dashboard Layout
* White Icons
* KPI Cards
* Professional Color Palette
* Interactive Navigation
* Responsive Visual Design

---

# 🚀 Key Benefits

* Real-time business insights
* Improved decision-making
* Easy sales monitoring
* Better customer understanding
* Regional performance analysis
* Dealer performance tracking
* Revenue trend forecasting
* Executive-level reporting

---

# 📚 Skills Demonstrated

This project demonstrates proficiency in:

* Power BI
* Power Query
* Data Modeling
* Star Schema
* DAX
* Business Intelligence
* Data Visualization
* Dashboard Design
* Data Analysis
* KPI Reporting

---

# 📌 Future Enhancements

Possible improvements include:

* Live SQL Database Integration
* Real-Time Dashboard Refresh
* AI-Based Sales Forecasting
* Predictive Analytics
* Mobile Dashboard Optimization
* Row-Level Security (RLS)
* Power BI Service Deployment
* Automated Email Reports

---
