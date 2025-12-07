# Random-Forest-Regression-for-Predictive-Maintenance
### Predicting the Remaining Useful Life using Random Forest Regression

This project was developed as part of the course **'Projektstudium'** at **OTH Regensburg**.

It's goal is to use **Random Forest Regression** to predict the **Remaining Useful Life (RUL)** of machines baased on historical sensor data as well as malfunction logs.

---

### Overview

The project includes:
- Data loading and pre-processing
- Exploratory data analysis (EDA)
- RUL calculation
- Model development using a Random Forest Regressor
- Evaluation of model performance
- Discussion of results and practical implications

---

### Dataset

The dataset used in this project is available on Kaggle:

https://www.kaggle.com/datasets/arnabbiswas1/microsoft-azure-predictive-maintenance?select=PdM_errors.csv

(Note: Because of it's large size, the dataset “PdM_telemetry.csv” contained in this repository is a smaller subset of the original dataset. The complete dataset (on which the random forest model was trained) is available at the specified Kaggle link.) 

---

### Technologies Used
- Python
- Jupyter Notebook
- pandas
- numPy
- matplotlib
- scikit-learn

---

### Project Steps

**1. Data Loading, Pre-processing & EDA**
- Importing and merging datasets
- Handling missing values
- Exploratory analysis to understand the data

**2. Calculating the Remaining Useful Life (RUL)**
Since the RUL is not provided as part of the dataset, it is computed as follows:

RUL = time of the next malfunction - current time

**3. Random Forest Regression**
- Feature selection and engineering
- Splitting the dataset into a test- and train-set
- Model training using `RandomForestRegressor`
- Model evaluation using the metrics R² (R-squared) and MAE (Mean average error)

---

