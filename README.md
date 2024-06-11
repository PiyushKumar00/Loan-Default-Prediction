# Loan Default Prediction and Visualization

## Project Overview
This project aims to predict loan defaults using a machine learning model and visualize the predicted dataset using Power BI. The goal is to identify key factors contributing to loan defaults and create an efficient ML model to make prediction on production dataset then use Power BI on predicted dataset to provide actionable insights through interactive dashboards.

## Objectives
1. Run Models: Import the "Raw_Data_Singapore Credit Dataset" and run multiple supervised ML models with 3 different train-test split ratios (70/30, 75/25, 80/20).

2. Select Best Model: Perform a comparative analysis of the models based on evaluation metrics to select the best model. Fit the final model on the test dataset and save it for future use.

3. Predict New Data: Use the selected model to predict outcomes for the "Predict_Data_Singapore Credit Dataset" (production data) and generate the target labels.

4. Visualize in Power BI: Import the predicted dataset into Power BI and create visualizations for client reporting.

## Table of Contents    
1. [Introduction](#introduction)
2. [Data Description](#data-description)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Visualization](#visualization)
6. [Conclusion](#conclusion)
7. [How to Run](#how-to-run)

## Introduction
Provide a detailed explanation of the project's motivation, goals, and context.


## About the dataset:
 This dataset contains information about the credit landscape (credit loan
provided to customers) of a large Singapore bank

## Methodology
Outline the steps taken to process the data, engineer features, and build the machine learning model.

## Results
Summarize the key findings and model performance metrics.

## Visualization
Explain the Power BI dashboard and highlight key insights.

## Conclusion
Summarize the project outcomes and potential future work.

## How to Run
Instructions on setting up the environment and running the code:
```bash
# Clone the repository
git clone https://github.com/yourusername/loan-default-prediction.git

# Navigate into the directory
cd loan-default-prediction

# Install required packages
pip install -r requirements.txt

# Run the Jupyter notebooks
jupyter notebook
