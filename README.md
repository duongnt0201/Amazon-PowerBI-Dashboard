# 📊 Amazon Ads Data Processing with Google Colab

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
