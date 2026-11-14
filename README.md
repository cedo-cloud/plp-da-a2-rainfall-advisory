# Kenya Rainfall Analysis - Planting Advisory

One year of monthly rainfall for five counties (Machakos, Kitui, Makueni, Nairobi, Kisumu) is
cleaned with a specific `except ValueError`, loaded into a 5 x 12 NumPy array, and summarised into
annual totals, monthly averages, wettest months, dry-month counts and planting windows using
vectorised operations. The notebook writes `rainfall_summary.csv` (one row per county) and ends
with a Planting Advisory and Data Quality Notes.

## How to run

1. `pip install -r requirements.txt`
2. `jupyter notebook rainfall_analysis.ipynb` - or upload the notebook to Colab.
3. Run All, top to bottom. `rainfall_summary.csv` is written to the notebook's own folder
   (`/content` on Colab). No external data file is needed: the raw readings are in the second cell.

## Planting Advisory

- Machakos, Makueni, Nairobi and Kisumu should plant with the long rains in **March-April**, because
  both months clear 100 mm and April is the wettest month in all four, so land preparation must be
  finished by early March.
- Kitui should wait for the short rains in **November-December**, because its Oct-Dec total (358 mm)
  beats its Mar-May total (302 mm) and no two consecutive long-rain months reach 100 mm.
- This is planning guidance from a single year of data, not a forecast: three Machakos months were
  imputed, and the semi-arid counties spend five to six months below 50 mm, so drought-tolerant
  varieties and moisture conservation matter more than the exact planting date.

## Files

- `rainfall_analysis.ipynb` - cleaning, analysis, advisory.
- `rainfall_summary.csv` - generated output, 5 rows.
- `requirements.txt` - dependencies.