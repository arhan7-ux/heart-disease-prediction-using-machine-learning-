PROJECT TITLE
heart-disease-prediction-using-machine-learning

BRIEF ONE LINE SUMMARY
A Machine Learning-based classification project that predicts the likelihood of heart disease using patient medical attributes and Logistic Regression, achieving 81.97% accuracy on the test dataset.

OVERVIEW
Heart Disease Prediction is a supervised Machine Learning project developed to analyze patient health information and predict whether a person is likely to have heart disease.

The project uses a Logistic Regression classification algorithm trained on medical attributes such as age, gender, chest pain type, resting blood pressure, cholesterol level, maximum heart rate, and other clinical parameters.

The model learns patterns from historical patient data and classifies the input into two categories:

1 – Heart Disease Present

0 – Heart Disease Absent

The primary objective is to demonstrate how Machine Learning techniques can be applied to healthcare data for predictive analysis and preliminary risk assessment.

PROBLEM STATEMENT
Heart disease is one of the major health concerns worldwide. Identifying potential heart disease indicators through patient health information can help support early risk assessment.

The objective of this project is to develop a Machine Learning classification model that:

Analyzes patient medical and clinical attributes.

Identifies patterns associated with heart disease.

Trains a predictive model using historical medical data.

Predicts the presence or absence of heart disease for new patient inputs.

Evaluates model performance using training and testing accuracy.

The project aims to demonstrate the practical application of supervised learning in healthcare analytics.

DATASET
Dataset Name: Heart Disease Dataset

Dataset Dimensions:

Total Records: 303

Total Columns: 14

Input Features: 13

Target Variable: 1

Dataset Attributes:

Feature                Description

age                    Age of the patient

sex                    Gender indicator

cp                     Chest pain type

trestbps               Resting blood pressure

chol                   Serum cholesterol level

fbs                    Fasting blood sugar

restecg                Resting electrocardiographic results

thalach                Maximum heart rate achieved

exang                  Exercise-induced angina

oldpeak                ST depression induced by exercise

slope                  Slope of the peak exercise ST segment

ca                     Number of major vessels
 
thal                   Thalassemia-related categorical attribute

target                 Heart disease classification (0 or 1)

Target Distribution:

Heart Disease Present (1): 165 records

Heart Disease Absent (0): 138 records

Data Quality Checks:

Checked dataset structure and data types.

Examined statistical information using descriptive statistics.

Checked for missing values.

No missing values were identified in the dataset.

TOOLS AND TECHNOLOGIES 

Programming Language:

Python

Libraries and Frameworks:

NumPy – Numerical computations and array operations.

Pandas – Data loading, manipulation, and analysis.

Scikit-learn – Machine Learning model development and evaluation.

Machine Learning Algorithm:

Logistic Regression

Development Environment:

Jupyter Notebook

Key Techniques:

Data preprocessing and inspection.

Exploratory Data Analysis (EDA).

Supervised Machine Learning.

Binary Classification.

Train-Test Split.

Model Evaluation.

Predictive Analysis.

METHODS AND IMPLEMENTATION

The project follows these implementation steps:

Step 1: Data Collection and Loading

Loaded the Heart Disease Dataset from a CSV file into a Pandas DataFrame.

Step 2: Data Exploration

Examined the first and last five records.

Checked dataset dimensions and structure.

Analyzed data types and statistical summaries.

Identified missing values.

Examined the distribution of the target variable.

Step 3: Feature Selection

Separated the dataset into independent and dependent variables.

X: 13 independent input features.

Y: Target variable representing heart disease classification.

Step 4: Train-Test Splitting

Split the dataset into training and testing subsets using Scikit-learn's train_test_split().

Training Data: 80% (242 records).

Testing Data: 20% (61 records).

Stratified Sampling: Enabled.

Random State: 2.

Step 5: Model Development

Implemented the Logistic Regression algorithm using Scikit-learn.

The model was trained using the training dataset to identify relationships between patient health attributes and the target classification.

Step 6: Model Evaluation

