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

---

---


# 📊 Amazon Ads Performance Dashboard for Automotive Category | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)

**Author:** Nguyễn Tùng Dương

**Date:** Sep 2024

**Tools Used:** Power BI


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

The dataset consists of 8 main tables used to build the Amazon Ads and Sales Performance Dashboard:

| No. | Table Name           | Description                                |
|-----|---------------------|--------------------------------------------|
| 1  | **Fact_PriceList**   | Price list by SKU          |
| 2  | **Fact_Order**       | Order details including quantity and units |
| 3  | **Fact_Total**       | Consolidated total sales and market KPIs   |
| 4  | **Fact_Ads**         | Advertising performance by campaign        |
| 5  | **Dim_Product**      | Product master data (SKU, ASIN, Niche, etc.) |
| 6  | **Dim_Market**       | Market information (e.g., US, Canada)      |
| 7  | **Dim_Date**         | Date dimension table for time intelligence |
| 8  | **Dim_LaunchingDate**| Product launching date           |


#### 2️⃣ Data Relationships:

[![Power BI Data Model](https://i.postimg.cc/4x9gjRtZ/Screenshot-4.png)](https://postimg.cc/YvMZmVby)


---

## 🔗 Data Model Relationships

| From Table      | To Table        | Join Key          | Relationship Type                      |
|-----------------|-----------------|-------------------|-----------------------------------------|
| Fact_Total      | Dim_Date        | Date              | Many-to-One (sales data per date)       |
| Fact_Total      | Dim_Product     | SKU               | Many-to-One (sales data per product)    |
| Fact_Total      | Dim_Market      | Market            | Many-to-One (sales data per market)     |
| Fact_Ads        | Dim_Date        | Date              | Many-to-One (ad data per date)          |
| Fact_Ads        | Dim_Product     | SKU               | Many-to-One (ad data per product)       |
| Fact_Ads        | Dim_Market      | Market            | Many-to-One (ad data per market)        |
| Fact_Order      | Dim_Product     | SKU               | Many-to-One (order data per product)    |
| Fact_Order      | Dim_Date        | Date              | Many-to-One (order data per date)       |
| Fact_PriceList  | Dim_Product     | SKU               | Many-to-One (price list per product)    |
| Dim_Product     | Dim_LaunchingDate | Product Number | Many-to-One (product linked to launch date) |

---

## 📊 Visualized Insights & Key Findings

### 1️⃣ Amazon Overview Dashboard 2024
[![Amazon Overview Dashboard 2024](https://i.postimg.cc/MKcNGkDL/Dashboard-Sample-Data-not-for-use-page-0001.jpg)](https://postimg.cc/nCJ0dPNK)
### 📌 Key Findings:
- Total Sales reached **$1.13M**, a **+94.3%** increase YoY  
- Ad Sales contributed **$591.9K**, growing by **52.3%**  
- Total Ad Spend: **$185.8K**, up **45%**, but **ACoS decreased** to 31.4%  
- **ROAS improved** to 3.19, indicating better ad efficiency  
- Top-selling products include `SW1951C`, `72873G01`, and `89-817109A3`  
- Most effective ad formats: `SP PT` and `SB Video Broad` campaigns  

---

### 2️⃣ Sales Analysis Dashboard
[![Sales Analysis Dashboard](https://i.postimg.cc/QCv67tby/Dashboard-Sample-Data-not-for-use-page-0002.jpg)](https://postimg.cc/Wq66LsxG)
### 📌 Key Findings:

- The **US market dominates** with over $1.02M in sales  
- Canada contributes $106K, Mexico remains marginal  
- Key product niches: Starter Solenoids, Fuel Pumps, Air Filters  
- Monthly sales trends indicate consistent growth, with seasonal peaks  
- Top products show high **Conversion Rates**, notably `72873G01` at **20.72%**

---

### 3️⃣ Amazon Advertising Analysis Dashboard
[![Advertising Analysis Dashboard](https://i.postimg.cc/Xvnsdtf4/Dashboard-Sample-Data-not-for-use-page-0003.jpg)](https://postimg.cc/LJ0kMCQb)
### 📌 Key Findings:

- Highest ad spend on `SB Video Broad` and `SP PT` formats  
- Overall **Conversion Rate (CVR)** improved to **7.47%**, a 0.44% increase  
- `TOS` and `SP Query` campaigns achieve outstanding CVR above **17%**  
- `Research` campaigns deliver the best **ROAS** at **4.76**  
- Average **CPC** remains low at **$0.41**, though some formats vary significantly  
- ACoS varies across campaign forms but shows an overall downward trend  

---

### 4️⃣ Year-over-Year Change Dashboard
### 📌 Key Findings:

[![Year-over-Year Change Dashboard](https://i.postimg.cc/9MrKwv2z/Dashboard-Sample-Data-not-for-use-page-0004.jpg)](https://postimg.cc/wyY0S47d)

- Significant total sales growth, led by:
  - `SW1951C`: +$19,978
  - `72873G01`: +$16,850
  - `89-817109A3`: +$9,603  
- Top ad revenue growth from:
  - `SB Video Broad`: +$54.3K  
  - `SP PT`: +$36.1K  
  - `SB Video PT`: +$40.1K  
- Certain campaigns underperformed (e.g., `SD PT`, `Performance`) requiring review  
- Ad spend efficiency improved, translating $57.6K extra spend into $203.3K more in ad revenue  

---




