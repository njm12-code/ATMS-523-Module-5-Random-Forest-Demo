# Random Forest Rain Rate Activity

An interactive Jupyter notebook activity that demonstrates **Random Forest Regression** with scikit-learn,
predicting **rain rate** from radar-derived parameters.

- **Data**: [radar_parameters.csv](https://github.com/swnesbitt/ATMS-523-Module-5/blob/main/homework/radar_parameters.csv)
- **Goal**: Predict rain rate from the other columns and explore how hyperparameters affect skill.
- **Interactivity**: Sliders to tweak RandomForest hyperparameters and instantly see updated metrics and plots.

## Quick Start

```bash
# (Option A) Using conda/mamba
mamba create -n rf-activity -y python=3.11
mamba activate rf-activity
pip install -r requirements.txt

# Launch
jupyter lab  # or: jupyter notebook
```

Then open `notebooks/01-rf-rainrate-activity.ipynb`.

> If ipywidgets doesn't render sliders, run:
>
> ```bash
> jupyter nbextension enable --py widgetsnbextension
> ```

## What you'll do

- Load the dataset directly from GitHub (or local copy).
- Explore variable relationships (scatter matrix and correlation heatmap).
- Train/test split and baseline.
- Build a **RandomForestRegressor**, adjust sliders for:
  - `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `max_features`
- See **RMSE**, **MAE**, **bias**, and plots:
  - Predicted vs Observed with 1:1 line
  - Residual histogram
  - Feature importances

## File Structure

```
rf-rainrate-activity/
├── LICENSE
├── README.md
├── requirements.txt
├── .gitignore
└── notebooks/
    └── 01-rf-rainrate-activity.ipynb
```

## GitHub Publishing (optional)

```bash
cd rf-rainrate-activity
git init
git add .
git commit -m "Random Forest rain rate activity with interactive sliders"
git branch -M main
git remote add origin YOUR_REPO_URL
git push -u origin main
```
