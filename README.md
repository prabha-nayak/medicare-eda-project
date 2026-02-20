# medicare-eda-project

# Medicare High-Cost Patient Analysis (2023)

## Project Overview
An exploratory data analysis of 2023 CMS Medicare Part A and Part B data 
to identify high-cost patient populations across geographic, demographic, 
and clinical dimensions.

**[View Interactive Tableau Dashboard](YOUR_TABLEAU_URL_HERE)**

---

## Key Findings
- **New York** has the highest Medicare spend per enrollee at $14,140 - 
  72% more than Hawaii's $8,221
- **Children under 18** on Medicare cost $60,014 per enrollee - driven 
  by disability and end-stage renal disease qualifications
- **American Indian/Alaska Native** beneficiaries spend 23.9% above the 
  national average - the largest racial disparity in the dataset
- **COVID-19 visibly reduced spending** across all service types in 2020 
  except Hospice, which grew continuously from $19.25B to $25.67B
- **Medicaid dual enrollees** cost more than twice as much as non-dual 
  enrollees ($21,394 vs $10,228)
- **Iowa** has the highest patient cost burden at 21.3% - meaning patients 
  pay 21 cents of every dollar spent on their care

---

## Data Source
Centers for Medicare & Medicaid Services (CMS)  
Medicare Part A and Part B Summary, Calendar Year 2023  
[CMS Medicare Geographic Variation Public Use File](https://data.cms.gov/summary-statistics-on-use-and-payments/medicare-medicaid-spending-by-geography/medicare-geographic-variation-public-use-file)

---

## Tools Used
| Tool | Purpose |
|------|---------|
| Python (Pandas) | Data cleaning and transformation |
| SQLite (via Python) | Data analysis and querying |
| Tableau Public | Interactive dashboard |
| Jupyter Notebook | Documentation and workflow |

---

## Project Structure
```
medicare-eda-project/
  01_data_cleaning.ipynb    ← Data extraction and cleaning
  02_sql_analysis.ipynb     ← SQL queries and findings
  output/                   ← Cleaned CSV files
```

---

## SQL Queries & Insights

| Query | Business Question | Key Finding |
|-------|------------------|-------------|
| Q1 | Top 10 highest cost states | New York: $14,140/enrollee |
| Q2 | Bottom 10 lowest cost states | Hawaii: $8,221/enrollee |
| Q3 | Cost by age group | Under 18: $60,014 (disability) |
| Q4 | Cost by race | AIAN: $14,896/enrollee |
| Q5 | Spending trends 2018-2023 | COVID dip visible in 2020 |
| Q6 | Dual vs non-dual Medicaid | Dual enrollees cost 2x more |
| Q8 | Cost burden by state | Iowa: 21.3% highest burden |
| Q10 | Racial disparity index | AIAN 23.9% above national avg |

---

## How to Run This Project
1. Clone this repository
2. Install dependencies: `pip install pandas openpyxl sqlalchemy`
3. Download the source data from the CMS link above
4. Run `01_data_cleaning.ipynb` first
5. Then run `02_sql_analysis.ipynb`

---

*Analysis by Prabha Nayak | MS Health Informatics, University of San Francisco*
