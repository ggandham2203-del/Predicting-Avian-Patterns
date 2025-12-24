# 🦆 Mallard Presence Prediction using Machine Learning

This repository contains our **Final Data Science (FDS) course project**, which focuses on predicting the presence of **mallard ducks (mallar3)** at backyard feeder sites using observational and habitat data from **Project FeederWatch**, a large citizen-science initiative by the Cornell Lab of Ornithology.

The project demonstrates an end-to-end data science workflow, including data cleaning, feature selection, handling class imbalance, model development, evaluation, and interpretation of results in an ecological context.

---

## 📌 Project Motivation

Understanding bird presence patterns helps support ecological monitoring, conservation planning, and habitat management. Citizen-science datasets provide rich observational data but are often large, noisy, and highly imbalanced.

In this project, we address the following core question:

> **How accurately can mallard presence be predicted using site-level habitat characteristics and observation data?**

Due to the rarity of mallard sightings in the dataset, we focus on evaluation metrics that are meaningful for imbalanced classification problems, particularly **recall** and **ROC-AUC**.

---

## 🧠 Project Overview

- Integrated large observational and site-level habitat datasets  
- Cleaned, standardized, and merged heterogeneous data sources  
- Addressed severe class imbalance using **SMOTE resampling**
- Trained and compared multiple supervised learning models
- Interpreted feature importance with ecological relevance in mind

Our final results show that **tree-based models**, especially **Random Forest**, are well-suited for capturing complex relationships between habitat features and mallard presence.

---

## 📊 Dataset

The data used in this project was obtained from **Project FeederWatch** (Cornell Lab of Ornithology) and covers observations from **2020–2024**.

### Data Sources
- **Observer data**: Bird sightings and observation effort
- **Site description data**: Habitat features, vegetation, feeder availability, and human/animal activity

### ⚠️ Data Availability
Due to GitHub file size limitations, **raw and processed datasets are not included** in this repository.

You can request and download the data from:
> Project FeederWatch – Cornell Lab of Ornithology  
> https://feederwatch.org/explore/raw-dataset-requests/

After downloading, place the files in: data/raw/


---

## 🤖 Models Implemented

The following supervised learning models were trained and evaluated:

- **Logistic Regression** (baseline model)
- **Decision Tree**
- **Random Forest**
- **k-Nearest Neighbors (kNN)**

### Model Evaluation
Because mallard presence is rare, model performance was evaluated using:
- Recall (presence class)
- Precision
- F1-score
- ROC-AUC

**Random Forest** achieved the best overall balance between recall and ROC-AUC, making it the most suitable model for birdwatcher-oriented prediction scenarios where missing a true presence is costly.

---

## 🌿 Key Findings

- Geographic location (latitude and longitude) is the strongest predictor of mallard presence  
- Freshwater habitat availability plays a significant role  
- Vegetation features (deciduous and evergreen trees) contribute meaningfully  
- Human and animal activity variables have relatively lower predictive impact  

These findings align well with known ecological behavior of mallards and demonstrate the value of machine learning for species-distribution modeling.

---

## 📁 Repository Structure
data/
raw/ # (excluded from GitHub; see Data Access section)
processed/ # (excluded from GitHub)
notebooks/
BirdBrains_Preprocessing.ipynb
BirdBrains_Modeling.ipynb
report/
Final_Data_Science_Bird_Brains_Report.pdf
Bird_Brains_Presentation.pptx


---

## 🛠️ Tools & Technologies

- Python  
- pandas, numpy  
- scikit-learn  
- imbalanced-learn (SMOTE)  
- matplotlib  

---

## 👥 Contributors

- **Gayathri Gandham**
- Lynn Jacobs
- Sri Moukthika Aluri
- Jeffrey Cris

---

## 📌 Notes

This project was completed as part of a graduate-level **Final Data Science (FDS)** course and is intended to demonstrate practical data science skills, including handling real-world data challenges such as scale, missing values, and class imbalance.

For detailed methodology, analysis, and discussion, please refer to the full project report included in the `report/` directory.

