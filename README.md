# TCS Data Visualization Project: Online Retail Sales Analysis

## Project Overview
This repository documents the TCS Data Visualization Virtual Simulation. The project's goal was to act as a **Data Visualization Analyst** for a simulated Online Retail client, transforming raw sales data into **actionable business intelligence** for executive review.

---

## Technical Verification and Achievements

The included files serve as technical proof for the claims made on the accompanying resume:

### Dashboard Delivery
The core deliverable was a suite of **Power BI dashboards** focused on **CEO/CMO views** (available in the included PDF/PBIX files). Analysis covered key areas like Monthly Revenue Trends and Top Customer/Geographic Performance.

### Data Integrity (Power Query)
**Critical data cleaning** was performed in **Power Query** to ensure data reliability. This transformation included filtering for valid transactions (**Quantity $\ge 1$** and **Unit Price $ > 0$**) to remove errors and returns, as required by the task. The exact cleaning steps are documented in **`# Data Transformation and Cleaning Logic.md`**.

### Robust Measures (DAX)
A **Robust Revenue measure** was created using **DAX**. This calculation relies on the pre-cleaned data to guarantee accurate financial totals. The specific DAX formula is provided in **`DAX_Measures.txt`**.

---

## Files Included
* **`Online_Retail_Dashboard_Analysis.pbix`**: Working Power BI source file.
* **`DAX_Measures.txt`**: Technical proof of DAX calculations.
* **`# Data Transformation and Cleaning Logic.md`**: Documentation of Power Query steps.
