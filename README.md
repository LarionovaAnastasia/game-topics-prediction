# game-topics-prediction

⚠️ Work in progress ⚠️

A complete end-to-end machine learning project from the initial idea to deployment.
The goal of this project is to create a game topic prediction application.

<img src="https://github.com/LarionovaAnastasia/game-topics-prediction/blob/main/assets/life_run.gif" width="750" height="420" />


📍 The work on this project contains several phases : 

1. Exploratory data analysis 
2. Data cleaning and normalization 
3. Building a training / testing pipeline for a baseline model
4. Traininig production model **(coming soon)**
5. Error analysis **(coming soon)**
6. Setting up API and web extention 
7. Deploying the application and connecting a continuous integration solution **(coming soon)**


# Repo structure

    ├── assets                          <- Media files.
    │
    ├── config                          <- Configuration files.
    │
    ├── data  
    │   ├── processed                   <- Intermidiate, transformed data. 
    │   ├── raw                         <- The original data
    │   └── splitted                    <- The final data sets for modeling. 
    │
    ├── deploy                          <- Scripts for Web extension and Docker deployement                  
    │
    ├── game_topics                     <- Source code for use in this project. 
    │   ├── models                      <- Scripts to define models. 
    │   ├── utils                       <- Scripts with basic utilities used in other scripts. 
    │   ├── normalize_and_clean.py      <- Script to normalize and clean the data. 
    │   └── train_model.py              <- Script to train the model.   
    │
    ├── model_checkpoints               <- Trained and serialized models, fitted tokenizers and vectorizers. 
    │
    ├── notebooks                       <- Jupyter notebooks containing Exploratory Data Analysis and Error Analysis. 
    │
    ├── server                          <- Scripts to define the API. 
    │
    └── tests                           <- Testing scripts.


# Data Source 

The data used in this project is publicly available on Kaggle : https://www.kaggle.com/nikdavis/steam-store-games

The original dataset contains 6 files. Only two are used in this project : 
- steam.csv
- steam_description_data.csv

# Features

- **Logistic regression** powered by [Scikit Lean](https://scikit-learn.org/stable/) 
- **CNN model** power by Keras (with Tensorflow background)
- **Exploratory data analysis** using Pandas
- **Data cleaning and normalizing** powered by NLTK and Regex
- **Functionality tests** powered by Unittest
- **Server** via FastAPI and Uvicorn.
- **Chrome extension** for interacting with a model in the browser.
