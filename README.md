# 🧠 RFM Analysis Sales Dashboard

This repository contains a Power BI dashboard for performing **RFM (Recency, Frequency, Monetary)** analysis on customer sales data. The goal is to segment customers based on their purchasing behavior and enable real-time insights using automation tools.

---

**RFM analysis** is a data-driven technique used to:
- Identify high-value and at-risk customers
- Prioritize marketing and sales strategies
- Drive customer retention and lifetime value

This dashboard:
- Visualizes RFM segments
- Highlights top customers and churn risks
- Auto-refreshes with updated scores

---

## ⚙️ Project Architecture

1. **🔁 Data Pipeline (Python)**
   - Raw sales data processed using Python
   - RFM scores calculated per customer
   - Output saved to `rfm_scores.csv`

2. **📊 Power BI Dashboard**
   - Imports `rfm_scores.csv` as data source
   - Visualizes key RFM metrics and customer segments
   - Built with slicers, bar charts, KPIs

3. **🔄 Live Updates (Power Automate)**
   - Monitors new CSV file versions
   - Triggers Power BI data refresh
   - Enables near real-time RFM updates

---

## 📁 Repository Structure
rfm-sales-dashboard/
├── rfm_analysis.py # Python script for calculating RFM
├── rfm_scores.csv # Output CSV used in Power BI
├── SalesDashboard.pbix # Power BI report file
├── .gitignore
└── README.md
