# Generator Fuel Consumption Analysis & Prediction

This repository contains Machine Learning notebooks and datasets focused on analyzing and predicting generator fuel consumption. The project explores various regression and classification techniques to understand consumption patterns, optimize fuel usage, and detect potential anomalies or fraud.

## Project Overview

The primary goal of this project is to analyze generator performance data, specifically focusing on fuel usage. The analysis includes identifying instances of fuel fraud, such as generators consuming more than their daily maximum capacity or being reported as running with zero consumption.

### Key Datasets

- `Gen.xlsx`: Main dataset containing generator visit logs, fuel readings, running hours, and consumption rates.
- `All cluster.xlsx`: Additional clustered data for comparative analysis across different generator sites.

### Analyzed Features

- **Consumption HIS**: Total fuel consumed within a specific visit period.
- **NBRE HEURES DE FONCTIONNEMENT DG1**: Total running hours of the generator.
- **CONSOMMATION HORAIRE DE FUEL DG1**: Fuel consumption rate per hour.
- **Consumption per Day**: Average daily fuel usage based on the visit period.
- **Running Time per Day**: Average hours the generator operates per day.

## Machine Learning Models

The project evaluates and compares several models to predict consumption and detect anomalies:

- **Support Vector Machines (SVM)**: Used to classify instances of abnormal consumption, achieving up to 88% accuracy with tuned parameters (`C=10`, `gamma=0.1`).
- **Artificial Neural Networks (Multi-layer Perceptron)**: For complex pattern recognition in consumption data.
- **Logistic Regression**: Used as a baseline for classification tasks.
- **Anomaly Detection**: Specialized techniques to identify potential fraud cases where fuel usage doesn't align with recorded engine hours.

## Repository Structure

- `Anomaly detection.ipynb`: Notebook focused on finding outliers and suspicious consumption entries.
- `Artificial Nueral Network-multi layer perceptron.ipynb`: Implementation of MLP for consumption prediction.
- `Support Vector Machine-Copy1.ipynb`: Detailed SVM implementation and parameter tuning.
- `Logistic Regression-Copy1.ipynb`: Linear classification baseline.
- `Project Progress.ipynb`: Main notebook featuring data visualization and initial preprocessing.

## Getting Started

1. Ensure you have Python installed with the following libraries:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
   - `scikit-learn`
   - `yellowbrick`
2. Open the Jupyter notebooks using `jupyter notebook` or `jupyter lab`.
3. Start with `Project Progress.ipynb` for an overview of the data and initial visualizations.
