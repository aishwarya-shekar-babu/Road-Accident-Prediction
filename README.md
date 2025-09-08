# 🚦 Machine Learning Prediction of Road Accident Severity

This project predicts the severity of road accidents in the UK using urban factors, weather, and vehicle data. The main goal is to **identify high-risk accidents** and prioritize detection of severe or fatal cases.  

##  Project Overview

- **Goal:** Predict accident severity — Slight vs Severe/Fatal  
- **Focus Metric:** Recall (maximize detection of serious/fatal accidents)  
- **Dataset:** UK Road Safety Data (STATS19)  obtained via [Kaggle]([https://www.kaggle.com/](https://www.kaggle.com/datasets/tsiaras/uk-road-safety-accidents-and-vehicles).
- **Size:** ~1.9 million records  
- **Environment:** Python (Google Colab)  

## Dataset Details

- **Source**: [UK Department for Transport (DfT)]([https://www.gov.uk/government/statistical-data-sets/road-accidents-and-safety-statistics-data-tables](https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-accidents-safety-data)
- **Accident Data:** `Accident_Information.csv`  
- **Vehicle Data:** `Vehicle_Information.csv`  
- **License:** UK Open Government Licence (OGL)  

### Key Features

**Accident-level:** Severity, Weather, Lighting, Urban/Rural, Road Surface, Road Type, Date & Time, Location  
**Vehicle-level:** Vehicle Type, Engine Capacity, Vehicle Age, Driver Age & Sex, Vehicle Hand Drive  

**Processing:** Datasets merged on `Accident_Index`; missing values handled; categorical encoding applied.  

## Methodology

1. Merge accident and vehicle datasets  
2. Clean and preprocess data: handle missing values, remove redundant columns, engineer features  
3. Encode categorical variables (label encoding and one-hot encoding)  
4. Balance classes via downsampling for fair model training  
5. Train machine learning models: Logistic Regression, Random Forest, XGBoost, Multilayer Perceptron (MLP)  
6. Evaluate models using **recall, F1-score, ROC AUC, confusion matrices, and precision-recall curves**  

##  Interactive Input Window

A small interface allows users to test accident severity predictions using custom inputs.

**Adjustable Inputs:**

- Casualties, Vehicles, Hour, Month, Year, Day of Week  
- Road Type, Speed Bin, Urban/Rural, Weather, Lighting, Surface, Season, Time of Day  
- Driver Age, Sex, IMD Decile  
- Vehicle Type, Left-Hand Drive, Vehicle Age, Engine CC  

**Functionality:**

- Enter or select values for accident and vehicle features  
- Click **Predict**  
- Model outputs predicted severity: **Slight, Serious, or Fatal**  

This allows **real-time testing and exploration** of different accident scenarios.  

##  Files
- `dataset`- archive-vehicle.zip,archive.zip are both dataset,you could unzip it and  save  at  **/content/drive/MyDrive/RoadAccidentData/archive/** 
   since it is a large file then please use below commands in colab
#!wget https://github.com/aishwarya-shekar-babu/Road-Accident-Prediction/raw/main/archive.zip -O /content/drive/MyDrive/RoadAccidentData/archive.zip
#!wget https://github.com/aishwarya-shekar-babu/Road-Accident-Prediction/raw/main/archive-vehicle.zip -O /content/drive/MyDrive/RoadAccidentData/archive-vehicle.zip

     
## 🚀 Notebooks  

### Road_Accident_Prediction_finalmodels.ipynb  
- Complete workflow: data loading, preprocessing, exploratory data analysis, feature engineering, model building, training, and evaluation.  
- Use this notebook if you want to see the **entire pipeline** and replicate the results.  

### Road_Accident_Prediction_finalmodels_app.ipynb  
- Interactive application built on top of the trained models.  
- Provides an interface for users to input parameters and get accident predictions.  


##  Notes

- The model focuses on **maximizing recall for severe/fatal accidents**, ensuring these high-risk cases are reliably identified.  
- All data is anonymized and used in accordance with ethical research practices. 
