# Mallard Presence Prediction using Machine Learning

This repository contains our Final Data Science (FDS) course project focused on predicting the presence of mallard ducks using observational and habitat data from Project FeederWatch.

## Project Overview
We explore whether mallard presence can be predicted using site-level habitat characteristics and observation effort. Due to strong class imbalance, recall and ROC-AUC were emphasized during evaluation.

## Dataset
Data was obtained from **Project FeederWatch (Cornell Lab of Ornithology)** for the years 2020–2024.

> Raw datasets are not included due to size constraints.

## Models Used
- Logistic Regression  
- Decision Tree  
- Random Forest  
- k-Nearest Neighbors (kNN)

Random Forest performed best overall.

## Repository Structure
data/
    raw/
    processed/
notebooks/
    BirdBrains_Modeling.ipynb
    BirdBrains_Preprocessing.ipynb
report/
    Final_Data_Science_Bird_Brains_Report.pdf
    Bird Brains Presentation.pptx


## Contributors
- Gayathri Gandham
- Lynn Jacobs
- Sri Moukthika Aluri
- Jeffrey Cris

## Tools
Python, pandas, numpy, scikit-learn, imbalanced-learn, matplotlib

## Data Access
Due to GitHub file size limitations, raw datasets are not included in this repository.

The data can be obtained from:
Project FeederWatch – Cornell Lab of Ornithology  
https://feederwatch.org/explore/raw-dataset-requests/

After downloading, place the files in:
data/raw/

