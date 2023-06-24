# Sepsis_Prediction_with_Machine-Learning-FastAPI
[![View Repositories](https://img.shields.io/badge/View-My_Repositories-blue?logo=GitHub)](https://github.com/violetteallotey?tab=repositories)
[![View My Profile](https://img.shields.io/badge/MEDIUM-Article-purple?logo=Medium)](https://medium.com/@violetteallotey/fastapi-spells-conjuring-predictive-powers-for-sepsis-detection-adfd22866b77)
[![Docker App](https://img.shields.io/badge/Docker-App-yellow)](https://huggingface.co/spaces/Adoley/Sepsis-Prediction-Using-FastAPI)
[![Website Portfolio](https://img.shields.io/badge/My-Website-darkgreen)](https://adoley.my.canva.site/)

Develop a Machine Learning API (Application Programming Interface) using FastAPI.

![ai(3)](https://github.com/violetteallotey/Sepsis_Prediction_with_Machine-Learning-FastAPI/blob/main/assets/screenshots/sepsis%20prediction.jpg)

## Introduction

Sepsis is a life-threatening condition that requires early detection and prompt treatment. This API provides a machine-learning model that can predict the likelihood of sepsis based on patient data. By leveraging the power of FastAPI, we can quickly and efficiently process incoming requests and provide accurate predictions in real-time.

## Description

This repository contains an API for sepsis prediction using machine learning techniques. The API is built using FastAPI, a modern, fast (high-performance), web framework for building APIs with Python.

## Importance of Project  

The dataset used contains a list of patients in a hospital and their attributes and whether the patient is positive for Sepssis or not.

Sepsis is a severe and potentially life-threatening condition that occurs when the body's response to an infection triggers widespread inflammation. It is often referred to as blood poisoning.

The aim of this project is to explore the various factors that can cause sepsis in order to predict the occurence of sepsis.

Predicting sepsis is important because early recognition and intervention can significantly improve patient outcomes. Sepsis can progress rapidly and become life-threatening within a short period. By identifying patients who are at risk of developing sepsis, healthcare providers can initiate timely treatment and interventions to prevent the condition from worsening.

# Dataset Description -

The data for this project is in a csv format. The following describes the columns present in the data.

| Column Name | Target | Description                                                                   |
| ----------- | ------ | ----------------------------------------------------------------------------- |
| ID          | N/A    | Unique number to represent patient ID                                         |
| PRG         | False  | Plasma glucose                                                                |
| PL          | False  | Blood Work Result-1 (mu U/ml)                                                 |
| PR          | False  | Blood Pressure (mm Hg)                                                        |
| SK          | False  | Blood Work Result-2 (mm)                                                      |
| TS          | False  | Blood Work Result-3 (mu U/ml)                                                 |
| M11         | False  | Body mass index (weight in kg/(height in m)^2                                 |
| BD2         | False  | Blood Work Result-4 (mu U/ml)                                                 |
| Age         | False  | patients age (years)                                                          |
| Insurance   | N/A    | If a patient holds a valid insurance card                                     |
| Sepssis     | True   | Positive: if a patient in ICU will develop a sepsis , and Negative: otherwise |

## Features
Fast and efficient prediction of sepsis using a machine learning model
API endpoints for single patient prediction and batch prediction
Dockerized deployment for easy setup and portability

## Setup

Install the required packages to be able to run the evaluation locally.

You need to have [`Python 3`](https://www.python.org/) on your system (**a Python version lower than 3.10**). Then you can clone this repo and being at the repo's `root :: repository_name> ...` follow the steps below:

- Windows:

        python -m venv venv; venv\Scripts\activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt

- Linux & MacOs:
  python3 -m venv venv; source venv/bin/activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt

The both long command-lines have a same structure, they pipe multiple commands using the symbol `;` but you may manually execute them one after another.

1. **Create the Python's virtual environment** that isolates the required libraries of the project to avoid conflicts;
2. **Activate the Python's virtual environment** so that the Python kernel & libraries will be those of the isolated environment;
3. **Upgrade Pip, the installed libraries/packages manager** to have the up-to-date version that will work correctly;
4. **Install the required libraries/packages** listed in the `requirements.txt` file so that it will be allow to import them into the python's scripts and notebooks without any issue.

**NB:** For MacOs users, please install `Xcode` if you have an issue.

## Run FastAPI

- Run the demo apps (being at the repository root):

  FastAPI:

  - Demo

        uvicorn src.demo_01.api:app --reload

    <!-- - Sepsis prediction

          uvicorn src.salary.api:app --reload  -->

  - Go to your browser at the following address, to explore the api's documentation :
    http://127.0.0.1:8000/docs

## Screenshots
![ezgif com-optimize (1)](https://github.com/ikoghoemmanuell/Machine-Learning-API-using-FastAPI/assets/102419217/a8352c5f-afea-43b1-8bf5-c24607cf3481)
![ezgif com-crop](https://github.com/ikoghoemmanuell/Machine-Learning-API-using-FastAPI/assets/102419217/df0ed5a8-2daf-47ca-a4f5-e6128429d5d3)

## API Endpoints
* GET / - Returns information about the API.

* POST /predict - Makes a prediction for a single patient.

* POST /predict/batch - Makes predictions for multiple patients.

For detailed information on request and response formats, refer to the API documentation accessible at http://localhost:8000/docs when the API server is running.

## Deployment and Scaling
The API can be deployed and scaled using Docker. By containerizing the application, we achieve portability and consistency across different environments.

## Resources

Here are some ressources you would read to have a good understanding of FastAPI :

- [Tutorial - User Guide](https://fastapi.tiangolo.com/tutorial/)
- [Video - Building a Machine Learning API in 15 Minutes ](https://youtu.be/C82lT9cWQiA)
- [FastAPI for Machine Learning: Live coding an ML web application](https://www.youtube.com/watch?v=_BZGtifh_gw)
- [Video - Deploy ML models with FastAPI, Docker, and Heroku ](https://www.youtube.com/watch?v=h5wLuVDr0oc)
- [FastAPI Tutorial Series](https://www.youtube.com/watch?v=tKL6wEqbyNs&list=PLShTCj6cbon9gK9AbDSxZbas1F6b6C_Mx)
- [Http status codes](https://www.linkedin.com/feed/update/urn:li:activity:7017027658400063488?utm_source=share&utm_medium=member_desktop)

## 👏 Support

Contributions to the Sepsis Prediction API project are welcome and encouraged! If you have any ideas, improvements, or bug fixes, please submit a pull request. Make sure to follow the established coding style and conventions.

If you find any issues or have suggestions for new features, please open an issue on the GitHub repository.

## Author

- [Violette Naa Adoley Allotey](https://medium.com/@violetteallotey)
