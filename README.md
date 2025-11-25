# Healthcare Claims Data Analysis

## Project Description

Analysis of healthcare claims data from Stony Brook University Hospital (May 2024) to investigate billing patterns, diagnoses, procedures, and payer relationships. This project displays relational data analysis skills applicable to healthcare analytics and revenue cycle management.

## Data Source

Three interconnected CSV files:
- **HEADER**: One row per claim (provider details, dates, payers)
- **LINE**: One row per service line (procedure codes and costs).
- **CODE**: The diagnosis codes (ICD-10) for each claim

Files are connected by 'ProspectiveClaimId'. Data files are not included in the repository (see '.gitignore').

## How to Run

1. **Clone and setup:**
   ```bash
   git clone https://github.com/yourusername/claims-analysis.git
   cd claims-analysis
   pip install -r requirements.txt
   ```

2. **Add data files to `data/` directory:**
   - `STONYBRK_20240531_HEADER.csv`
   - `STONYBRK_20240531_LINE.csv`
   - `STONYBRK_20240531_CODE.csv`

3. **Run notebook:**
   ```bash
   jupyter notebook notebooks/claims_analysis.ipynb
   ```

## Key Findings

- The top 5 providers account for the majority of billing activity. 
- The primary payer mix is dominated by a few major insurers. 
- The most prevalent procedures and diagnoses represent the hospital's main service lines.
- Average of X diagnosis codes and Y service lines per claim.
- Charges vary significantly amongst payers.

## Required Libraries

```
pandas>=1.3.0
matplotlib>=3.4.0
seaborn>=0.11.0
```

Install with: `pip install -r requirements.txt`

## Repository Structure

```
claims-analysis/
├── README.md
├── requirements.txt
├── data/              (CSV files - not in repo)
└── notebooks/
    └── claims_analysis.ipynb
```
