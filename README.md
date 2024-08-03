# Predictive Analysis on Autoscaling of Pods

This project predicts the optimal number of replicas for Kubernetes Pods based on CPU and memory usage metrics. Using linear regression, it helps dynamically adjust the number of replicas to optimize resource utilization in a 5G mobile network environment.

## Key Features

- **Data Collection**: Captures CPU and memory metrics from Pods.
- **Data Preprocessing**: Normalizes and cleans data.
- **Model Training**: Trains a linear regression model for predicting replicas.
- **Model Evaluation**: Assesses model performance with Mean Squared Error.
- **Deployment Update**: Automatically updates Kubernetes deployments based on predictions.

## Usage

1. **Train the Model**:

    ```bash
    python scripts/train_model.py
    ```

2. **Evaluate the Model**:

    ```bash
    python scripts/evaluate.py
    ```

3. **Predict and Update Deployment**:

    ```bash
    python scripts/predict_and_update.py
    ```

## Requirements

- Python 3.x
- Dependencies listed in `requirements.txt`

## Configuration

Update `config/config.yaml` with paths to your data, model, and deployment files.
