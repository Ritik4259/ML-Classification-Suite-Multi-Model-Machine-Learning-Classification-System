# ML Classification Suite  
A modular machine learning system implementing Logistic Regression, Decision Trees, and Support Vector Machines (SVM) across multiple datasets to analyze and compare model performance.

---

## Project Overview
The **ML Classification Suite** is a unified machine learning framework designed to explore how different classical ML algorithms perform on varied datasets. It follows a structured pipeline covering:

- Data loading  
- Preprocessing  
- Model training  
- Evaluation  
- Visualization  
- Comparative analysis  

This project was built entirely by me as part of my ongoing learning in machine learning.

---

## Problem Statement
Different datasets have different structures, levels of complexity, and decision boundaries.  
No single ML model performs best on every dataset.

This project solves the problem of understanding **which model works best for which dataset** by implementing and comparing three widely used classification algorithms.

---

## Tech Stack

**Language:**  
- Python 3.8+

**Libraries:**  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-Learn  

**Tools:**  
- Jupyter Notebook / Google Colab  

---

## System Architecture

                ┌───────────────────────┐
                │      Dataset Loader   │
                │  (student, diabetes)  │
                └──────────┬────────────┘
                           │
                ┌──────────▼────────────┐
                │     Data Preprocessor │
                │ (cleaning, encoding)  │
                └──────────┬────────────┘
                           │
          ┌────────────────┼─────────────────┐
          ▼                ▼                 ▼
┌────────────────┐  ┌───────────────┐  ┌────────────────┐
│ Logistic Reg.  │  │ Decision Tree │  │       SVM      │
└──────┬─────────┘  └──────┬────────┘  └─────────┬──────┘
       │                   │                     │
       └──────────────┬────┴───────────┬────────┘
                      ▼                ▼
             ┌────────────────┐  ┌──────────────────┐
             │ Model Metrics  │  │ Visualization    │
             └────────────────┘  └──────────────────┘


---

## Features

### Multi-dataset support  
- Diabetes dataset  
- Student performance dataset  
- Student scores dataset  

### Three machine learning models  
- Logistic Regression  
- Decision Tree Classifier  
- Support Vector Machine  

### Modular, reusable pipeline  
Each notebook includes:
- Data preprocessing  
- Model training  
- Evaluation  
- Visualizations  

### Visualization & comparison  
- Accuracy scores  
- Confusion matrix  
- Classification report  

---

## Models Used

| Model | Use-Case Strength | Trade-Off |
|-------|------------------|-----------|
| Logistic Regression | Linearly separable data | Limited on complex datasets |
| Decision Tree | Handles non-linear data | Overfits without pruning |
| SVM | High accuracy on scaled data | Computationally heavy |

---

## Metrics & Observations
- Logistic Regression performed best on linearly separable datasets.  
- Decision Trees performed well but showed signs of overfitting.  
- SVM achieved strong performance on the diabetes dataset after scaling.  

This highlights the importance of **choosing the right model for the right data**.
