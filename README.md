# Retail-Sales-Performance-Dashboard-Power-BI-
# 📊 Superstore Analytics Dashboard

A dynamic and interactive Power BI dashboard designed to analyze retail sales performance, customer behavior, and product trends using a structured star schema model.

---

## 📌 Short Description / Purpose

The Superstore Analytics Dashboard provides a comprehensive view of sales, profit, and operational performance across products, customers, and regions. It enables users to explore key business metrics and uncover insights that support data-driven decision-making.

---

## 🛠️ Tech Stack

The dashboard was built using the following tools and technologies:

• 📊 **Power BI Desktop** – Main data visualization platform used for report creation
• 📂 **Power Query** – Used for data cleaning, transformation, and shaping
• 🧠 **DAX (Data Analysis Expressions)** – Used for calculated measures and business logic
• 🧩 **Data Modeling (Star Schema)** – Fact and dimension tables structured for efficient querying and filtering
• 📁 **File Format** – `.pbix` for development

---

## 📂 Data Source

• Source: Superstore dataset (retail transactional dataset)

The dataset includes:

* Orders and sales transactions
* Product details (Category, Sub-category, Product Name)
* Customer information (Customer Id, Customer Name, Customer Segment)
* Geographic data (City, State, Region, Country)
* Time-based data (Order Date, Ship Date)

---

## ⭐ Features / Highlights

### 🔹 Business Problem

Retail businesses generate large volumes of transactional data, but without proper modeling and visualization, it becomes difficult to:

* Track sales and profitability trends
* Identify high-performing products and regions
* Make strategic decisions based on data

---

### 🎯 Goal of the Dashboard

To build an interactive analytics tool that:

* Provides a clear overview of business performance
* Enables slicing data by product, region, and time
* Supports decision-making for sales and marketing strategies
* Implements a clean and scalable data model

---

### 📊 Walkthrough of Key Visuals

#### 🔸 KPI Cards

* Total Sales
* Total Profit
* Total Orders
* Profit Margin

#### 🔸 Sales by Category (Bar Chart)

Displays performance across major product categories such as Furniture, Office Supplies, and Technology.

#### 🔸 Sub-Category Analysis

Highlights top-performing and underperforming sub-categories.

#### 🔸 Regional Performance (Map / Bar Chart)

Breaks down sales and profit by region and state.

#### 🔸 Time Series Analysis (Line Chart)

Shows trends in sales over time (monthly/yearly patterns).

---

### 📈 Business Impact & Insights

## 📈 Business Impact

- Identified **West region as top-performing**, with highest:
  - **Sales:** 725.46k  
  - **Profit:** 108.42k  
  - **Profit Margin:** 14.94%  
  → Establishes West as the primary revenue driver  

- Detected **category-level profitability imbalance**:
  - **Furniture:** 2.49% margin (lowest)  
  - **Technology:** 17.40% margin (highest)  
  → Indicates need for category-level pricing and cost optimization  

- Flagged **loss-making sub-categories despite high sales**:
  - **Tables:** Sales (206.97k) → Loss (17.73k)  
  - **Bookcases:** Sales (114.88k) → Loss (3.48k)  
  - **Office Supplies:** Sales (46.67k) → Loss (1.18k)  
  → Suggests pricing/discount inefficiencies  

- Identified **high-profit sub-categories**:
  - **Phones:** Profit (44.52k)  
  - **Copiers:** Profit (55.62k)  
  → Strong candidates for revenue prioritization  

- Highlighted **Central region underperformance**:
  - **Profit Margin:** 7.92% (lowest)  
  - **Total Profit:** 39.71k  
  → Indicates operational inefficiencies despite strong sales  

- Detected **7 loss-making segments in Central region**  
  (3 Furniture, 3 Office Supplies, 1 Technology)  
  → Points to region-specific issues in pricing, logistics, or discounting  

---

## 🧹 Data Cleaning & Modeling

* Removed duplicate product records using **Product ID**
* Resolved inconsistent product descriptions by selecting the most frequent value per Product ID
* Built dimension tables:

  * DimProduct
  * DimCustomer
  * DimGeography
  * DimDate
* Implemented **one-to-many relationships** between dimensions and fact table
* Avoided circular dependencies and ensured clean filter propagation

---

## 🧠 Key Learnings

* Importance of **star schema design** in Power BI
* Difference between **merge vs relationship**
* Understanding **filter context vs row context**
* Handling **data inconsistencies in dimension tables**
* Avoiding **many-to-many relationships and circular dependencies**

---

## 📸 Screenshots / Demo

![Dashboard Preview](https://github.com/Tarun707/Retail-Sales-Performance-Dashboard-Power-BI-/blob/main/Retail%20Sales%20Dashboard%20Screenshot.png)

## 🚀 Future Improvements

* Add advanced DAX measures (YoY growth, rolling averages)
* Enhance dashboard interactivity using bookmarks and drill-through
* Improve performance optimization
* Add tooltips and storytelling elements

---

## 🙌 Author

Tarun Rao
