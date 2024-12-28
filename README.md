This repository contains the code for our submission to the "Repeat Buyers Prediction-Challenge the Baseline" competition hosted by T-Mall on [Tianchi](https://tianchi.aliyun.com/competition/entrance/231576). Our approach secured the 7th position out of 39,037 teams. The team operated under two accounts: "Bryan Constantine Sadihin" and "Made in Tsinghua".

![alt text](image.png)

# Getting Started
## Prerequisites
Before running the code, download the datasets from the competition's website.

# Installation
Clone the repository and navigate to the downloaded folder. Place the datasets into the repository's root directory according to the following structure:
- `data_format1/data_format1/csv_files`
- `data_format1/csv_files`
- `data_format2/... (similar structure as data_format1)`

# Usage
This project is divided into two main phases: Feature Engineering and Model Training. Below are the descriptions and instructions for each Jupyter notebook used.

## Feature Engineering Phase
- ``double11.ipynb``: Extracts features related to the promotion day (11-11).
- ``matteo_notebook.ipynb``: Uses tf-idf for extracting semantic instances.
- ``work_bryan.ipynb``: Applies dense vector embeddings for semantic instance extraction and explores different aggregation methods.
- ``shei_franklin_features.ipynb``: Generates count-based features, diversity features, penetration, demographic information, and applies dimensionality reduction.
The combined features from `double11.ipynb` and `shei_franklin_features.ipynb` are available for download:
- [X features](https://drive.google.com/file/d/1PbyqG8q9Ulfet8ip22nWPXkDoPe4S4c4/view)
- [X features](https://drive.google.com/file/d/1K4SnrmmkbP1ffHHWuXtTLqx1eIskZuvt/view?usp=sharing )

## Model Training Phase
- ``deepFm.ipynb``: Trains a model using Deep Factorization Machine (DeepFM).
- ``franklin.ipynb``: Trains models using XGBoost and LightGBM. The best-performing model, an XGB model (xgb_model_best_noID.bin), is used for the final predictions.

# Project Report
The detailed project report will be uploaded shortly.