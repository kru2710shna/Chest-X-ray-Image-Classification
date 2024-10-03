# Chest X-ray Image Classification Project

## Project Overview
This project focuses on developing a binary classification model to predict 14 different pathological conditions based on frontal-view chest X-ray images. Utilizing the ChestX-ray8 dataset, which contains 108,948 images from 32,717 unique patients, we aim to provide accurate predictions that can assist physicians in diagnosing various diseases. Each image in the dataset comes with multiple text-mined labels, enabling the classification of eight different diseases.

## Accessing the Dataset
You can download the entire ChestX-ray8 dataset for free [here](https://nihcc.app.box.com/v/ChestXray-NIHCC). For convenience, a subset of approximately 1,000 images has been provided. You can access these images in the folder path stored in the `IMAGE_DIR` variable.

The dataset includes a CSV file with labels for each X-ray. Additionally, we have processed the labels for a small sample and generated three new files to help you get started:

- `nih/train-small.csv`: 875 images for training.
- `nih/valid-small.csv`: 109 images for validation.
- `nih/test.csv`: 420 images for testing.

The dataset is annotated by consensus among four different radiologists for five of the fourteen pathologies:

- Consolidation
- Edema
- Effusion
- Cardiomegaly
- Atelectasis

## Table of Contents
- [Data Preparation](#data-preparation)
- [Visualizing Data](#visualizing-data)
- [Preventing Data Leakage](#preventing-data-leakage)
- [Model Development](#model-development)
- [Addressing Class Imbalance](#addressing-class-imbalance)
- [Leveraging Pre-trained Models Using Transfer Learning](#leveraging-pre-trained-models-using-transfer-learning)
- [Evaluation](#evaluation)
- [AUC and ROC Curves](#auc-and-roc-curves)

## Data Preparation
In this section, we focus on preparing the dataset for model training, including data cleaning and normalization processes.

## Visualizing Data
Data visualization techniques are employed to understand the distribution of labels and the overall characteristics of the dataset.

## Preventing Data Leakage
Strategies are implemented to detect and mitigate data leakage, particularly concerning patient overlap between training and testing datasets. The function `check_for_leakage` is utilized to ensure no shared patient IDs.

## Model Development
We develop a model that will provide binary classification predictions for each of the 14 labeled pathologies, predicting 'positive' or 'negative' outcomes.

## Addressing Class Imbalance
Class imbalance is a significant concern in medical datasets. We compute class frequencies and apply weighting strategies during model training to balance contributions from each class.

## Leveraging Pre-trained Models Using Transfer Learning
To enhance model performance, we utilize transfer learning techniques with pre-trained models that have already been trained on large datasets.

## Evaluation
Model performance is evaluated through various metrics to assess its effectiveness and reliability in predicting pathologies.

## AUC and ROC Curves
We employ AUC and ROC curves to evaluate the model's predictive capabilities and visualize its performance across different threshold values.

---

For any questions or contributions to this project, please feel free to reach out!
