# GC-MS Results Processing (Google Colab)

A Colab notebook that turns raw GC-MS result exports into clean, comparable compound tables and figures. I built it during food biotechnology research for aroma profiling, so that lab members without a programming background could process their own runs.

![GC-MS processing workflow](https://user-images.githubusercontent.com/55685832/223360864-5404e014-2507-4984-88a6-ce061940cea9.png)

## What it does

- **Cleans exports:** reads `RESULT.CSV` files from the GC-MS data analysis software (RT, Area Pct, Library/ID, CAS, Qual, Area)
- **Filters noise:** removes listed contaminant compounds and harmonises compound IDs/names
- **Identifies compounds** by CAS number and inspects retention times
- **Compares against a reference list** (optional) of known compounds, attributes and classes
- **Compares samples:** occurrence-similarity **heatmaps** and **PCA biplots** across samples, with interactive re-plotting to adjust figure settings

## How to use

1. Open the notebook in Colab and **save a copy to your Drive** (File → Save a copy in Drive) so the original stays unchanged.
2. Prepare each sample: copy the needed columns from `RESULT.CSV` into a new sheet and save it as CSV. Optionally prepare a reference CSV with `Compounds`, `Attribute` and `Class` columns.
3. Edit **Section 2.2 Configuration Setup** (paths, sample list, reference file, contaminants, options).
4. Connect Google Drive when prompted, then run all cells. Outputs are saved to the folder you set.

The notebook's first section is a full user guide, with file preparation steps and plotting tips.

## Tech stack

Python · pandas · NumPy · scikit-learn (PCA) · matplotlib · seaborn · Google Colab

## Author

Navavat Pipatsart, PhD · [LinkedIn](https://www.linkedin.com/in/navavat-pipatsart-6479b6185/)# GC-MS Results Processing (Google Colab)

A Colab notebook that turns raw GC-MS result exports into clean, comparable compound tables and figures. I built it during food biotechnology research for aroma profiling, so that lab members without a programming background could process their own runs.

![GC-MS processing workflow](https://user-images.githubusercontent.com/55685832/223360864-5404e014-2507-4984-88a6-ce061940cea9.png)

## What it does

- **Cleans exports:** reads `RESULT.CSV` files from the GC-MS data analysis software (RT, Area Pct, Library/ID, CAS, Qual, Area)
- **Filters noise:** removes listed contaminant compounds and harmonises compound IDs/names
- **Identifies compounds** by CAS number and inspects retention times
- **Compares against a reference list** (optional) of known compounds, attributes and classes
- **Compares samples:** occurrence-similarity **heatmaps** and **PCA biplots** across samples, with interactive re-plotting to adjust figure settings

## How to use

1. Open the notebook in Colab and **save a copy to your Drive** (File → Save a copy in Drive) so the original stays unchanged.
2. Prepare each sample: copy the needed columns from `RESULT.CSV` into a new sheet and save it as CSV. Optionally prepare a reference CSV with `Compounds`, `Attribute` and `Class` columns.
3. Edit **Section 2.2 Configuration Setup** (paths, sample list, reference file, contaminants, options).
4. Connect Google Drive when prompted, then run all cells. Outputs are saved to the folder you set.

The notebook's first section is a full user guide, with file preparation steps and plotting tips.

## Tech stack

Python · pandas · NumPy · scikit-learn (PCA) · matplotlib · seaborn · Google Colab

## Author

Navavat Pipatsart