Evaluated the trained model using the accuracy_score() metric on both training and testing datasets.

Step 7: Prediction on New Data

Provided a sample patient's medical attributes as input to the trained model and generated a binary classification prediction.

KEY INSIGHTS

The following observations were obtained during dataset exploration:

The dataset contains 303 patient records and 13 predictive features.

The target variable contains 165 positive and 138 negative classifications.

No missing values were detected across the 14 columns.

Patient attributes include demographic information, blood pressure, cholesterol, heart rate, and other clinical measurements.

The dataset was divided into training and testing subsets while maintaining target-class proportions.

Logistic Regression successfully learned patterns from the training data and generated predictions for unseen test records.

DASHBOARD / MODEL / OUTPUT

Model: Logistic Regression Classifier

This project currently implements a Machine Learning model through a Jupyter Notebook rather than an interactive dashboard.

Model Performance:

Evaluation Metric                       Result

Training Accuracy                       85.12%

Testing Accuracy                        81.97%


Sample Prediction:

A sample patient record was provided to the trained model:

input_data = (41, 0, 1, 130, 204, 0, 0, 172, 0, 1.4, 2, 0, 2)

Model Output:

Prediction: [1]

The Person has Heart Disease
The model classified the sample input as belonging to the positive heart disease class.

Note: This is an educational Machine Learning project and its predictions are not a substitute for professional medical diagnosis.

HOW TO RUN THIS PROJECT?

Follow these steps to execute the project locally.

Prerequisites:

Python 3.x

Jupyter Notebook

Basic knowledge of Python and Machine Learning

Step 1: Clone the Repository
git clone <your-repository-url>

Step 2: Navigate to the Project Directory
cd <your-project-folder>

Step 3: Install Required Libraries
pip install numpy pandas scikit-learn jupyter

Step 4: Add the Dataset

Place the heart_disease_data.csv file inside your project directory.

Update the dataset loading statement in the notebook:
heart_data = pd.read_csv("heart_disease_data.csv")

Step 5: Launch Jupyter Notebook
jupyter notebook

Step 6: Execute the Notebook

Open Heart Disease Prediction.ipynb and execute the cells sequentially to:

Load and explore the dataset.

Prepare input and target variables.

Split the data.

Train the Logistic Regression model.

Evaluate model accuracy.

Generate predictions for new patient data.

RESULTS AND CONCLUSION
The project successfully demonstrates the implementation of a supervised Machine Learning classification model for heart disease prediction.

The Logistic Regression model achieved:

Training Accuracy: 85.12%

Testing Accuracy: 81.97%

The results demonstrate that Logistic Regression can identify useful patterns in patient health attributes and perform binary classification on unseen test data.

This project provided practical experience in data preprocessing, exploratory data analysis, feature selection, model training, model evaluation, and predictive analytics using Python and Scikit-learn.

The project also demonstrates how Machine Learning can be applied to healthcare-related datasets to support data-driven analysis.

FUTURE WORK
The project can be enhanced through the following improvements:

Advanced Exploratory Data Analysis: Introduce correlation heatmaps, feature distribution plots, and visual analysis to better understand relationships between variables.

Feature Scaling: Apply StandardScaler to standardize numerical features and improve Logistic Regression convergence.

Algorithm Comparison: Experiment with Random Forest, Decision Tree, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN).

Performance Optimization: Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV.

Advanced Evaluation Metrics: Include Precision, Recall, F1-Score, Confusion Matrix, and ROC-AUC to obtain a more comprehensive evaluation.

Interactive Web Application: Develop a user-friendly prediction interface using Streamlit or Flask.

Model Deployment: Deploy the trained model through a web application or cloud-based platform for demonstration purposes.

AUTHOR & CONTACT
Author: Arhan
Project: Heart Disease Prediction Project Using Machine Learning
LinkedIn: www.linkedin.com/in/arhan-gogi-34aa992b9
GitHub: https://github.com/arhan7-ux
Email: arhangogi07@gmail.com 


