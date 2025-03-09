# Predictive Maintenance Model

## Project Overview

Predictive maintenance is a technique that uses machine learning models to predict equipment failures before they happen. This project analyzes machine performance data, preprocesses it, and trains classification models to detect potential failures.

The dataset contains machine operating conditions and failure types. The goal is to build a robust predictive model that helps prevent unplanned downtimes by identifying early signs of equipment failure.

## Installation

To set up the environment, install the required dependencies:

```sh
pip install mlflow scikit-learn imbalanced-learn pandas numpy
```

## Data Exploration

The dataset contains information on machine types, operational metrics, and failure types. Key steps in data exploration include:

- Checking feature distributions
- Identifying missing values
- Understanding failure type occurrences

## Data Preprocessing

To prepare the data for modeling, the following steps are performed:

- Encoding categorical variables (e.g., machine type and failure type)
- Handling data leakage by removing non-predictive identifiers
- Balancing class distribution using **SMOTE** to address imbalanced data

## Model Training

Two classification models are trained and evaluated:

1. **Logistic Regression**
2. **Naïve Bayes**

The dataset is split into training and testing sets. Both leaky and non-leaky versions of the dataset are used to understand the impact of data leakage on model performance.

### Evaluation Metrics

Models are evaluated using:

- **Accuracy**: Measures overall correctness of predictions
- **Classification Report**: Includes precision, recall, and F1-score for each failure type

## Model Deployment

The project integrates **MLflow** for model tracking and experiment logging. The best-performing model can be saved and deployed for real-world predictive maintenance applications.

## Usage

Run the preprocessing and model training scripts to train models on the dataset. Modify the pipeline as needed to test different machine learning approaches.

## Future Improvements

- Experiment with advanced models like **Random Forest** or **Neural Networks**
- Feature engineering to enhance predictive power
- Implement real-time monitoring with **streaming data**

---

This project demonstrates how machine learning can be used for predictive maintenance, helping industries minimize downtime and improve operational efficiency.

