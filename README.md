# 📊 Amazon Ads Data Processing with Google Colab

[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]

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

## 📂 Repository Structure

