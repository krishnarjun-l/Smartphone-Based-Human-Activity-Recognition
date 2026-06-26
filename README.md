# Smartphone-Based Human Activity Recognition Using Supervised Machine Learning

Classifying six daily physical activities — walking, walking upstairs, walking downstairs, sitting, standing, and laying — from smartphone accelerometer and gyroscope signals, using classical supervised machine learning models.

This was the final project for an Advanced Machine Learning course.

## Overview

As wearable and mobile devices become part of everyday life, automatic Human Activity Recognition (HAR) has become an important task in ubiquitous computing, healthcare monitoring, and fitness tracking. The goal of this project is to build accurate models that classify a person's physical activity from sensor data, with applications in elder care, personalized fitness tracking, and rehabilitation monitoring.

We use the [UCI HAR dataset](https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones), which contains sensor recordings from 30 volunteers (ages 19–48), each wearing a Samsung Galaxy S II on the waist. The smartphone's embedded accelerometer and gyroscope captured 3-axial linear acceleration and 3-axial angular velocity at 50 Hz. The signals were pre-processed into fixed-width 2.56-second sliding windows, and a 561-feature vector (time- and frequency-domain variables) was computed for each window.

## Dataset

The dataset is **not included** in this repository because of its size. Download it directly from the UCI Machine Learning Repository:

- https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones

After downloading, unzip it and place the `UCI HAR Dataset` folder at the repository root (or update the file paths at the top of the notebooks to point to wherever you saved it):

```
Smartphone-Based-Human-Activity-Recognition/
├── UCI HAR Dataset/        <- place the downloaded dataset here
   ├── train/
   ├── test/
   ├── features.txt
   └── activity_labels.txt
```

The dataset provides, for each record: triaxial acceleration, triaxial angular velocity, a 561-feature vector, an activity label, and the subject identifier. It is pre-split into 70% training and 30% test data by subject.

## Methods

The workflow covers:

- **Exploratory data analysis** of the sensor features and activity distribution
- **Dimensionality reduction** with Principal Component Analysis (PCA)
- **Model training and comparison** across several supervised classifiers:
  - Support Vector Machine (SVM / SVC)
  - Random Forest
  - XGBoost
  - Multi-Layer Perceptron (MLPClassifier)
  - Logistic Regression
- **Evaluation** using accuracy, classification reports, and confusion matrices

## Repository structure

```
├── human_activity_recognition.ipynb
├── Individual_Project_Report.pdf
├── requirements.txt
└── README.md
```

## Authors

Group 9 — Advanced Machine Learning final project:

- Krishnarjun Lakshminarayanan
- Ekshitha Yella
- Venkata Sai Harshith Royal Chikati
- Shyam Sundar Theerdhala

## Acknowledgements

Dataset: Reyes-Ortiz, J., Anguita, D., Ghio, A., Oneto, L., & Parra, X. (2012). *Human Activity Recognition Using Smartphones*. UCI Machine Learning Repository.
