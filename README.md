# Sports vs Politics Text Classification

## Natural Language Understanding  
Assignment-1

## Overview

This project implements a machine learning pipeline to classify news articles into:

- Sports  
- Politics  

The dataset is derived from the AG News corpus. From the original four categories 
(World, Sports, Business, Sci/Tech), only the World and Sports classes were retained.  
The World class was relabeled as **Politics**, while the remaining categories were removed.

---
## Project Pipeline

1. Data Selection (AG News Dataset)
2. Data Cleaning and Preprocessing
3. Feature Extraction (BoW, TF-IDF)
4. Model Training (Naive Bayes, Logistic Regression, SVM)
5. Evaluation (Accuracy, Precision, Recall, F1-score)
6. Error Analysis and Interpretation
   
---
## Dataset Source

AG News Dataset  
https://www.kaggle.com/datasets/amananandrai/ag-news-classification-dataset

## Dataset

- Total samples used: 63,800  
- Balanced dataset (Sports vs Politics)  
- Title and description fields were concatenated into a single text feature  

---

## Feature Engineering

The following feature extraction techniques were used:

- Bag of Words (BoW)
- TF-IDF
- Unigram representation

---

## Models Compared

1. Multinomial Naive Bayes  
2. Logistic Regression  
3. Linear Support Vector Machine (SVM)

---

## Results

| Model | Feature | Accuracy |
|--------|----------|----------|
| Naive Bayes | BoW | 97.54% |
| Logistic Regression | TF-IDF | 97.73% |
| SVM | TF-IDF | 97.62% |

Logistic Regression achieved the highest accuracy.

---

## Confusion Matrix (SVM)

<img width="548" height="455" alt="image" src="https://github.com/user-attachments/assets/74d5ce08-f881-4ab4-a2fc-b250ed71db96" />


---

## Key Observations

- TF-IDF outperformed raw Bag of Words.
- All models achieved over 97% accuracy.
- Strong vocabulary separation exists between Sports and Politics articles.

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/StutiYadav4/sports-politics-classifier.git
