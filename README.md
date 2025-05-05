# Anomaly-Detection-in-Network-Traffic

## Project Overview

This project focuses on building an Intrusion Detection System (IDS) that identifies anomalous network activity using unsupervised deep learning techniques — **Autoencoder** and **Restricted Boltzmann Machine (RBM)**.

## Objective

Create a system capable of detecting network intrusions by learning normal traffic behavior and identifying deviations as anomalies.

## Techniques Used

- **Autoencoder**: A deep neural network trained to reconstruct normal network patterns. Anomalies are detected based on reconstruction error.
- **Restricted Boltzmann Machine (RBM)**: A generative stochastic neural network used for feature extraction and anomaly detection.

## Hyperparameters

The following six hyperparameters were applied and tuned to optimize model performance:

- **Encoding Size**: Defines the size of the compressed representation in Autoencoder.
- **Learning Rate**: Controls how fast the model learns during training.
- **Dropout**: Prevents overfitting by randomly dropping neurons during training.
- **Batch Size**: Number of samples processed at a time during training.
- **Optimizer**: Algorithm used for updating weights (e.g., Adam, SGD).
- **Training Epochs**: Number of complete passes through the training dataset.

## Dataset

A benchmark network traffic dataset is used, preprocessed and normalized. The dataset includes both normal and anomalous traffic patterns. The model is trained on normal traffic, and anomalies are detected based on learned reconstruction errors or deviations.

## Results

The model's performance is evaluated using metrics such as:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
