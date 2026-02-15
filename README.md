# Sports vs Politics Text Classification

## Natural Language Understanding  
Assignment-1

## Overview

This project implements a machine learning pipeline to classify text into:

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
6. Interpretation
   
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

| Model Used | Feature Extraction Technique | Accuracy |
|--------|----------|----------|
| Naive Bayes | BoW | 97.54% |
| Logistic Regression | TF-IDF | 97.73% |
| SVM | TF-IDF | 97.62% |


---

## Confusion Matrix

<img width="1772" height="490" alt="image" src="https://github.com/user-attachments/assets/77986c96-56b3-4a80-840d-1b34817478ec" />

---

## Key Observations

- Logistic Regression achieved the highest accuracy (97.73%), closely followed by SVM and Naive Bayes.
- TF-IDF features slightly outperformed raw Bag of Words, indicating that term weighting improves discriminative power.
- The high accuracy across all models suggests strong vocabulary separation between Sports and Politics articles.
- Most misclassifications occurred in cases where articles contained overlapping contextual terms (e.g., political leaders attending sports events).
- Linear models performed extremely well due to the high-dimensional sparse nature of textual data.
- The dataset’s balanced class distribution contributed to stable and unbiased model performance.


---
## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
---

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/StutiYadav4/sports-politics-classifier.git
```
---
## Author

Stuti Yadav  
Roll Number: B23CH1044
