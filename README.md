# Patient Readmission Prediction

This project focuses on predicting whether a patient will be readmitted to the hospital using machine learning.

The goal is to use patient data (age, medical history, visits, etc.) to identify high-risk cases early. This can help hospitals make better decisions and potentially reduce unnecessary readmissions.

---

## What I did

I built a full machine learning pipeline from scratch:

- Explored and cleaned the data  
- Created new features based on domain understanding  
- Trained multiple models  
- Compared model performance  
- Selected the best model  
- Tuned the classification threshold  
- Evaluated results using metrics and visualizations  

---

## Dataset

The dataset includes features such as:

- Age  
- Number of comorbidities  
- Length of hospital stay  
- Number of medications  
- Follow-up visits  
- Previous readmissions  
- Diagnosis and treatment details  

*Dataset is not included in this repo.*

---

## Feature Engineering

I created additional features to improve model performance, including:

- Interaction features (e.g. age × comorbidities)  
- Risk flags (elderly patients, complex cases, frequent visitors)  
- A simple manual risk score  
- Some non-linear combinations  

These helped capture patterns that aren’t obvious from the raw data.

---

## Models Used

- Logistic Regression (baseline)  
- Random Forest  
- Gradient Boosting  
- XGBoost  

Each model was trained and evaluated, and the best one was selected based on performance.

---

## Evaluation

I evaluated models using:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

Since this is a healthcare problem, I focused more on **recall** to reduce missed high-risk patients.

---

## Threshold Tuning

Instead of using the default 0.5 threshold, I tuned it using the precision-recall curve to improve performance.

This helped:
- Increase recall  
- Improve F1 score  
- Reduce false negatives  

I also compared results before and after tuning.

---

## Results

- Tree-based models performed better than the baseline  
- Feature engineering improved performance  
- Threshold tuning made the model more effective at identifying high-risk patients  

---

## How to run

Clone the repo:
