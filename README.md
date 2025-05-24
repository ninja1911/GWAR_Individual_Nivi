# H-Predict: Machine Learning-Based Healthcare Cost Estimation

## Overview

H-Predict is a machine learning-based tool designed to estimate treatment costs using patient demographic and medical data. It leverages various regression models to help patients, insurance companies, and healthcare providers understand and plan for healthcare expenses. The project follows a CRISP-DM methodology and is built using Python with open-source libraries.

## Key Features

* **Prediction Targets:** Estimate healthcare treatment costs.
* **Data Sources:** Government-provided hospital discharge records and federal healthcare surveys.
* **Models Used:** Linear Regression, Polynomial Regression, Random Forest, Gradient Boosting Regressor, and XGBoost.
* **Performance Metrics:** MAE, MSE, RMSE, and R-squared.
* **Best Model:** Random Forest (R2 = 0.911), XGBoost performed second-best with computational efficiency.

## Dataset

The dataset combines:

* Federal government healthcare surveys (2021–2023)
* State-level hospital discharge data

After cleaning and merging, the dataset size is approximately 100MB and contains around 1 million records.

## Folder Structure

```
GWAR_Individual_Nivi/
├── Data270_project_Individual_Updated.ipynb      # Final Jupyter notebook
├── README.md                                     # Project summary and details
├── GWAR_Reference_ccs_dcode.csv                 # CCS Diagnosis Code Reference
├── GWAR_Reference_ccs_pcode.csv                 # CCS Procedure Code Reference
├── pickle_models/                               # Contains ML model files
│   ├── Pickle_LR_Model.pkl                       # Linear Regression model
│   ├── Pickle_Poly_Model.pkl                     # Polynomial Regression model
│   ├── xgb_model_data.pkl                        # XGBoost model input data
│   └── xgb_model_results_hyperparameter.pkl      # XGBoost tuned results
```

## Requirements

* Python 3.x
* Libraries: `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `xgboost`, `seaborn`, `plotly`, `jupyter`
* Deployment (optional): Google Cloud Platform (GCP) or similar

## Running the Project

1. Clone the repo:

```bash
git clone https://github.com/ninja1911/GWAR_Individual_Nivi.git
cd GWAR_Individual_Nivi
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook and run the notebook:

```bash
jupyter notebook Data270_project_Individual_Updated.ipynb
```

---

*This project was developed as part of the DATA 270 - Data Analytics Processes course at San Jose State University.*
