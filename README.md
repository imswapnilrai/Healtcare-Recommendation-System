# Health Recommendation System

A Flask-based web application that recommends diseases, precautions, medications, diet, and workout routines based on user-inputted symptoms. The system uses a machine learning model to predict the disease from the given symptoms and provides relevant recommendations.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Model Information](#model-information)
- [Datasets](#datasets)
- [Routes](#routes)
- [License](#license)

## Overview

The Health Recommendation System allows users to input symptoms, and based on the provided symptoms, the application predicts the most likely disease. It then provides a description of the disease, precautions to take, recommended medications, dietary suggestions, and workout routines to follow.

## Features

- **Symptom Input:** Users can input symptoms to receive a disease prediction.
- **Disease Prediction:** Predicts the disease using a pre-trained Support Vector Classifier (SVC) model.
- **Recommendations:** Provides detailed information on the disease, precautions, medications, diet, and workout routines.
- **User-Friendly Interface:** The interface is simple and easy to use, built using Bootstrap for responsive design.

## Project Structure

Healthcare/
│
├── templates/
│ ├── index.html
│ ├── about.html
│ ├── contact.html
│ ├── developer.html
│
├── dataset/
│ ├── symtoms_df.csv
│ ├── precautions_df.csv
│ ├── workout_df.csv
│ ├── description.csv
│ ├── medications.csv
│ ├── diets.csv
│
├── model/
│ └── svc.pkl
│
├── main.py
└── README.md


# Health Recommendation System

## Overview
This is a Flask-based web application that predicts diseases based on input symptoms and provides recommendations on precautions, medications, diet, and workouts.

## Usage

### Home Page
- Navigate to the home page where you can input symptoms in the text box provided.
- Use symptoms like `itching, skin rash, acidity` separated by commas.
- Click on **"Recommend"** to get the predictions.

![image](https://github.com/user-attachments/assets/ab3a8d00-d633-4e5e-9c43-578cee1b9994)


### Results
- The app will display the predicted disease along with buttons to view detailed information such as:
  - **Description**
  - **Precautions**
  - **Medication**
  - **Diet**
  - **Workout**
![image](https://github.com/user-attachments/assets/1fc0d1f2-ea4e-4c60-ba80-785fa318cc26)
![image](https://github.com/user-attachments/assets/e4dd3dae-aacb-4d6c-83f8-93b45a4c9a17)
![image](https://github.com/user-attachments/assets/fc330236-c89a-4959-bd69-f5eb48b5a0f4)


### Navigation
- Use the navbar to navigate to the **"About"**, **"Contact"**, and **"Developer"** pages.

## Model Information
The application uses a pre-trained Support Vector Classifier (SVC) model to predict diseases based on the input symptoms. The model was trained on a dataset of symptoms and diseases.

## Datasets
The following datasets are used in this project:
- **symtoms_df.csv**: Contains a mapping of symptoms to disease indexes.
- **precautions_df.csv**: Contains precautionary measures for each disease.
- **workout_df.csv**: Contains recommended workouts for each disease.
- **description.csv**: Contains descriptions for each disease.
- **medications.csv**: Contains recommended medications for each disease.
- **diets.csv**: Contains dietary suggestions for each disease.

## Routes
- **/**: Home page where users can input symptoms and get recommendations.
- **/index**: Another route to access the home page.
- **/predict**: Handles the prediction logic and displays the results.
- **/about**: Information about the application.
- **/contact**: Contact information.
- **/developer**: Information about the developer.

## License
This project is licensed under the MIT License. See the LICENSE file for details.



