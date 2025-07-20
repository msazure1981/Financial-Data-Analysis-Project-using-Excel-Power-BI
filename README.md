# 💳 Personal Financial Insights using Excel & Power BI | HDFC Bank Statement (2015–2025)

## 📘 Project Overview

This project showcases how to clean, transform, and visualize personal banking transactions using **Microsoft Excel** and **Power BI**. The dataset is sourced from my personal HDFC bank statement covering **July 2015 to July 2025**. The goal is to:
- Understand personal spending behavior
- Analyze income vs. expenses
- Identify savings patterns and financial habits

## 📂 Dataset Description

- **Source**: HDFC bank account Excel statement
- **Period**: July 2015 – July 2025
- **Fields**:
  - Date
  - Narration (transaction description)
  - Chq/Ref Number
  - Withdrawal Amount
  - Deposit Amount
  - Closing Balance

> 🔒 Note: All personal/sensitive details have been anonymized.

---

## 🧹 Data Cleaning (Excel)

Performed using Microsoft Excel:
- Removed merged headers, blank rows, footnotes
- Renamed columns for clarity
- Parsed dates into consistent `yyyy-mm-dd` format
- Converted text-based currency values into numeric fields
- Created a new column to classify transactions using keyword logic (EMI, ATM, Salary, UPI, Transfer, Shopping, etc.)

---

## 📊 Power BI Visualizations

The cleaned Excel data was imported into Power BI to create interactive dashboards.  

### 🖼 Power BI Dashboard Preview

![Power BI Dashboard](./images/powerbi_dashboard.png)

---

## 📈 Insights & Key Metrics

### 💵 Income vs Expenses
- Consistent salary inflows visible across years
- Spikes in expenses aligned with EMIs, education payments, and major withdrawals

### 💸 Cash Flow Trends
- Monthly cash flow shows seasonal dips, likely due to EMI spikes or large transfers

### 🏦 Net Savings & Balance Growth
- Overall net savings of ₹837K over 10 years
- Compound balance growth visible post-2019

### 🧾 Spending Categories (Auto-classified)
| Category         | % of Expenses |
|------------------|---------------|
| EMI Payments     | 23.1%         |
| Utility & Bills  | 18.1%         |
| ATM Withdrawals  | 12.0%         |
| Transfers        | 10.4%         |
| Shopping & Misc  | 36.4%         |

---

## 📁 Folder Structure

HDFC-Financial-Insights-Portfolio/
│
├── Excel/
│ ├── Raw_Statement.xlsx
│ └── Cleaned_Statement.xlsx
│
├── PowerBI/
│ └── HDFC_Banking_Report.pbix
│
├── images/
│ └── powerbi_dashboard.png
│
└── README.md

---

## 📌 Tools Used

- Microsoft Excel – Data cleaning & transformation
- Microsoft Power BI – Dashboards & insights
- GitHub – Project versioning and portfolio hosting

---

## ✅ What I Learned

- Excel scripting & cleaning large, messy datasets
- Pattern recognition in personal finance
- Advanced Power BI visualization design
- Presenting raw data as clear, actionable insight

---

📊 Power BI Report Pages & Visuals 
1. Overview Page
KPI Cards:

Total Debits

Total Credits

Total Transactions

Net Balance

2. Monthly Analysis
Column Chart: Debit vs Credit by Month

Line Chart: Running Balance over Time

3. Category Analysis
Pie Chart: Spending by Category

Stacked Bar: Category-wise monthly debit

4. Trends & Outliers
Scatter Plot: Debit amounts vs Dates (highlight large spikes)

Slicer: Filter by Category or Month

💡 Measures to Create in Power BI
Few DAX measures:
Total Debit = SUM('Sheet1'[Debit Amount])
Total Credit = SUM('Sheet1'[Credit Amount])
Net Balance = SUM('Sheet1'[Credit Amount]) - SUM('Sheet1'[Debit Amount])
Transaction Count = COUNTROWS('Sheet1')---

## 📬 Contact

Feel free to connect on [LinkedIn](https://www.linkedin.com/) or raise an issue for collaboration ideas.

