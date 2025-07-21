# Heart-Failure-Risk-Prediction
This project is a machine learning model that predicts the likelihood of death from heart failure based on clinical records. It aims to support healthcare professionals by offering an intelligent tool for early risk assessment, potentially aiding in timely and life-saving interventions.

A machine learning model that predicts the probability of death due to heart failure using clinical data. Built with Python and XGBoost, this model supports early diagnosis and risk assessment—providing doctors and researchers a tool for smarter, data-informed decisions.

##  What the Model Does

This project uses patient data to identify individuals at high risk of death from heart failure. It:

- Cleans and preprocesses clinical data
- Engineers insightful new features
- Trains an XGBoost classifier
- Predicts whether a patient is likely to experience a fatal event (`1` = Yes, `0` = No)

##  Dataset Overview

The dataset (`heart_failure_clinical_records_dataset.csv`) includes **299 patients** with **13 features** like:

- `age`, `sex`, `smoking`, `diabetes`, `anaemia`
- `serum_creatinine`, `serum_sodium`, `ejection_fraction`
- `platelets`, `creatinine_phosphokinase`
- `high_blood_pressure`, `time`, and `DEATH_EVENT` (target)

###  Feature Engineering

We introduced five custom features to enhance prediction:

- `creatinine_sodium_ratio`
- `cpk_platelet_ratio`
- `anaemia_diabetes`
- `bp_smoking`
- `age_ejection_interaction`

These help the model understand compound clinical effects better.


## Model Performance

After training and evaluation on a stratified 80/20 split:

 **Accuracy**: `~81.67%



