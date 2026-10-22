# Build a Churn Prediction Model using Ensemble Learning

To build ensemble models like Random Forest, Adaboost, and Gradient boosting models on the given dataset to determine whether the customer will churn or not.

## Overview
Ensemble methods aim to combine the predictions of several base estimators built with a given learning algorithm to improve generalizability/robustness over a single estimator. Ensemble methods are ideal for regression and classification, where they reduce bias and variance to boost the accuracy of models. The most famous ensemble methods are boosting and bagging. Bagging is a homogeneous weak learners’ model that learns from each other independently in parallel and combines them for determining the model average. The Random Forest model uses Bagging.

Boosting is also a homogeneous weak learners’ model but works differently from Bagging. In this model, learners learn sequentially and adaptively to improve model predictions of a learning algorithm. The AdaBoost and Gradient Boosting use Boosting techniques.

## Data
This data provides information about a video streaming service company, where they want to predict if the customer will churn or not. The CSV consists of around 2000 rows and 16 columns

_Data is not included in this repository._

## Approach
1. Importing the required libraries and reading the dataset.
2. Feature Engineering  Dropping of unwanted columns
3. Model Building  Performing train test split  Random Forest Model  AdaBoost Model  Gradient Boosting Model
4. Model Validation (predictions)  Recall score  Precision score  F1-score  ROC and AUC
5. Feature Importance  Create a function to find important features  Plot the features
6. LIME implementation  Define a function for implementing the LIME technique over the dataset.

Modular code overview

Once you unzip the modular_code.zip file you can find the following folders within it.
1. input
2. src
3. output
4. lib
1. Input folder - It contains all the data that we have for analysis. There is one csv file in our case,  Data_regression
2. Src folder - This is the most important folder of the project. This folder contains all the modularized code for all the above steps in a modularized manner. This folder consists of:  Engine.py  ML_Pipeline The ML_pipeline is a folder that contains all the functions put into different python files, which are appropriately named. These python functions are then called inside the engine.py file.
3. Output folder – The output folder contains three subfolders.  LIME_reports - contains the LIME reports generated for all three algorithms.  Models - contains the models generated for all three algorithms.  ROC_curves - contains the ROC curves generated for all three algorithms.
4. Lib folder - This is a reference folder. It contains the original ipython notebook that we saw in the videos.

## Tech stack
 Language - Python  Libraries - NumPy, pandas, matplotlib, sklearn, pickle, imblearn, lime

## How to run
```bash
pip install -r Modular_code/src/requirements.txt
```
Notebooks: [`[DEMO]_Ensemble_Learning.ipynb`](Modular_code/lib/[DEMO]_Ensemble_Learning.ipynb)

## Project structure
```
.gitignore
Modular_code/
  lib/
    [DEMO]_Ensemble_Learning.ipynb
  src/
    Engine.py
    ML_Pipeline/
    requirements.txt
README.md
```

## Credits
Based on a ProjectPro guided project.
