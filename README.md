# Sentiments Analysis ML Project (Complete Pipline)

This repository contains a complete machine learning pipeline for **sentiment analysis** of product reviews using Python and scikit-learn.

The project was developed as part of a learning module, where we demonstrated all typical phases of a machine learning workflow from raw data to a ready-to-use trained model.

---

## Project structure

|- data/

| ---product_reviews_full.csv # dataset

|- notebook/

| ---exploratory_analysis.ipynb # EDA and preprocessing

|- src/

| ---train_model.py # Script for training and saving the model
| ---test_model.py # Script for testing saved model

|-README.md

## What We Did in This Module

Through this module, we covered all major steps of a real-world ML project:

### 1. Project Setup
- Created a new GitHub repository
- Defined project folder structure
- Uploaded raw dataset

### 2. Data Exploration
- Loaded and analyzed a large dataset with product reviews
- Used *matplotlib* and *seaborn* for visualisation
- Investigated distribution of sentiments and text characteristics

### 3. Data Cleaning & Preprocessing
- Removed missing values
- Standardized sentiments labels (positive/negative/neutral)
- Parsed and validated prices
- Converted review text to numerical lenght

### 4. Feature Engineering
- Selected meaningful input features: *review_title*, *review_text*, and *review_lenght*
- Removed irrelevant columns
- Explored correlation between price and sentiment 

### 5. Model Training & Evaluation
- Compared multiple ML models(Logistic Regression, Naive Bayes, Decision Tree, Random Forest, SVM)
- Used *Column Transformer* and *Pipeline* for unified preprocessing
- Evaluated using precision, recall, F1-score and confusion matrix

### 6. Final Model Training
- Trained final model on full dataset
- Saved the pipeline using * joblib* to *sentiment_model.pkl

### 7. Inference & Usage 
- Loaded saved model 
- Built an interactive interface for predicting sentiment of new reviews
- Enabled real-time testing via console input

### How to Use
```bash
cd src
python train_model.py
```
This will create a file called sentiment_model.pkl in the root directory.

### Run Inference
- Use the interactive script (model_test.py) to classify new reviews using the trained model.

### Author 
- This repository was developed as part of an educational program on practical machine learning using Python. All steps were carefully documented and modularized to help students understand and reproduce the entire workflow. 

### License$
- This project is open-sourse  and freely available for educational use.