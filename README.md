# Obesity Level Prediction Analysis

## Overview
This project aims to predict obesity levels based on various lifestyle and physiological factors. The analysis uses Decision Tree and K-Nearest Neighbors (KNN) classification models to identify major contributors to obesity and compare the performance of the models.

## Objective
Identify the key factors contributing to obesity.
Compare the performance of Decision Tree and KNN models in predicting obesity levels.

## Dataset
The dataset was sourced from the UC Irvine Machine Learning Repository and contains 17 attributes, including age, diet, activity, and transport preferences. It spans 2111 individuals from Mexico, Peru, and Colombia, with ages ranging from 14 to 61. After preprocessing, 2082 rows were used for analysis.

## Models
 - Decision Tree: Chosen for its ability to capture complex relationships and rank feature importance.
 - KNN: Selected for its simplicity and effectiveness in handling non-linear boundaries.

## Preprocessing
 - Renamed attributes for clarity.
 - Removed highly correlated variables like weight and height.
 - Applied one-hot encoding for categorical variables and PCA to reduce dimensionality.
 - Train/test split (75%/25%) with cross-validation (5-fold grid search) to fine-tune model parameters.

## Evaluation
 - Metric: F1-score (Micro-average) was chosen for a balanced assessment of precision and recall across all classes.
 - Results: The KNN model performed better with a micro-average F1-score of 0.81, compared to the Decision Tree's 0.76.

## Conclusion
The models achieved moderate success, with room for improvement, particularly in handling class imbalances. Further refinement and data collection are needed for real-world deployment.

## Tools
 - Models: Decision Tree, KNN 
 - Preprocessing: PCA, One-Hot Encoding
 - Evaluation: F1-Score (Micro-average)
