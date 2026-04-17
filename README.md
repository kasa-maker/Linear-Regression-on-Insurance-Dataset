# Medical Insurance Cost Prediction 🏥💵

## Overview
This project uses a **Multiple Linear Regression** model to predict the medical insurance costs billed to a patient based on their health and demographic data. 

## Author
**Kasaam Ali**

## Dataset & Preprocessing
* **Features:** Age, Sex, BMI, Children, Smoker status, and Region.
* **Target Variable (`y`):** `charges` (Medical bills).
* **Data Cleaning:** * Handled duplicate records.
  * Mapped categorical data (`sex`, `smoker`) into binary integers (1/0) using Lambda functions and mapping.
  * Applied **One-Hot Encoding** (`pd.get_dummies`) on the 'region' column for model compatibility.

## Performance Metrics
The model generalized perfectly without overfitting, yielding the following results:
* **Training R-squared:** 0.736
* **Testing R-squared:** 0.772 (77.2% variance explained)

## Technologies Used
* Python, Pandas, Scikit-Learn (Linear Regression, train_test_split, metrics)
