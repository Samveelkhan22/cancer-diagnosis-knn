# Cancer Diagnosis Using K-Nearest Neighbors (KNN)

This project implements a K-Nearest Neighbors (KNN) algorithm to predict the type of cancer based on gene expression data. The dataset includes 20 genes as biomarkers used to classify cancer types. The goal is to use KNN to predict the cancer type for a given test dataset based on training data.

## Overview

The KNN algorithm works by finding the 'k' closest data points in the training set to a test point. The label of the test point is then predicted by the majority class among its nearest neighbors. The Euclidean distance is used to measure the similarity between data points.

## Files

- `KNN.ipynb`: Python implementation of the K-Nearest Neighbors algorithm.
- `training.txt`: The training dataset containing gene expression data and corresponding labels.
- `test.txt`: The test dataset containing gene expression data (labels are unknown).
- `predictions.txt`: Output file containing the predicted cancer types for the test dataset.

## Algorithm Details

- Load Data: The training and test datasets are read, where each row represents a patient and the columns represent gene expression levels.
- Calculate Euclidean Distance: For each test point, the distance to all points in the training set is computed using Euclidean distance.
- Find Nearest Neighbors: The k nearest neighbors are identified based on the shortest distances.
- Predict Label: The majority label of the k nearest neighbors is assigned as the predicted label for the test point.

