# Cybersecurity-and-ML
Network Traffic Classifier

## Overview
This project is focused on the classification of network traffic data to identify potential intrusions. The codebase includes data loading, preprocessing, feature extraction, model training, and evaluation phases with the utilization of two datasets: KDD and UNSW-NB15. The datasets are subjected to normalization, encoding, dimensionality reduction using Independent Component Analysis (ICA), and feature selection using Feature from Model (FFM). The classification is performed by Support Vector Machine (SVM).

## Dependencies
- pandas
- numpy
- matplotlib
- scikit-learn
- tqdm
- scipy

## Data Preprocessing
Preprocessing includes normalization of numerical features and label encoding of categorical features.

### Raw Data Filtering
A function `raw_data_filter` is provided to load and filter the raw data, applying headers and mapping the 'attack' field to a binary classification target.

## Feature Selection and Dimensionality Reduction
Dimensionality reduction is performed using ICA, reducing the features to a set amount, which is further used to train the SVM model.

## Model Training
An SVM with a linear kernel is trained after feature extraction.

## Evaluation
Model evaluation is performed through accuracy, precision, recall, and F1-score metrics. Confusion matrices and a comparison between predicted and actual labels are also presented via bar plots.

## Visualization
Various plots are generated and saved as .png files to visualize accuracy metrics and the comparison between predicted and actual class distributions.

## Feature Selection Using FFS
Filters features using feature importance provided by an SVM model and assesses the impact on model performance.

## Data Description
Two separate datasets are explored:
1. KDD dataset for network-based intrusion detection systems.
2. UNSW-NB15 dataset providing a more modern and diverse set of features.

The data is split into training and test sets, with further data characterization through information and unique value exploration.

## Usage
The code is structured in functions that can be called with the appropriate parameters related to the datasets used.

