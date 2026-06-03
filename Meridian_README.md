# Budget Anomaly Investigation — Meridian Solutions Group
## Internal Financial Forensics Report

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![pandas](https://img.shields.io/badge/pandas-Data%20Analysis-150458?logo=pandas)
![Excel](https://img.shields.io/badge/Excel-Audit%20Report-217346?logo=microsoft-excel)
![Tableau](https://img.shields.io/badge/Tableau-Dashboard-1F6FA4?logo=tableau)

---

## Scenario

> *"The Operations Department budget is over 20% without an approved variance request. My supervisor wants me to investigate — in case it's tampering, stealing, embezzlement, or unethical behavior."*

This project simulates a real-world internal forensic investigation. The Operations Department at Meridian Solutions Group (a fictional mid-size consulting firm) has been running 23.4% over budget for 14 consecutive months with no approved variance on file. The Director of Finance has tasked a data analyst with finding out why.

---

## What the Investigation Found

**$345,637** in unexplained expenditure traced to a single ghost vendor: **Apex Facility Services LLC** (V-2023-0891), added to the system by **Marcus Webb** (Operations Manager) in January 2023.

Every one of the 38 invoices is structured between **$8,536 and $9,789** — consistently below the **$10,000 dual-approval threshold**. Marcus Webb added the vendor and serves as the sole approver for all Operations invoices. No W-9, no contract, no supporting documentation.

The pattern is consistent with a **fictitious vendor scheme** — the most common form of accounts payable fraud per the ACFE 2024 Global Fraud Report.

---

## Investigation Framework

| Phase | Analysis | Key Finding |
|---|---|---|
| 1 | Budget Variance Analysis | Operations is the only dept averaging >20% over budget |
| 2 | Temporal Pattern Analysis | Variance begins Jan 2023 — same month ghost vendor added |
| 3 | Transaction Deep Dive | Ghost vendor represents 46% of total OPS spend in period |
| 4 | Vendor Analysis | No W-9, no contract, no verifiable business existence |
| 5 | Fraud Indicators | 10/10 ACFE red flags present — 3 Critical, 3 High, 4 Medium |
| 6 | Findings & Recommendation | Escalate to HR and Legal; freeze vendor; preserve evidence |

---

## Deliverables

### 1. Jupyter Notebook (`budget_anomaly_investigation.ipynb`)
Six-phase investigation documented in Python:
- Budget variance analysis across all 8 departments
- Timeline reconstruction of when anomaly began
- Invoice distribution analysis showing structuring pattern
- Vendor cross-reference and self-approval audit
- ACFE fraud indicator scorecard
- Formal investigation findings memo

### 2. Excel Audit Report (`Meridian_Budget_Investigation_Report.xlsx`)
Five-sheet workbook formatted for stakeholder distribution:

| Sheet | Contents |
|---|---|
| **Investigation Summary** | Trigger, financial exposure, full fraud indicator scorecard, recommendation |
| **Budget vs Actual** | All 8 departments × 26 months — color-coded variance status |
| **Flagged Transactions** | All 38 ghost vendor invoices with evidence annotations |
| **Vendor Analysis** | Vendor master with documentation status and spend totals |
| **Remediation Actions** | 10 prioritized actions with owner, timeline, and status fields |

### 3. Tableau Dashboard
Three-panel dashboard:
- Budget vs Actual trend by department
- Ghost vendor invoice timeline and cumulative exposure
- Invoice clustering below approval threshold (structuring visualization)

---

## The Fraud Pattern Explained

**Invoice structuring** is the deliberate splitting or sizing of transactions to stay below an approval threshold — in this case $10,000. It's the same concept as financial structuring (smurfing) in money laundering, applied to internal accounts payable.

The ACFE reports that asset misappropriation via fictitious vendor schemes:
- Accounts for 89% of occupational fraud cases
- Has a median loss of $120,000
- Takes an average of 14 months to detect without automated controls

In this scenario, the detection took exactly 14 months — and only because the budget variance finally crossed the 20% investigation trigger.

**The systemic fix** is not just catching Marcus Webb. It's closing the control gap: dual approval for vendor additions, W-9 required before first payment, and automated variance alerts at 10% (not 20%).

---

## Fraud Red Flags Identified

All 10 ACFE red flags from the fictitious vendor framework are present:

🔴 **Critical (3):** Invoice structuring below threshold | Vendor added and approved by same employee | No W-9 on file

🟠 **High (3):** No contract documentation | Anomaly starts at specific date and persists | Disproportionate vendor spend (46% of dept)

🟡 **Medium (4):** Vague invoice descriptions | No supporting work orders | Single approval chain | Variance exceeds investigation trigger

---

## Synthetic Data Note

All company names, employee names, vendor names, and financial figures are entirely fictional and generated synthetically for portfolio purposes. The fraud patterns are modeled on documented real-world cases from ACFE literature and public enforcement actions.

---

## Author

**Alejandro (Alex) Molina**
GitHub: [@chooseyourtacoday](https://github.com/chooseyourtacoday)
Location: Dallas–Fort Worth, TX
Certifications: Codecademy BI Data Analyst | Databricks Analyst Associate (In Progress)
