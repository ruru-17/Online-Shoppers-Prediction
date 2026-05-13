# Online Shopper Conversion Prediction

Course project for MTL782 Data Mining (IIT Delhi, Spring 2024–25). The goal is to predict whether an online shopping session results in a purchase using session activity features. The evaluation metric is F1-score.

## Contents
- `Non_comp_notebook.ipynb` — non-competitive track (restricted models/feature engineering).
- `Comp_Notebook.ipynb` — competitive track (Kaggle run).
- `Project_Report.pdf` — methodology, experiments, and results.
- `MTL782-A1.pdf` — assignment statement and rules.
- `requirements.txt` — base Python dependencies.

## Data
The dataset is not included in this repository. The notebooks expect the following files from the assignment/Kaggle data:
- `kaggle_train.csv`
- `kaggle_test.csv` (if evaluating on a test set)
- `metadata.txt`

Paths used in notebooks:
- `Non_comp_notebook.ipynb` reads `data/kaggle_train.csv` by default. Place the files under `data/` or update the path.
- `Comp_Notebook.ipynb` uses Kaggle input paths (`/kaggle/input/...`). Update paths when running locally.

## Setup
1. Create and activate a Python environment.
2. Install base requirements:
   ```
   pip install -r requirements.txt
   ```
3. Install notebook tooling (for example, `jupyterlab`) and any extra dependencies needed for the competitive notebook:
   - `xgboost`
   - `imbalanced-learn`
   - `scikit-optimize`

## Running
Open the notebooks in Jupyter and run all cells:
- `Non_comp_notebook.ipynb`
- `Comp_Notebook.ipynb`

## Notes
The competitive notebook was developed on Kaggle and may require path and environment adjustments when run locally. See `Project_Report.pdf` for full methodology and results.
