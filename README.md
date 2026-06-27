# Power-BI_Excel_AeroCost_PPV_CostOut_Analytics
PPV bridge and Cost Out pipeline analytics for aerospace procurement — Excel/VBA, Power BI


## AeroCost: PPV & Cost Out Analytics for Aerospace Procurement

A end-to-end supply chain financial analytics project simulating the monthly PPV reporting and Cost Out pipeline tracking workflow for an aerospace procurement function — built in Advanced Excel with VBA Macros and Power BI.  

## Project Overview

Supply Chain Financial Analysts at aerospace companies like Eaton track two core financial metrics every month:   

  * PPV (Purchase Price Variance) — the difference between what was budgeted to pay for parts and what was actually paid, multiplied by quantity received  
  * Cost Out — structured savings initiatives tracked through a pipeline from identification to realization

This project replicates that end-to-end monthly reporting workflow across a synthetic dataset of 319 receipt transactions, 30 aerospace parts, 10 suppliers, and 12 cost-out initiatives spanning 12 months (Jul 2025 – Jun 2026).  

## Business Questions Answered

Q. Are we paying more or less than standard cost?  
A: PPV Calculation sheet + Power BI Page 1 

Q. Which commodity categories are driving unfavorable variance?  
A: PPV by Category summary + Power BI Page 1  

Q. Is variance improving or worsening month over month?  
A: Monthly PPV trend line — Power BI Page 1  

Q. How much of our Cost Out target have we delivered?    
A: Cost Out Pipeline sheet + Power BI Page 2  

Q.Which initiatives are stuck and at what stage?  
A: Pipeline Stage funnel — Power BI Page 2  

Q: Which suppliers are underperforming on delivery?  
A: Supplier SCM Performance sheet + Power BI Page 3  

Q. Are we paying suppliers on time vs agreed terms?  
A: DPO Variance analysis — Power BI Page 3  

Q. Which suppliers represent concentration risk?  
A. Spend treemap — Power BI Page 3  

## Dashboard Preview

### Page 1 — PPV Summary
<img width="1322" height="746" alt="PPV" src="https://github.com/user-attachments/assets/8d778465-2c1c-4994-83dd-cd4962bf799d" />


### Page 2 — Cost Out Pipeline
<img width="1327" height="737" alt="Cost-out" src="https://github.com/user-attachments/assets/930046e9-2da3-4f05-826d-b61c37fc5a02" />


### Page 3 — Supplier SCM Performance
<img width="1327" height="737" alt="SCM" src="https://github.com/user-attachments/assets/457c439e-adbd-4704-b612-c0a942135967" />


## Excel Workbook —
319 receipt transactions across 30 parts, 10 suppliers, and 12 months. Each row represents one part receipt from one supplier in one month, with Standard Cost vs Actual Price — the raw input for PPV calculation.  

### VBA Macro — Import Monthly Receipts

The workbook includes a production-style VBA macro that automates the monthly data consolidation process.

**What it does:**
    * Opens a file picker for the analyst to select the new month's ERP export file  
    * Validates column headers match the expected schema before importing  
    * Checks for duplicate months — warns if data for that month already exists  
    * Appends only the data rows (paste values, no formulas) to Raw Receipts  
    * Confirms rows added and month imported via dialog box  

## SOP Document
  * Data import via VBA macro  
  * PPV validation checks before publish  
  * Cost Out initiative status update process  
  * Supplier SCM metrics review  
  * Power BI dashboard refresh and stakeholder distribution  

Includes KPI alert thresholds and escalation procedures — structured per ISO documentation standards.

## Key Findings from the Dataset

* **Overall PPV:** Total actual spend exceeded standard cost by approximately $49,000 across 12 months (unfavorable), driven primarily by Machined Components and Raw Materials categories  

 * **Cost Out delivery:** 12 initiatives targeting $753,574 in combined annual savings — 44.5% achieved to date ($335,599 realized). 5 initiatives Fully Realized, 3 In Progress, 4 Approved but not yet started   

* **Supplier performance:** Titan Forge & Cast Inc and Meridian Precision Tools are consistent OTD underperformers (below 85% threshold)  

* **Spend concentration:** Top 3 suppliers represent the majority of total procurement spend — concentration risk flagged in treemap visual  

* **DPO:** Several suppliers show actual payment days exceeding agreed terms by more than 5 days — AP process improvement opportunity


**The dataset, supplier names, part numbers, and financial figures are entirely synthetic and created for demonstration purposes only.**






