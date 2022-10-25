# Snowpark Handson-Lab for Credit Card Approval Prediction
This repository contains resources to get first handson experience with Snowpark.

### Use-Case: Credit Card Approval Prediction
You are part of a team of data engineers and data scientists at a banking company that has been tasked to identify high-risk customers using a machine learning based solution. The goal is to give a recommendation to either approve or reject the issueing of a credit card.

To build this, you have access to customer demographic and credit history data. Using Snowpark, we will ingest, analyze and transform this data to train a model that will then be deployed inside Snowflake to score new data.

The dataset you are using is part of a Kaggle competition that can be found here:\
[Kaggle: Credit Card Approval Prediction](https://www.kaggle.com/datasets/rikdifos/credit-card-approval-prediction)

### What you'll learn
* Loading and transforming data via Snowpark
* Defining Stored Procedures for non-SQL-based Data Transformations
* Defining Stored Procedures for training different machine learning models
* Defining User Defined Functions for distributed scoring of machine learning models
* Using hyper paratemer tuning in Stored Procedures

### What you’ll build 
You will build an end-to-end data science workflow leveraging Snowpark for Python
- to load, clean and prepare data
- to train different machine learning models using Python Stored Procedures
- to deploy the trained models in Snowflake using Python User Defined Functions (UDFs)

### Requirements
- A free [Snowflake Trial Account](https://signup.snowflake.com/) 
- [Anaconda Integration enabled by ORGADMIN](https://docs.snowflake.com/en/developer-guide/udf/python)
- Python 3.8

### Setup
First, clone the source code for this repo to your local environment:
```bash
git clone https://github.com/michaelgorkow/snowpark_hol_frauddetection.git
cd snowpark_hol_frauddetection
```

If you are using [Anaconda](https://www.anaconda.com/products/distribution) on your local machine, create a conda env for this quickstart:
```bash
conda env create -f conda_env.yml
conda activate pysnowpark
```

Conda will automatically install `snowflake-snowpark-python==0.10.0` and all other dependencies for you.

Now, launch Jupyter Notebook on your local machine:
```bash
jupyter notebook
```

If you decide to bring your own Python environment, please make sure to have the following packages installed:
- [Snowpark](https://pypi.org/project/snowflake-snowpark-python/)
- [Pandas](https://pypi.org/project/snowflake-snowpark-python/)
- [NumPy](https://pypi.org/project/numpy/)
- [scikit-learn](https://pypi.org/project/scikit-learn/)
- [LightGBM](https://pypi.org/project/lightgbm/)
- [XGBoost](https://pypi.org/project/xgboost/)
- [SciPy](https://pypi.org/project/scipy/)
- [Seaborn](https://pypi.org/project/seaborn/)
- [cloudpickle](https://pypi.org/project/cloudpickle/)
- [cachetools](https://pypi.org/project/cachetools/)
- [imbalanced-learn](https://pypi.org/project/imbalanced-learn/)
- [optuna](https://pypi.org/project/optuna/)