# Airline Satisfaction Regression Analysis

## Overview
This project explores airline passenger satisfaction using a machine learning regression-style workflow. It loads survey data, preprocesses mixed categorical and numeric features, and evaluates a Random Forest regressor on a satisfaction target. This repository is preserved as an earlier modeling experiment related to the more polished airline satisfaction classification projects.

## Motivation
The project demonstrates experimentation with preprocessing pipelines, feature encoding, and model evaluation on tabular survey data. It is useful as a learning artifact because it shows the difference between framing satisfaction as a regression problem and framing it as classification.

## Dataset
- **Source:** Kaggle Airline Passenger Satisfaction dataset.
- **File:** `data/airline_satisfaction.csv`
- **Target variable:** `satisfaction`.
- **Important features:** demographic fields, travel type, cabin class, flight distance, delay fields, and service ratings.
- **Dataset size:** TODO: add dataset size after rerunning notebook.
- **Known limitations:** The target is categorical, so regression is not the most natural final framing.

## Methods
- Loaded the airline satisfaction dataset.
- Dropped missing values.
- Split features and target.
- Applied one-hot encoding to categorical variables.
- Trained a Random Forest regressor.
- Evaluated with mean squared error and R-squared.

## Results
The notebook reports:

- Mean Squared Error: **0.05**
- R-squared: **0.81**

## Key Insights
- The dataset has strong predictive signal from passenger service ratings.
- Regression can produce a reasonable numerical fit, but classification is a clearer formulation for this target.
- This repo is best viewed as an intermediate experiment rather than the final airline satisfaction project.

## Limitations
- Regression is not ideal for a categorical satisfaction label.
- The notebook does not yet include cross-validation.
- The project overlaps with other airline satisfaction repos.
- Results should be compared with the classification-based version before drawing conclusions.

## Future Improvements
- Convert the modeling objective fully to classification.
- Add cross-validation and feature importance.
- Link this repo clearly to the stronger airline satisfaction repos.
- Consider archiving this repo after the best version is pinned.

## How to Run
```bash
git clone https://github.com/BobbY-24/Airline-Satisfaction-Satisfaction-Prediction-Model---Data-Analysis-ML-Model-Fitting-.git
cd Airline-Satisfaction-Satisfaction-Prediction-Model---Data-Analysis-ML-Model-Fitting-
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook notebooks/airline_satisfaction_analysis.ipynb
```
