# CS316 Project: Solar Power Forecasting

Prince Sultan University, College of Computer and Information Systems
CS316 Introduction to AI and Data Science, Section 1282

Team: Rozana Aljudhy, Deema Alqahtani, Lama Alangari, Layan Alagel

## Project
We predict the AC power of two solar plants from weather and time-of-day data,
and compare two tree-based models: XGBoost and Random Forest.

## Dataset
Solar Power Generation Data (Kaggle, anikannal/solar-power-generation-data):
two plants, 15-minute readings, 15 May to 17 June 2020. The four CSV files
are in the `data/` folder. The original source is Kaggle.

## How to run
1. Open `CS316_project.ipynb` in Google Colab (File > Upload notebook).
2. Choose Runtime > Run all.
3. Libraries used: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost.

## Notebook contents
1. Loading the data
2. Cleaning and preprocessing: date parsing, weather gap filling, merging
3. Feature engineering and memory optimization
4. Exploratory data analysis
5. Model training: XGBoost and Random Forest, chronological 80/20 split
6. Evaluation: MAE, MSE, RMSE, R2, per-plant results, feature importance

## Results
Overall test R2 is about 0.85 for both models. Plant 1 reaches about 0.98
and Plant 2 about 0.62.

## Files
- `data/`: the four dataset files
- `CS316_project.ipynb`: the full pipeline
- `report/`: the project report
