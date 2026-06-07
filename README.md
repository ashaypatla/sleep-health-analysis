# Sleep Health Analysis — DSCI 631 Project

## Dataset
This project uses a synthetic sleep health dataset of 100,000 records designed for comprehensive sleep health analysis. Each record represents a unique 
individual's daily snapshot capturing:

- **Sleep Architecture** — duration, quality, REM percentage, deep sleep percentage, sleep latency, and wake episodes
- **Lifestyle Factors** — caffeine intake, alcohol consumption, screen time, exercise, daily steps, and nap duration
- **Demographics** — age, gender, occupation, BMI, and country
- **Psychological State** — stress score and mental health condition
- **Environmental Factors** — room temperature, season, day type, and chronotype

The dataset contains 32 columns and targets two outcome variables:
- `sleep_disorder_risk` — 4 class categorical (Healthy, Mild, Moderate, Severe)
- `cognitive_performance_score` — continuous numeric score

Although synthetic, the statistical distributions and correlations are calibrated against peer-reviewed sources including the CDC National Health 
Interview Survey (2024), Sleep Foundation population studies, and the Framingham Heart Study.

---

## Project Overview

This project applies supervised machine learning techniques to the sleep health 
dataset across two tasks:

### 1. Classification
Predict `sleep_disorder_risk` across four severity classes — Healthy, Mild, Moderate, and Severe. The dataset presents a significant class imbalance 
(54/33/8/4%) which is addressed through preprocessing and modeling decisions. Three classification algorithms are evaluated and compared.

### 2. Regression
Predict `cognitive_performance_score` as a continuous outcome. This task explores the relationship between sleep health, lifestyle factors, and 
next-day cognitive performance using regression models.

---

## Repository Structure

| File | Description |
|---|---|
| `eda.ipynb` | Exploratory data analysis |
| `classification.ipynb` | Classification models and evaluation |
| `regression.ipynb` | Regression models and evaluation |
| `sleep_health_dataset.csv` | Dataset |

---

## Requirements

- pandas
- numpy
- scikit-learn
- imbalanced-learn
- category_encoders
- matplotlib
- seaborn
- xgboost
