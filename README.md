# db-unza26-csc4792-chililabombwe

Dataset and scraping notebook for the **CSC 4792 Data Mining and Warehousing** 
mini-project (University of Zambia, 2025/26).

**Assigned Council:** Chililabombwe Municipal Council  
**Project Team:** #11  
**Website:** http://www.chililabombwecouncil.gov.zm

## 📁 Contents

### Data (pipe-separated CSVs)
| File | Description | Rows |
|---|---|---|
| `db-unza26-csc4792-chililabombwe_obb_budget_2024.csv` | 2024 Output-Based Budget | 60 |
| `db-unza26-csc4792-chililabombwe_budget_comparison_2023_2024.csv` | YoY budget growth | 4 |
| `db-unza26-csc4792-chililabombwe_budget_programmes_2025.csv` | 3-year programme budgets | 59 |
| `db-unza26-csc4792-chililabombwe_cdf_projects_2024.csv` | Approved CDF projects | 13 |
| `db-unza26-csc4792-chililabombwe_output_targets_2025.csv` | 2025 output KPIs | 11 |
| `db-unza26-csc4792-chililabombwe_revenue_sources_2025.csv` | Revenue by source | 23 |

### Notebook
- `db-unza26-csc4792-chililabombwe_scraper.ipynb` — Complete Jupyter 
  notebook documenting scraping, extraction, cleaning, and validation.

## 🛠️ Methods

1. **Site reconnaissance** — mapped the council website using `requests` + `BeautifulSoup`
2. **PDF harvesting** — downloaded 46 PDFs from the Council Documents 
   and Publications pages
3. **Diagnostic scan** — classified PDFs into text-based vs. scanned
4. **Table extraction** — `pdfplumber` for text-based PDFs
5. **Manual transcription** — for 1-page scanned CDF projects list
6. **Validation** — extracted totals matched printed totals in source PDFs

## ✅ Verification

| Dataset | Extracted Total | Printed Total | Match |
|---|---|---|---|
| 2024 OBB Budget | K147,958,491 | K147,958,491 | ✅ |
| 2025 Budget Programmes | K222,580,695 | K223,603,854 | 99.5% |

## 📊 Kaggle Dataset

Published at: https://www.kaggle.com/datasets/isaiahchileshe/chililabombwe-municipal-council-data-zambia

## 📄 License

CC BY 4.0

## 👥 Contributors

- Isaiah Chileshe
- [Add group members here]
