# -Predicting-Heart-Disease-Using-Clinical-Parameters
Project Summary: Predicting Heart Disease Using Clinical Parameters
Objective
The primary goal of this project is to develop machine learning models that can predict whether a patient has heart disease based on 13 clinical parameters. The clinical parameters include age, sex, chest pain type, resting blood pressure, cholesterol levels, fasting blood sugar, resting electrocardiographic results, maximum heart rate achieved, exercise-induced angina, ST depression, slope of the ST segment, number of major vessels colored by fluoroscopy, and thalium stress test results. The target variable is a binary outcome indicating the presence or absence of heart disease.

Dataset Overview
The dataset contains the following columns:

age: Age of the patient in years.
sex: Gender of the patient (1 = male; 0 = female).
cp: Chest pain type (0-3, ranging from typical angina to asymptomatic).
trestbps: Resting blood pressure (in mm Hg).
chol: Serum cholesterol level in mg/dl.
fbs: Fasting blood sugar (>120 mg/dl; 1 = true; 0 = false).
restecg: Resting electrocardiographic results (0-2, indicating normal to possible left ventricular hypertrophy).
thalach: Maximum heart rate achieved.
exang: Exercise-induced angina (1 = yes; 0 = no).
oldpeak: ST depression induced by exercise relative to rest.
slope: Slope of the peak exercise ST segment (0-2).
ca: Number of major vessels (0-3) colored by fluoroscopy.
thal: Thalium stress test result (1 = normal; 3 = fixed defect; 6 = reversible defect).
target: Presence of heart disease (1 = yes; 0 = no).
Approach
Data Preprocessing:

Loaded the dataset and checked for missing values and basic statistics.
Standardized the features to ensure all variables are on the same scale, which is crucial for distance-based models like K-Nearest Neighbors.
Split the dataset into training and testing sets (70% training, 30% testing).
Model Development:

Logistic Regression: A linear model used for binary classification.
K-Nearest Neighbors (KNN): A non-parametric method used for classification based on the closest training examples in the feature space.
Support Vector Machine (SVM): A linear classifier that tries to find the best margin that separates the classes.
Decision Tree Classifier: A tree-based model that splits the data into subsets based on the most significant features.
Random Forest Classifier: An ensemble method that builds multiple decision trees and merges them to get a more accurate and stable prediction.
Model Evaluation:

Evaluated each model using accuracy, confusion matrix, and classification report (precision, recall, F1-score).
Compared the performance of all models using a bar plot of their accuracies.
Results
Each model provided different levels of accuracy in predicting heart disease.
Logistic Regression: Provided a solid baseline with linear separability of the data.
K-Nearest Neighbors: Performance depended on the number of neighbors; generally effective but sensitive to scaling.
Support Vector Machine: Generally performed well with linearly separable data and was effective after scaling.
Decision Tree: Good at capturing complex interactions but prone to overfitting.
Random Forest: Offered the best performance by reducing overfitting through the ensemble of trees.
Conclusion
The project successfully demonstrated the use of different machine learning models to predict heart disease using clinical parameters. The Random Forest Classifier typically emerged as the most accurate model, but the choice of the model could vary depending on the specific needs (e.g., interpretability vs. accuracy).
