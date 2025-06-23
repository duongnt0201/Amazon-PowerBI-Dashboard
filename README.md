# 📊 Amazon Ads Data Processing | Google Colab

![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

---

## 📖 Overview

This project provides a **Google Colab** notebook that automates the processing of Amazon Ads Excel reports (Sponsored Products, Sponsored Display, Sponsored Brand). It:

- Uploads your raw `.xlsx` file into Colab  
- Reads and cleans multiple sheets  
- Matches campaign names to SKUs from a Google Sheets checklist  
- Identifies campaigns missing SKU references  
- Aggregates Spend & Sales by Date and SKU  
- Exports a final cleaned report and downloads it

---

## 🧰 Technologies & Libraries

- **Google Colab** (Python 3 runtime)  
- **pandas**, **numpy**  
- **google.colab.files** for upload/download  
- **io** (built-in)

---

## 🚀 How to Use

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload your `.xlsx` file containing three sheets:
   - Sponsored_Products
   - Sponsored_Display
   - Sponsored_Brand
3. The script will process, check SKU matching, and export a final report.

## 📥 Input Format

- An Excel file (.xlsx) with 3 campaign type sheets
- A Google Sheets checklist for SKUs (provided via link in code)

## 📦 Output

- A cleaned `.xlsx` report summarizing Spend and Sales per SKU per day




# 📊 Amazon Ads Performance Dashboard for Automotive Category | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)

**Author:** Nguyễn Tùng Dương

**Date:** Sep 2024

**Tools Used:** Power BI

---

## 📑 Table of Contents

- [📌 Background & Overview](#-background--overview)  
- [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
- [🧠 Design Thinking Process](#-design-thinking-process)  
- [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
- [🔎 Final Conclusion & Recommendation](#-final-conclusion--recommendation)

---

## 📌 Background & Overview
### 📖 What is this project about?

This project analyzes Amazon advertising and sales performance for the **Automotive** category in 2024, with the following objectives:

- Track key performance indicators (KPIs): **Ad Sales, Spend, ROAS, ACoS, CVR**
- Compare performance year-over-year (YoY)
- Identify top-performing products, niches, and markets
- Evaluate the effectiveness of ad campaign types (SP, SB, SD)
- Provide insights for smarter ad spend and strategy optimization

---

## 👤 Who is this project for?

This dashboard is designed for:

- **E-commerce Marketing Managers**
- **Digital Marketing Teams**
- **Team Leaders & Marketing Managers**
---

## ❓ Business Questions

- How are total sales, ad sales, and advertising spend currently performing?
- Which Automotive products are the best-selling across platforms?
- Which ad campaigns are delivering the best performance in terms of revenue and profitability (based on ACoS/TACoS and ROAS)?
- How have sales and advertising spend trends evolved over time (monthly, yearly)?
- How does sales and advertising performance vary across markets (e.g., United States, Canada) and product niches?
- What is the conversion rate (CVR) across different campaign types and product segments?
- How have total sales, ad sales, and advertising costs changed compared year-over-year?

---

## 🎯 Project Outcome

The dashboard helped identify critical areas for improvement in procurement operations. Key results include:

### 🎯 Project Outcome

This project provided comprehensive insights into the performance of Amazon ad campaigns and product sales in the automotive category:

- ✔️ Monitor key performance indicators (KPIs): Sales, ad spend, ROAS, and ACoS
- ✔️ Identify high-performing SKUs, growth niches, and effective ad formats
- ✔️ Understand performance across different markets (e.g., US, Canada) and product segments
- ✔️ Make data-driven decisions to optimize advertising strategies, reduce costs, and drive overall business growth
- ✔️ Track year-over-year (YoY) performance to uncover areas for improvement or further investment

**Outcome:**  
### 📈 Outcome

The project empowered Digital Marketer to make smarter decisions by visualizing campaign effectiveness, identifying revenue opportunities, and optimizing ad performance. It contributed directly to improving operational efficiency, advertising ROI, and strategic planning across Amazon marketplaces.

---

## 📂 Dataset Description & Data Structure

### 📂 Dataset Description

This project uses a simulated dataset based on actual performance of Amazon advertising campaigns in the automotive category.

### 📌 Data Source

- **Source:** Sample data based on real Amazon campaign performance  
- **Format:** `.pbix` (Power BI Desktop)

---

### 📊 Data Structure & Relationships


#### 1️⃣ Table Used
### 📊 Data Structure & Tables

The dataset consists of 7 main tables used to build the purchasing performance dashboard:

| No. | Table Name                           | Description                                |
|-----|--------------------------------------|--------------------------------------------|
| 1  | **Fact_Purchasing_OrderDetail**      | Line-level order details                   |
| 2  | **Fact_Product_Inventory**           | Current inventory levels                   |
| 3  | **Dim_Product_Product**              | Product master data                        |
| 4  | **Dim_Purchasing_OrderHeader**       | Order-level metadata                       |
| 5  | **Dim_Purchasing_Vendor**            | Vendor master data                         |
| 6  | **Dim_Purchasing_ProductVendor**     | Product-vendor mapping                     |
| 7  | **Dim_Product_ProductTaxonomy**      | Product categories                         |
| 8  | **Dim_Product_ProductTable**         | Product category and hierarchy             |

### 🔗 Data Model Relationship Diagram

Below is the relationship model used in this project:

![Power BI Model](https://prnt.sc/ZKhPNyHd-xpt)
![Power BI Data Model](https://i.imgur.com/yourImageLink.png)


