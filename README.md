# 🏥 Healthcare Claims Revenue Analytics — Python + SQL + Power BI

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![SQL](https://img.shields.io/badge/SQL-pandasql-orange)
![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📌 Overview

End-to-end healthcare claims analysis on **1,000 insurance claims** using
Python for data cleaning and SQL for analysis, with results delivered through
an interactive **2-page Power BI dashboard**.



## 🎯 Business Problem

Healthcare providers face revenue loss from:
✅  High claim denial rates
✅  Unresolved Accounts Receivable
✅  Billing and authorization errors

**This project answers:**
1. What is the denial rate and what drives it?
2. Which insurance types show the highest revenue gap?
3. Which AR statuses represent the most money at risk?
4. How do claim volumes and revenue trend month over month?

---

## 📂 Dataset — 1,000 Claims × 15 Columns

| Column | Type | Description |
|--------|------|-------------|
| Claim ID | Text | Unique identifier |
| Provider ID | Text | Healthcare provider |
| Patient ID | Text | Patient identifier |
| Date of Service | Date | When service was rendered |
| Billed Amount | Numeric | Amount billed by provider |
| Allowed Amount | Numeric | Amount approved by payer |
| Paid Amount | Numeric | Amount actually paid |
| Insurance Type | Category | Medicare/Medicaid/Commercial/Self-Pay |
| Claim Status | Category | Paid/Denied/Under Review/Pending |
| Reason Code | Text | Reason for denial or adjustment |
| AR Status | Category | Open/Closed/Pending/On Hold |
| Outcome | Category | Paid/Denied/Partially Paid |
| Follow-up Required | Boolean | Yes/No |

---

## 🛠️ Tech Stack

| Tool | Role |
|------|------|
| Python + Pandas | Data loading and cleaning |
| pandasql | SQL queries on DataFrames |
| Jupyter Notebook | Analysis environment |
| Power BI Desktop | Interactive dashboard |
| Power BI Web | Publishing and sharing |
| GitHub | Version control and documentation |

---

## 🔄 Workflow

```
claim_data.csv → Python (clean) → SQL (analyze) → 8 CSVs → Power BI → Dashboard
```

---

## 📊 Dashboard Pages

### Page 1 — Executive Overview
![Overview](dashboard/dashboard_overview.png)

### Page 2 — Denial Analysis & Financial & AR Analysis
![Denials](dashboard/dashboard_denials.png)

---

## 💡 Key Findings

- **Denial Rate**: 32.8% of claims denied (industry avg ~15%)
- **Revenue Gap**: $96,437.00 uncollected 
- **Top Denial Reason**: Authorization not obtained (14.6% of denials)
- **Highest AR Risk**: Open status holds $18,300 at risk
- **Lowest Collection Rate**: Self-Pay insurance type

---

## 📁 Repository Structure

```
├── data/                  → raw input data
├── powerbi_data/          → cleaned CSVs loaded into Power BI
├── notebook/              → Jupyter notebook (Python + SQL)
├── dashboard/             → Power BI screenshots
└── README.md
```

---

## 🚀 How to Reproduce

```bash
# Clone repo
git clone https://github.com/Deeksha-bhadoria/Revenue-analytics.git

# Install dependencies
pip install pandas pandasql jupyter

# Run notebook
jupyter notebook notebook/claims_analysis.ipynb


---

## 👤 Author
**Deeksha Bhadoria** | www.linkedin.com/in/deeksha-bhadouria-03 | [GitHub](https://github.com/Deeksha-bhadoria)
