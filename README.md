# 🏭 Machine Output Power BI Dashboard

> **Replacing manual log reporting with a real-time analytics pipeline in a semiconductor manufacturing environment.**

---

## 📌 Project Overview

In a semiconductor/electronics manufacturing facility, production teams relied on **manual extraction and reporting** from machine `.log` files to track daily output — a tedious, error-prone process that consumed over **2 hours of engineering time every day**.

This project delivered an **end-to-end automated data pipeline and Power BI dashboard** that eliminated manual reporting entirely, giving process engineers, production engineers, and upper management instant access to production metrics and yield trends.

---

## 🎯 Business Problem

| Pain Point | Impact |
|---|---|
| Manual `.log` file extraction & processing | 2+ hours lost daily per reporting cycle |
| No centralized view of machine output | Engineers couldn't track trends efficiently |
| Delayed data reaching management | Decisions based on outdated information |
| Human error in manual reporting | Inconsistent and unreliable numbers |

---

## 💡 Solution

Built a fully automated pipeline — from raw `.log` file ingestion to an interactive Power BI dashboard — enabling **real-time visibility** into machine output, yield, and rejection rates across the production floor.

---

## 📊 Dashboard Features

- **Production Output Tracking** — Monitor total input and output units per machine, per shift, and over time
- **Rejection Quantity & Rate** — Identify defect trends at a granular level to drive process improvement
- **Yield Trend Analysis** — Visualize yield performance over time to spot degradation or improvement
- **Anomaly Detection** — Flagging of abnormal readings identified during exploratory data analysis
- **Multi-level Reporting** — Views tailored for engineers (detailed drill-down) and management (high-level KPIs)

---

## 🔄 Data Pipeline Architecture

```
[Machine System]
      │
      ▼
 .log files (raw output)
      │
      ▼
[PowerShell Scripts]
  • Auto-scan shared folder for new files
  • Unzip & extract relevant log entries
  • Parse and structure raw data
      │
      ▼
[Excel — Exploratory Data Analysis]
  • Data cleansing & validation
  • Anomaly detection
  • Structured output for Power BI
      │
      ▼
[Power BI Dashboard]
  • Real-time visual analytics
  • Interactive filters & drill-through
  • Shared across 35+ stakeholders
```

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **PowerShell** | Automated file scanning, unzipping, data extraction & processing |
| **Microsoft Excel** | Exploratory Data Analysis (EDA), anomaly detection, data structuring |
| **Microsoft Power BI** | Interactive dashboard & data visualization |

---

## 📈 Results & Impact

| Metric | Result |
|---|---|
| ✅ Data Accuracy | **97%** (up from error-prone manual extraction) |
| ⏱️ Time Saved | **2+ hours eliminated** from daily manual processing |
| 👥 Stakeholders Served | **35+ users** across 3 levels of the organization |
| 📉 Manual Reporting | **Fully eliminated** |

---

## 👥 Stakeholder Impact

| Role | How They Used the Dashboard |
|---|---|
| **Process Engineers (~20)** | Tracked machine input/output and rejection rates to drive process improvement initiatives |
| **Production Engineers (~5–10)** | Monitored daily production performance and shift-level output |
| **Managers / Upper Management (~8)** | Used yield trends and output forecasts to support site-level production planning and decision-making |

---

## 📁 Repository Structure

```
machine-output-powerbi-dashboard/
│
├── README.md                   ← You are here
├── dashboard.pbix              ← Power BI report file (sanitized)
├── scripts/
│   └── extract_data.ps1        ← PowerShell automation script (sanitized)
└── assets/
    └── dashboard_preview.png   ← Dashboard screenshot
```

> ⚠️ **Note:** All data in this repository has been sanitized. Machine identifiers, production values, and any proprietary information have been replaced with anonymized dummy data to protect confidentiality.

---

## 🚀 How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/fariezeirfan/machine-output-powerbi-dashboard.git
   ```

2. **Run the PowerShell script** to simulate the data extraction pipeline
   ```powershell
   .\scripts\extract_data.ps1
   ```

3. **Open `dashboard.pbix`** in Microsoft Power BI Desktop to explore the report

---

## 👤 About the Author

**Fariez Eirfan** — Aspiring Data Analyst with a background in Mechanical Engineering (UTM). Passionate about turning raw operational data into actionable insights that drive real business decisions.

🔗 [LinkedIn](https://www.linkedin.com/in/fariezeirfan)

---

*Built during an apprenticeship program in the semiconductor/electronics manufacturing industry.*
