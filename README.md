# Tata Online Retail Performance – Tableau Dashboard

This repository contains a Tableau dashboard that analyzes online retail performance for Tata using the **Tata Online Retail Dataset** from Kaggle.

---

## 📌 Project Overview

The goal of this project is to understand **sales performance, revenue trends, and profitability** across products and countries for Tata’s online retail business.

The dashboard is designed to be:
- **Executive-friendly** – high-level KPIs at the top
- **Analytical** – detailed table for drilling into products
- **Visual** – trends, distributions, and geographical view in one place

---

## 📊 Dataset

- **Source**: [Tata Online Retail Dataset – Kaggle](https://www.kaggle.com/datasets/ishanshrivastava28/tata-online-retail-dataset)
- **Owner**: Ishan Shrivastava (dataset author on Kaggle)
- **Data Type**: Transactional online retail data

> ⚠️ Note: The raw dataset is not mine. All credit for the dataset goes to the original author.  
> Depending on the license, the full dataset may or may not be included in this repository.  
> If it is not included, you can download it directly from Kaggle using the link above.

Typical columns include:
- `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `UnitPrice`, `InvoiceDate`, `Country`
- Calculated fields used in Tableau (e.g. `Total Price`, `Profit`)

---

## 🧮 Key Metrics & Calculations

The dashboard focuses on three main KPIs:

1. **Total Revenue**  
   - Formula: `SUM(Quantity * UnitPrice)`
2. **Sales Quantity**  
   - Formula: `SUM(Quantity)`
3. **Profit** (if used in the workbook)  
   - Example formula: `SUM([Total Price]) * [Profit Margin]` or a calculated field defined in Tableau.

These KPIs are displayed in large tiles at the top of the dashboard.

---

## 📈 Dashboard Contents

The Tableau dashboard includes:

1. **KPI Tiles**
   - Total Revenue
   - Sales Quantity
   - Total Profit

2. **Product Detail Table**
   - Product description
   - Order quantity
   - Profit
   - Total price

3. **Revenue by Year (Line Chart)**
   - Shows how yearly revenue evolves over months and across years.
   - Helps identify growth, seasonality, and peaks in performance.

4. **Top 5 Products (Pie Chart)**
   - Shows the share of revenue/quantity from the top-performing products.
   - Highlights key contributors to sales.

5. **Top Countries (Pie Chart)**
   - Shows which countries contribute most to sales.

6. **Sales by Country (Map)**
   - A filled map visualization showing sales distribution geographically.
   - Quickly shows strong and weak regions.

---

## 🛠 Tools Used

- **Tableau Desktop** – Dashboard creation and visualization
- **Microsoft Excel / CSV** – Data storage / basic cleaning (if applicable)
- **Kaggle** – Data source platform

---

## 📂 Repository Structure

```text
.
├── README.md                                    # Project documentation
├── TATA_online_retail_performance.twbx          # Packaged Tableau workbook (recommended to open)
├── TATA_online_retail_performance.twb           # Workbook version requiring separate data source
└── TATA_Online_Retail_Analysis_Dashboard.png    # Dashboard screenshot preview

