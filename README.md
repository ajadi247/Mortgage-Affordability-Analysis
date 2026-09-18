# U.S. Mortgage Affordability Analysis

A county-level analysis of how the cost of financing a typical-valued home changed relative to household income from **2015–2024**.

This project combines Zillow home values, Census SAIPE income estimates, and Freddie Mac / FRED mortgage rates for a balanced panel of **2,486 U.S. counties**. It models principal-and-interest payments for a **30-year fixed mortgage with a 20% down payment**.

## Key Findings

- Median county mortgage-payment burden increased from **12.93% of household income in 2015 to 21.84% in 2024**.
- **98.95% of counties** experienced an increase in modeled payment burden.
- Median county growth was **43.8% for household income**, **77.4% for home values**, and **144.7% for modeled mortgage payments**.

Results describe equally weighted counties and exclude taxes, insurance, and other homeownership costs.

## Full Report & Dashboard

- **[Read the full analysis report](Mortgage-Affordability-Analysis/REPORT.md)** for methodology, data preparation, validation, findings, and limitations.
- **[Explore the interactive Tableau dashboard](https://public.tableau.com/views/MortgageAffordabilityFinal/MortgageAffordability)** to view trends and geographic differences.

![Mortgage Affordability Dashboard](images/dashboard.png)

## Repository Structure

```text
Mortgage-Affordability-Analysis/
├── README.md             # Project summary
├── REPORT.md             # Full analysis report
├── requirements.txt      # Python dependencies
├── data/
│   ├── README.md         # Data documentation
│   ├── raw/              # Source datasets
│   └── processed/        # Exported analysis tables
├── notebooks/            # Analysis and validation
├── tableau/              # Tableau workbook
└── images/               # Dashboard screenshot
```

## Run the Analysis

1. Clone the repository.
2. Install dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

3. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `notebooks/housing_analytics_final.ipynb` and run the cells in order.

The notebook exports analysis tables to `data/processed/`.

## Tools & Data Sources

**Tools:** Python, Pandas, Matplotlib, Jupyter Notebook, and Tableau.

**Data sources:** Zillow Home Value Index, U.S. Census Bureau SAIPE, and Freddie Mac / FRED.
