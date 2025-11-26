# Capstone-Project
-Data Analysis of Depression Trends Based on Synthesized Data

-Predicting Depression Risk from Behavioral Data (Initial EDA + Baseline)

## Summary
This repository contains an initial exploratory data analysis and baseline modeling pipeline for my capstone project exploring whether behavioral and lifestyle features can predict depression risk. Because real world human datasets with validated PHQ-9 scores were not available for this stage, a **synthetic dataset** mimicking plausible relationships was generated and used.

### Files
- `data/depression_synth.csv` generated synthetic raw dataset.
- `data/depression_synth_clean_for_modeling.csv` cleaned/imputed dataset used for modeling.
- `outputs/eda_plots.png` EDA visualizations.
- `outputs/roc_curve_logistic.png` ROC for logistic baseline.
- `outputs/rf_perm_importance.png` Random forest permutation importance plot.
- `notebooks/Capstone_EDA_and_Baseline.ipynb` Jupyter Notebook (this repo's main artifact).

## What I did
- Generated a synthetic dataset with features: sleep duration/quality, physical activity, screen time, social media use, nutrition, social interactions, age, education, etc.
- Executed EDA to inspect distributions and relationships.
- Trained a logistic regression baseline and a random forest model.
- Evaluated models with classification reports and ROC AUC.
- Computed feature importance via permutation importance.

## Key preliminary observations
- Features such as sleep quality, physical activity, screen time and social interactions are associated with the synthetic PHQ-9 proxy and model predictions.
- Results are consistent with literature and expectations but must be validated on real data.

## Next steps
- Acquire a human dataset.
- Improve feature engineering and time series features.
- Tune models (GridSearch/Randomized), use calibrated probabilities, and add model explainability.
- Validate clinically work with domain experts.
