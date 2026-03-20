# 🚀 AI-Driven Supply Chain & Operations Intelligence Dashboard

---

## 📊 Dashboard Overview

### 🟦 Supply Chain Intelligence Dashboard

![Landing Page](Screenshots/page1.png)

### 📊 Executive Overview

![Executive Overview](Screenshots/page2.png)

### 🚚 Operations & Logistics Dashboard

![Operations Dashboard](Screenshots/page3.png)

### 👥 Customer & Product Insights

![Customer Insights](Screenshots/page4.png)

---

## 📌 Overview

This project presents a comprehensive **end-to-end Power BI solution** designed to analyze supply chain performance, operational efficiency, and customer-product insights.

The dashboard enables stakeholders to make **data-driven decisions** through interactive and visually rich reports.

---

## 🎯 Objectives

* Analyze **sales and profitability trends**
* Monitor **delivery performance and logistics efficiency**
* Identify **high-value customers and top-performing products**
* Evaluate **discount impact on profitability**
* Deliver an **interactive and intuitive dashboard experience**

---

## 🧱 Data Model

### 📊 Tables Used

* **orders** → Sales, Profit, Discount
* **customers** → City, Segment
* **products** → Category
* **shipments** → Delivery & Shipping data
* **suppliers** → Supplier performance

### 🔗 Relationships

* orders → customers (CustomerID)
* orders → products (ProductID)
* orders → suppliers (SupplierID)
* orders → shipments (OrderID)

---

## 📄 Dashboard Pages

---

### 🟦 Page 1: Supply Chain Intelligence Dashboard

* Clean UI design with background and branding
* Navigation button for smooth user flow
* Professional dashboard entry screen

---

### 📊 Page 2: Executive Overview

#### KPIs:

* Total Revenue
* Total Profit
* Total Orders
* Avg Order Value
* Avg Discount

#### Visuals:

* Revenue Trend
* Revenue by Category
* Revenue by City
* Profit vs Discount

---

### 🚚 Page 3: Operations & Logistics

#### KPIs:

* On-Time %
* Avg Days
* Late Orders
* Shipments
* Avg Cost

#### Visuals:

* Delivery Trend
* Supplier Performance
* On-Time vs Late Deliveries
* Shipping Cost by City

---

### 👥 Page 4: Customer & Product Insights

#### KPIs:

* Total Customers
* Avg Order Value
* Profit Margin %
* Top Revenue
* CLV (Customer Lifetime Value)

#### Visuals:

* Top Customers
* Top Products
* Segment Analysis
* Profit vs Sales

---

## ⚙️ DAX Measures

```DAX id="zzm2n3"
On-Time % = 
DIVIDE([On Time Orders], [Total Shipments])

Profit Margin % = 
DIVIDE(
    SUM('orders'[Profit]),
    SUM('orders'[SalesAmount])
)

CLV = 
DIVIDE(
    SUM('orders'[SalesAmount]),
    DISTINCTCOUNT('orders'[CustomerID])
)
```

---

## 🎨 Design & UX

* Dark-themed modern UI
* Clean KPI cards with icons
* Rounded containers for visuals
* Minimal slicers for better usability
* Cross-filtering enabled

---

## 🔄 Deployment

* Published to **Power BI Service**
* Configured **daily scheduled refresh**
* Ensures real-time data updates

---

## 💡 Key Insights

* Revenue shows consistent growth
* High discounts reduce profitability
* Certain cities dominate sales performance
* Supplier delays affect delivery efficiency
* Top customers contribute majority revenue

---

## 🛠️ Tools & Technologies

* Power BI Desktop
* DAX (Data Analysis Expressions)
* Power BI Service
* Data Modeling (Star Schema)

---

## 💼 Business Value

* Enables executive decision-making
* Improves operational efficiency tracking
* Supports customer segmentation
* Helps optimize profitability

---

## 📌 Project Highlights

✔ End-to-end dashboard development
✔ Multi-page analytical reporting
✔ Advanced DAX calculations
✔ Real-world deployment
✔ Automated data refresh

---

## 🔗 Project Link

👉 *(Add your Power BI Service link here)*

---

## 📁 Project Structure & Usage

### 📂 Folder Details

* **Datasets/**
  Contains all raw CSV files used in the dashboard

* **Screenshots/**
  Stores dashboard images for all pages

* **.pbix File**
  Main Power BI report file

* **README.md**
  Documentation file

---

## ⬇️ How to Use

### 🔹 Step 1: Download Project

```bash id="f4n7jz"
git clone https://github.com/your-username/your-repo-name.git
```

OR download ZIP from GitHub

---

### 🔹 Step 2: Open Dashboard

1. Open **Power BI Desktop**
2. Click:

   ```
   File → Open
   ```
3. Select `.pbix` file

---

### 🔹 Step 3: Load Data (if needed)

* Go to **Transform Data**
* Update file paths from **Datasets folder**

---

### 🔹 Step 4: Explore Dashboard

* Use slicers for filtering
* Click charts for cross-filtering
* Navigate between pages

---

## ⚠️ Notes

* Use latest Power BI Desktop version
* Update dataset paths if required

---

## 👤 Author

**Mehtab Khan**
Aspiring Data Analyst | Power BI Developer

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---
