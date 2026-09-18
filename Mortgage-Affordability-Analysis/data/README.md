# Data

## Raw inputs

- `zhvi.csv`: Zillow home value data loaded by the analysis notebook.
- `County_zhvi.csv`: additional county Zillow source file retained from the original repository; the notebook uses `zhvi.csv`.
- `MORTGAGE30US.xlsx`: original mortgage-rate spreadsheet retained for reference; the notebook uses the CSV.
- `mortgage30us.csv`: Freddie Mac / FRED weekly 30-year fixed mortgage rates.
- `saipe_2015.txt` through `saipe_2024.txt`: annual Census SAIPE fixed-width income estimates.

Keep source files in `raw/`. The notebook reads these files without modifying them.

## Processed outputs

The notebook exports these tables to `processed/` for the Tableau dashboard:

- `affordability_trends.csv`: annual affordability summary.
- `county_affordability_changes.csv`: county-level changes over the study period.
- `growth_comparison.csv`: growth comparisons for income, home values, and payments.
- `top_10_deterioration.csv`: counties with the largest affordability deterioration.

Running the notebook replaces these exported files. See the main README and notebook for methods, model assumptions, and limitations.
