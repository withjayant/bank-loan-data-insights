# 🏦 Bank Loan Data Insights — Power BI Dashboard

> An interactive Power BI dashboard for analyzing bank loan portfolios, tracking loan performance, identifying risk patterns, and monitoring repayment trends across borrower segments.

---

## 📌 Table of Contents

- [Problem Statement](#problem-statement)
- [Objective](#objective)
- [Dashboard Overview](#dashboard-overview)
- [Dashboard Screenshots](#dashboard-screenshots)
- [Features](#features)
- [Key Metrics & KPIs](#key-metrics--kpis)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Data Model](#data-model)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

---

## Problem Statement

The current approach to loan data analysis lacks depth and interactivity, hindering the ability to derive meaningful insights for informed decision-making. Traditional reporting methods fall short in providing a comprehensive view of lending operations, borrower behavior, and loan performance metrics.

There is a pressing need for advanced dashboard design to address these limitations and unlock the full potential of loan data — enabling stakeholders to:

- Understand lending operations end-to-end
- Track borrower behavior and demographics
- Monitor loan performance metrics in real time
- Make strategic decisions based on data-driven insights

---

## Objective

The objective is to craft a suite of **3 interconnected dashboards** that deliver dynamic and comprehensive insights into loan data, empowering decision-makers with actionable intelligence derived from robust data analysis.

These dashboards are meticulously designed to offer a holistic perspective on:

- 📊 Lending operations and financial KPIs
- 👤 Borrower demographics and behavior
- 📉 Loan performance and risk classification
- 💰 Financial metrics and repayment trends

By fulfilling these objectives, the goal is to **optimize lending strategies**, bolster financial health, and elevate borrower satisfaction through insightful data analysis and strategic dashboard design.

---

## Dashboard Overview

### Dashboard 1 — Executive Summary
**Purpose:** Provides an overview of critical Key Performance Indicators (KPIs) essential for evaluating the overall efficiency and performance of lending operations.

| KPI | Description |
|---|---|
| Total Loan Applications | Monitor total and MTD applications with MoM trend analysis |
| Total Funded Amount | Track cumulative disbursed funds and MTD disbursements with MoM variations |
| Total Amount Received | Assess cash inflows via total and MTD received amounts with MoM fluctuations |
| Average Interest Rate | Compute and track average interest rate across all loans with MTD and MoM changes |
| Average DTI | Evaluate borrowers' financial resilience via average Debt-to-Income ratio with MTD/MoM tracking |

**Loan Performance Classification:**
- ✅ **Good Loans** — Fully Paid and Current loans (application %, funded amount, received amount)
- ❌ **Bad Loans** — Charged Off loans (application %, funded amount, received amount)
- 📋 **Loan Status Grid View** — Detailed categorization by loan status for data-driven decision-making

---

### Dashboard 2 — Trends & Overview
**Purpose:** Offers interactive visualizations to illuminate lending trends, borrower demographics, and loan purposes — facilitating pattern recognition and opportunity identification.

| Visualization | Type | Insight |
|---|---|---|
| Monthly Trends by Issue Date | Line Chart | Seasonality and long-term lending trends |
| Regional Analysis by State | Filled Map | Significant lending regions and geographical disparities |
| Loan Term Analysis | Donut Chart | Distribution of loans across different terms |
| Employment Length Analysis | Bar Chart | Impact of employment history on lending metrics |
| Loan Purpose Breakdown | Bar Chart | Reasons behind borrowers' financing needs |
| Home Ownership Analysis | Tree Map | Influence of home ownership on loan applications |

---

### Dashboard 3 — Detailed Insights
**Purpose:** Offers a deep dive into loan data, equipping users with comprehensive access to key metrics and loan details — empowering fully informed decision-making.

A user-friendly platform providing a comprehensive solution for in-depth analysis of the loan portfolio, augmenting the capacity to make informed lending decisions at the individual loan level.

---

## Dashboard Screenshots

### 📊 Page 1 — Summary
![Summary Page](screenshot_summary.png)

> High-level KPIs with Good Loan vs Bad Loan breakdown and Loan Status table.

---

### 🗺️ Page 2 — Overview
![Overview Page](screenshot_overview.png)

> Monthly trends, US state map, loan purpose breakdown, employee length analysis, term split, and home ownership distribution.

---

### 📋 Page 3 — Details
![Details Page](screenshot_details.png)

> Full drill-through table with individual loan records — ID, purpose, grade, sub-grade, funded amount, interest rate, installment, and received amount.

---

## Features

| Feature | Description |
|---|---|
| 📊 Summary Page | KPI cards — Total Applications (38.6K), Funded ($435.8M), Received ($473.1M), Avg Interest (12%), Avg DTI (13.3%) |
| ✅ Good vs Bad Loan | Good Loan 86.2% ($370.2M funded) vs Bad Loan 13.8% ($65.5M funded) |
| 📉 Loan Status Table | Fully Paid / Charged Off / Current breakdown with MTD and MoM comparisons |
| 📈 Monthly Trend | Line chart showing loan growth from Jan (2.3K) to Dec (4.0K) |
| 🗺️ Geographic Map | Loan distribution across all US states with color intensity |
| 🍩 Term Analysis | 36-month (26.8%) vs 60-month (73.2%) loan term split |
| 👤 Borrower Profile | Segmentation by employment length, purpose, and home ownership |
| 🔍 Details Drill-through | Full individual loan record table with all fields |
| 🎛️ Interactive Slicers | Filter by State, Grade, and Good vs Bad Loan |

---

## Key Metrics & KPIs

| Metric | Value |
|---|---|
| Total Loan Applications | 38,576 |
| Total Funded Amount | $435,757,075 |
| Total Amount Received | $473,070,933 |
| Average Interest Rate | 12.05% |
| Average DTI | 13.33% |
| Good Loan % | 86.2% (33.2K applications) |
| Bad Loan % | 13.8% (5.3K applications) |
| Fully Paid Loans | 32,145 |
| Charged Off Loans | 5,333 |
| Current Loans | 1,098 |
| MTD Funded Amount | $53,981,425 |
| MoM Growth (Applications) | +6.9% |
| MoM Growth (Amount Received) | +15.8% |

---

## File Structure

```
📁 bank-loan-data-insights/
│
├── 📄 README.md                          ← Project documentation
├── 📊 Bank_Loan_Data_Insights.pbit       ← Power BI Template file
├── 🖼️ screenshot_summary.png             ← Summary dashboard screenshot
├── 🖼️ screenshot_overview.png            ← Overview dashboard screenshot
└── 🖼️ screenshot_details.png             ← Details dashboard screenshot
```

---

## Getting Started

### Prerequisites

- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) — Free download from Microsoft
- Windows 10 / 11
- Your loan dataset in CSV, Excel, or SQL Server format

### Step 1 — Clone or Download

```bash
git clone https://github.com/withjayant/bank-loan-data-insights.git
```

Or click **Code → Download ZIP** on this page.

### Step 2 — Open the Template

1. Launch **Power BI Desktop**
2. Go to **File → Open → Browse**
3. Select `Bank_Loan_Data_Insights.pbit`
4. Power BI will prompt you to connect a data source

### Step 3 — Connect Your Data

- **CSV/Excel**: Go to Transform Data → Data Source Settings → browse to your file
- **SQL Server**: Enter server name, database, and credentials

### Step 4 — Refresh

Click **Home → Refresh** — all 3 pages will populate with your data automatically.

---

## Implementation Strategy

- 🎨 Each dashboard is crafted with an **intuitive layout** to ensure seamless navigation and interaction
- 🔄 Integrated with **real-time data** for up-to-the-minute analysis and decision-making
- 💬 Incorporates **user feedback mechanisms** to continually refine and enhance dashboard functionalities

---

## Data Model

| Column | Data Type | Description |
|---|---|---|
| `id` | Integer | Unique loan identifier |
| `loan_amount` | Decimal | Total loan amount |
| `funded_amount` | Decimal | Amount actually funded |
| `interest_rate` | Decimal | Annual interest rate (%) |
| `installment` | Decimal | Monthly payment |
| `grade` | Text | Loan grade (A–G) |
| `sub_grade` | Text | Sub-grade (A1–G5) |
| `emp_length` | Text | Employment length |
| `home_ownership` | Text | RENT / OWN / MORTGAGE |
| `annual_income` | Decimal | Borrower annual income |
| `loan_status` | Text | Fully Paid / Charged Off / Current |
| `purpose` | Text | Loan purpose |
| `dti` | Decimal | Debt-to-income ratio |
| `addr_state` | Text | US state code |
| `issue_date` | Date | Loan issue date |
| `total_payment` | Decimal | Total payment received |

---

## Requirements

| Requirement | Version |
|---|---|
| Power BI Desktop | March 2023 or later |
| Operating System | Windows 10 / 11 |
| RAM | 4 GB minimum, 8 GB recommended |

---

## Contributing

Contributions are welcome!

1. Fork this repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit: `git commit -m "Add: description of change"`
4. Push to your fork: `git push origin feature/your-feature-name`
5. Open a **Pull Request** on GitHub

Please keep report pages clean, well-labeled, and consistent with the existing visual style.

---

## License

This project is licensed under the **MIT License**.
You are free to use, modify, and distribute this template for personal or commercial purposes with attribution.

---

## 🙋 Questions?

If you run into any issues:
- Open an **Issue** on this GitHub repository
- Describe what you were trying to do and any error messages you saw

---

*Built with ❤️ using Microsoft Power BI*
