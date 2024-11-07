# COVID-19-Detection-Using-Machine-Learning

This repository contains a machine learning project that predicts COVID-19 infection status based on various symptoms and demographic data. Inspired by the research paper titled "COVID-19 Detection Using Machine Learning" by researchers at the National Institute of Technology Karnataka, this project aims to build and compare different classification models to identify the presence of COVID-19 with high accuracy.

##📑 Project Overview
Early detection of COVID-19 can play a crucial role in slowing the spread of the virus. This project implements multiple machine learning algorithms to classify patients as COVID-positive or COVID-negative based on symptom data. We evaluate the models based on accuracy, Mean Squared Error (MSE), and ROC AUC scores, with the goal of identifying the best model for prediction.

##📂 Dataset
The dataset consists of various attributes collected from patients, including symptoms and demographic information. It includes both COVID-positive and COVID-negative samples.

Input Features: Includes binary indicators for symptoms like fever, cough, fatigue, breathing issues, and other relevant attributes.
Target Variable: COVID-19 status (1 for positive, 0 for negative).

##🛠 Project Workflow
1. Data Collection & Preprocessing
Data Cleaning: Removing redundant columns and handling missing values.
Encoding Categorical Variables: Converting 'yes'/'no' responses into binary values (1/0) for model compatibility.
Data Splitting: Splitting the dataset into training and testing sets (80%/20%) to assess model performance on unseen data.
2. Exploratory Data Analysis (EDA)
Visual Insights: Created bar charts and pie charts to explore the distribution of COVID-19 cases, symptoms, and other relevant data patterns.
Symptom Analysis: Examined which symptoms had a higher correlation with COVID-19 positive cases.
3. Model Training & Hyperparameter Tuning
Algorithms Used:
Logistic Regression
K-Nearest Neighbors (KNN)
Random Forest
Hyperparameter Tuning: Used GridSearchCV to optimize each model’s hyperparameters, focusing on achieving the best accuracy and minimizing error.
Training Results: Evaluated models based on Accuracy, MSE, ROC AUC Score, and execution time.
4. Model Evaluation
Performance Comparison: Compared models based on accuracy, ROC AUC, and MSE to identify the best-performing algorithm.
Visualization: Plotted accuracy, MSE, and ROC AUC scores to visually compare model performance.
5. Final Model Selection
Top Performer: Random Forest achieved the highest accuracy (98.39%) and low MSE, making it the best choice for COVID-19 prediction in this dataset.
## 📊 Results

| Model               | Accuracy | MSE   | ROC AUC | Time to Train (s) |
|---------------------|----------|-------|---------|--------------------|
| Logistic Regression | 97.03%   | 3.036 | 93.23   | 0.038             |
| K-Nearest Neighbors | 98.37%   | 2.57  | 98.58   | 24.252            |
| Random Forest       | 98.39%   | 2.207 | 97.41   | 213.331           |

The results indicate that the Random Forest classifier is the best choice for this task, achieving high accuracy and low error rates, though it requires more time to train compared to Logistic Regression.

##📈 Visualizations
Some key visualizations generated in this project:

Pie Charts: Distribution of COVID-19 positive and negative cases, distribution of symptoms (e.g., breathing issues, fever).
Bar Charts: Comparison of model accuracy, MSE, and ROC AUC across different algorithms.

##🤖 Future Enhancements
Feature Engineering: Adding more features like patient history or advanced symptoms.
Model Optimization: Testing additional algorithms like Support Vector Machines or deep learning approaches for potentially improved performance.
Real-world Deployment: Deploying the best-performing model as a web app for users to input symptoms and receive COVID-19 risk predictions.

##📜 References
This project is inspired by the research paper "COVID-19 Detection Using Machine Learning" by researchers at the National Institute of Technology Karnataka, which discusses the use of machine learning for early COVID-19 diagnosis.
