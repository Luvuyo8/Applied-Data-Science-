# Project Overview:
The project utilizes Support Vector Machines (SVM) to classify human cell records into either benign (B) or malignant (M) categories. The model is trained using cell characteristics, such as clump thickness, uniformity of cell size, and marginal adhesion, among others, to predict the diagnosis of cell samples. This classification helps in early cancer detection, aiding in medical decision-making.

## Objective:
The primary objective of this notebook is to build and train an SVM classifier using human cell sample records. These samples contain multiple features that help determine whether the sample is benign or malignant. The goal is to classify the samples accurately based on the given features using SVM.

## Dataset Description:
The dataset includes several hundred records of human cell samples. Each record contains:
ID: A unique identifier for the sample
Clump: Clump thickness (graded from 1 to 10, with 1 being closest to benign)
UnifSize: Uniformity of cell size
UnifShape: Uniformity of cell shape
MargAdh: Marginal adhesion
SingEpiSize: Single epithelial cell size
BareNuc: Bare nuclei
BlandChrom: Bland chromatin
NormNucl: Normal nucleoli
Mit: Mitoses
Class: Diagnosis (2 for benign, 4 for malignant)

## Model Training and Results:
Train set: 546 samples with 9 features
Test set: 137 samples with 9 features

## Machine Learning Model:

The Support Vector Machines (SVM) model was trained using the Radial Basis Function (RBF) kernel to classify cell samples. The results show that the SVM classifier achieved impressive accuracy in predicting whether the sample is benign or malignant.

The model was evaluated based on:
## Performance Metrics:
Precision: 0.97 (for benign), 0.90 (for malignant)
Recall: 0.94 (for benign), 1.00 (for malignant)
F1-Score: 0.96 (weighted average)
Accuracy: 96%
## Additional Metrics:
F1-Score: 0.9639
Jaccard Score: 0.9444

The classifier successfully predicted the diagnosis of the test set with a high level of accuracy, indicating the effectiveness of the SVM model for this type of classification task.



