 

# Project-Drone — AQI Analysis & Mapping

## Overview

This repository contains data, analysis notebooks, and mapping resources used to explore air quality (AQI) across Indian cities. The notebooks demonstrate data cleaning, exploratory data analysis, comparison of methods, and simple modeling experiments.

## Repository structure

- `AQI/` — Jupyter notebooks for cleaning, EDA, analysis comparison, and modeling.
- `datasets/` — CSV data files (city-level measurements and cleaned variants).
- `mapping/` — Mapping notebook and generated HTML map (`india_aqi_map (1).html`).
- `requirements.txt` — Python package dependencies.

## Key files

- `AQI/data-cleaning-imputation.ipynb` — Data cleaning and imputation steps.
- `AQI/data-eda.ipynb` — Exploratory data analysis and visualizations.
- `AQI/data-analysis-comparison.ipynb` — Comparative analyses between methods or time periods.
- `AQI/models.ipynb` — Simple modeling experiments on AQI.
- `datasets/city_day.csv` — Raw city-day pollutant measurements (includes PM2.5, PM10, NO2, O3, etc.).
- `datasets/city_day_cleaned.csv` — Cleaned version used by notebooks.
- `mapping/mapping.ipynb` — Produces interactive maps; see `mapping/india_aqi_map (1).html`.

## Datasets

- `city_day.csv` — Original daily pollutant readings per city (may contain missing values).
- `city_day_cleaned.csv` — Cleaned and preprocessed data used by the notebooks.
- `city_day_with_coordinates.csv` — City-level coordinates useful for mapping.
- `city_aqi_mapping_data.csv` — Aggregated data prepared for map visualizations.

If you use or redistribute the datasets, please verify and cite the original data source.

## Requirements

Install dependencies in a virtual environment:

```bash
python -m venv .venv
.
# Windows
.venv\Scripts\activate
pip install -r requirements.txt
```

## How to run

1. Open a terminal and activate the Python environment.
2. Install requirements (see above).
3. Start Jupyter Notebook or JupyterLab:

```bash
jupyter lab
# or
jupyter notebook
```

4. Recommended notebook order:
	- `AQI/data-cleaning-imputation.ipynb`
	- `AQI/data-eda.ipynb`
	- `AQI/data-analysis-comparison.ipynb`
	- `AQI/models.ipynb`
	- `mapping/mapping.ipynb` (to generate the HTML map)

Notes:
- Notebooks expect the `datasets/` directory to be present next to the notebooks.
- Some visualizations may require an interactive environment (JupyterLab or a browser).

