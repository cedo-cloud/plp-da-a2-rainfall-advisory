# Rainfall Analysis & Planting Advisory

## Project Summary
This project processes raw monthly rainfall data from five Kenyan counties to identify optimal planting windows for a farmer-support NGO. It cleans malformed data, performs vectorized statistical analysis using NumPy, and outputs a structured summary for SMS advisory distribution.

## How to Run the Notebook
1. Install the required dependencies: `pip install -r requirements.txt`
2. Open `rainfall_analysis.ipynb` in Jupyter Notebook or JupyterLab.
3. Run all cells sequentially to clean the data, perform the analysis, and generate the `rainfall_summary.csv` file.

## Planting Advisory
- Farmers in Nairobi, Nakuru, Kisumu, and Mombasa should target the April–May window for planting, as these months consistently provide the highest consecutive rainfall.
- Machakos farmers should target the November–December window for the highest moisture availability, as its rainfall pattern peaks later in the year.
- Please note that the Machakos dataset contained missing values that were statistically imputed, so local verification of current soil moisture is advised before making critical agricultural decisions.