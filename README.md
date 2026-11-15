# COSC 74 Final Project: Predicting Housing Competition and Analyzing the Influence of Demographics Beyond the Market

By Linus Law and Anthony Piotrowski

**Task:**
Train CatBoost models to predict monthly average Sale-to-List ratio based on the month's housing market factors and/or the demographic data of the specific zip code it is in.

**Research Question:**
How much does demographic data impact predictions of housing market competition? Does Zip Code function as a proxy for demographic data or does it encode additional spatial/geographic information as well?

## Datasets

We trained CatBoost models on five different datasets:

- Redfin data only (no zip code)
- Redfin data + zip code
- Redfin data + census data
- Redfin data + census data + zip code
- Census data only

Data is from Redfin (2023–2026) and the US Census 5-year estimate (2020–2024).

## Running the Notebooks

All Jupyter notebooks were run in Google Colab, so you may need to add the relevant files to the runtime if you want to run them.

## Notebooks

- `Census Getter.ipynb` – Downloads Census data from the API
- `Redfin Getter.ipynb` – Downloads Redfin data from the API
- `Data Processing.ipynb` – Processes the data and creates the final datasets
- `Heatmaps.ipynb` – Creates heatmaps of the data
- `Linear Regression Baseline.ipynb` – Creates a linear regression baseline model
- `ZipCode Tree Ensemble Tuning.ipynb` – Tunes CatBoost models for datasets with Zip Code
- `ZipCode-less Tree Ensemble Tuning.ipynb` – Tunes CatBoost models for datasets without Zip Code
- `Tree Training and Evaluation.ipynb` – Trains and evaluates CatBoost models
