
# Loan Default Prediction and Visualization

## Project Overview

This project aims to predict loan defaults using machine learning models and visualize the results using Power BI. The goal is to identify key factors contributing to loan defaults and create an efficient model to predict outcomes on a production dataset. The predicted dataset is then imported into Power BI for interactive reporting.

---

## Steps Taken

### 1. **Data Collection and Initial Exploration**
   - Imported the dataset: `Raw_Data_Singapore Credit Dataset.csv`.
   - Conducted initial data exploration using `df.head()`, `df.info()`, and `df.describe()`.
   - Checked for missing values and duplicates.
   - Identified categorical and numerical variables.

### 2. **Data Cleaning**
   - Removed unwanted characters from columns (e.g., "SGD" and "years").
   - Checked for and removed duplicate rows.
   - Dropped unnecessary columns (`job` and `phone`) based on low correlation with the target variable.

### 3. **Exploratory Data Analysis (EDA)**
   - Performed univariate analysis:
     - Histograms and boxplots for numerical variables.
     - Count plots and pie charts for categorical variables.
   - Conducted bivariate analysis:
     - Pairplot to visualize relationships between numerical variables.
     - Correlation heatmap for categorical variables using chi-square tests.
   - Identified and analyzed outliers but decided not to remove them to preserve data quality.

### 4. **Data Preprocessing**
   - Encoded categorical variables:
     - One-hot encoding for nominal variables (`checking_balance`, `savings_balance`, `purpose`, `other_credit`, `housing`).
     - Ordinal encoding for `credit_history`.
     - Label encoding for `employment_duration`.
   - Scaled numerical features using `StandardScaler`.

### 5. **Model Training**
   - Split the dataset into training and testing sets using three different ratios: 70/30, 75/25, and 80/20.
   - Trained three supervised machine learning models:
     - Logistic Regression
     - Random Forest
     - Decision Tree
   - Evaluated models using metrics such as accuracy, precision, recall, F1 score, and ROC AUC.

### 6. **Model Evaluation and Selection**
   - Compared the performance of all models across different train-test splits.
   - Selected Logistic Regression as the best model due to its consistent performance and high ROC AUC score.

### 7. **Prediction on Production Data**
   - Loaded the production dataset: `Predict_Data_Singapore Credit Dataset.csv`.
   - Applied the same preprocessing steps (encoding and scaling) to the production dataset.
   - Used the trained Logistic Regression model to predict loan defaults on the production dataset.
   - Added the predicted `default` column to the production dataset.

### 8. **Visualization in Power BI**
   - Exported the predicted dataset to a CSV file: `Predicted_Data_Singapore_Credit_Data.csv`.
   - Imported the dataset into Power BI.
   - Created interactive dashboards to visualize key insights and trends.

### 9. **Final Output**
   - Saved the final predicted dataset for future use.
   - Prepared a presentation in Power BI to showcase the results.

---

## Key Files
- **Raw Dataset**: `Raw_Data_Singapore Credit Dataset.csv`
- **Production Dataset**: `Predict_Data_Singapore Credit Dataset.csv`
- **Predicted Dataset**: `Predicted_Data_Singapore_Credit_Data.csv`
- **Jupyter Notebook**: Contains the entire code for data preprocessing, model training, and evaluation.
- **Power BI Dashboard**: Interactive visualizations of the predicted dataset.

---

## Tools and Libraries Used
- **Python Libraries**:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `scikit-learn` (for machine learning models and evaluation)
- **Power BI**: For data visualization and reporting.

---

## Results
- Logistic Regression achieved the best performance with an accuracy of ~76.7% and an ROC AUC of ~0.81.
- The predicted dataset was successfully visualized in Power BI, providing actionable insights for decision-making.

---
## Jupyter Notebook
https://github.com/PiyushKumar00/Loan-Default-Prediction/blob/main/iit%20internship%20-Copy1.ipynb




