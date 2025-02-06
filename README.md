# MLflow Tutorial Project

A simple demonstration of MLflow for experiment tracking using the California Housing dataset.

## Setup

```bash
pip install mlflow scikit-learn pandas numpy
```

## Project Structure

- `01_model_creation_and_tracking.ipynb`: Creates and tracks a model using MLflow
- `02_mlflow_retrival.ipynb`: Retrieves tracked experiments (WIP)
- `boston_toy_model.pkl`: Generated model file latest one 

## Usage

1. Run the training notebook:
```bash
jupyter notebook 01_model_creation_and_tracking.ipynb
```

2. View MLflow experiments:
```bash
mlflow ui
```
or
```bash
jupyter notebook 02_mlflow_retrival.ipynb
```

Then open http://localhost:5000 in your browser.

## Model Details

- Dataset: California Housing
- Pipeline: StandardScaler → PCA → LinearRegression
- Tracked metrics: MSE
- Tracked parameters: PCA components
