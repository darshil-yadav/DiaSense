# DiaSense 🩺

An AI-powered Diabetes Prediction System built using Machine Learning and Streamlit. DiaSense analyzes key health indicators and predicts whether a person is likely to have diabetes.

## Overview

DiaSense uses a Support Vector Machine (SVM) classifier trained on diabetes-related medical data. Users can enter their health metrics through a simple web interface and receive an instant prediction.

This project demonstrates the complete machine learning workflow:

* Data Collection
* Data Preprocessing
* Feature Scaling
* Model Training
* Model Evaluation
* Model Deployment with Streamlit

## Features

* User-friendly web interface
* Real-time diabetes prediction
* Standardized input processing
* Machine Learning-based classification
* Fast and lightweight deployment
* Open-source and customizable

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Streamlit
* Pickle

## Machine Learning Pipeline

### Data Preprocessing

* Loaded diabetes dataset
* Checked for missing values
* Separated features and target labels
* Applied StandardScaler for feature normalization

### Model Training

* Train-Test Split
* Stratified Sampling
* Support Vector Machine (SVM) Classifier
* Model Evaluation using Accuracy Score

### Deployment

The trained model and scaler are serialized using Pickle and integrated into a Streamlit web application for real-time predictions.

## Project Structure

```text
DiaSense/
│
├── diabetes.ipynb
├── app.py
├── diabetes_model.pkl
├── scaler.pkl
├── diabetes.csv
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/DiaSense.git
cd DiaSense
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run app.py
```

## Input Parameters

The model uses the following medical attributes:

* Pregnancies
* Glucose Level
* Blood Pressure
* Skin Thickness
* Insulin
* BMI
* Diabetes Pedigree Function
* Age

## Example Prediction

Input:

```text
Pregnancies: 2
Glucose: 120
Blood Pressure: 70
Skin Thickness: 25
Insulin: 100
BMI: 28.5
Diabetes Pedigree Function: 0.35
Age: 35
```

Output:

```text
Prediction: Not Diabetic
```

## Author

Developed as a Machine Learning project to demonstrate predictive healthcare analytics using Python and Scikit-Learn.
