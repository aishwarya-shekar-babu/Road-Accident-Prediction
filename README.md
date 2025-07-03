
# Machine Learning prediction of Road Accident Severity using Urban factors,vehicle data  and Weather conditions

This project explores the use of machine learning techniques to predict the **severity of road traffic accidents** in the United Kingdom. Using a large-scale dataset from the **Department for Transport (DfT)**, the objective is to identify key environmental and temporal factors influencing accident severity. The findings aim to support data-driven road safety policies and targeted interventions.

---

## Project Overview

- **Goal**: Predict accident severity — categorized as *Slight*, *Serious*, or *Fatal*.
- **Dataset**: UK Road Safety data (STATS19), obtained via [Kaggle]([https://www.kaggle.com/](https://www.kaggle.com/datasets/tsiaras/uk-road-safety-accidents-and-vehicles).
- **Size**: ~1.9 million records (~200–400 MB).
- **Environment**: Python in Google Colab, version control via GitHub.

---

## Dataset Details

- **Source**: [UK Department for Transport (DfT)]([https://www.gov.uk/government/statistical-data-sets/road-accidents-and-safety-statistics-data-tables](https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-accidents-safety-data)
- **File Used**: `Accident_Information.csv`
- **Data License**: UK Open Government Licence (OGL)
- **Key Features**:
  - Accident Severity (Target)
  - Weather Conditions
  - Lighting Conditions
  - Urban/Rural Classification
  - Road Surface Conditions
  - Date and Time of Accident

> All data is anonymized and used in accordance with ethical research practices.

---

## Methodology

### Preprocessing

- Data cleaning and feature engineering
- Encoding categorical variables
- Handling missing values
- Class balancing
