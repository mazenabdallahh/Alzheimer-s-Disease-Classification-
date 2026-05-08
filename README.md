# Alzheimer's Disease Classification

Built and compared predictive models using **XGBoost**, **Gradient Boosting**, and **Random Forest**, with emphasis on accuracy optimization, feature importance analysis, and reliable disease prediction

## Project Overview
This repository focuses on the development of a diagnostic classification tool for Alzheimer's Disease.  
By leveraging patient clinical data, lifestyle metrics, and cognitive assessments, this project provides a high‑accuracy predictive framework to assist in early detection and risk assessment.  

The project evaluates multiple ensemble learning techniques to identify the most robust model for clinical classification, ensuring high sensitivity and specificity in distinguishing between healthy and affected individuals.

##  Core Features
- **Data Engineering**: Automated cleaning of clinical datasets, including removal of non‑predictive identifiers like *PatientID* and *DoctorInCharge*.  
- **Exploratory Analysis**: Statistical visualization of demographic impacts and clinical correlations, identifying key features like *MMSE* and *Functional Assessment*.  
- **Multi‑Model Framework**: Comparative implementation of Random Forest, XGBoost, and Gradient Boosting architectures.  
- **Performance Optimization**: Systematic hyperparameter tuning via *GridSearchCV* to maximize testing accuracy.  
- **Reliability Metrics**: Evaluation using ROC‑AUC curves, confusion matrices, and a detailed performance summary table to monitor for overfitting.  

##  Dataset Structure
The analysis is performed on a clinical dataset containing **2,149 patient records** with the following feature categories:

- **Demographics**: Age, Gender, Ethnicity, Education Level  
- **Health Metrics**: BMI, Smoking status, Physical activity, Diet Quality  
- **Medical History**: Family history of Alzheimer's, Cardiovascular health, Diabetes, Hypertension  
- **Clinical Assessment**: MMSE (Mini‑Mental State Examination), ADL (Activities of Daily Living), Functional Assessment scores  
- **Target Variable**: Diagnosis (Binary: 0 = No Alzheimer's, 1 = Alzheimer's)
- 
##  Results

| Model              | Training Accuracy | Testing Accuracy | Gap    | Status |
|--------------------|------------------|-----------------|--------|--------|
| Random Forest      | 95.89%           | 96.28%          | -0.39% | ✓ Good |
| XGBoost            | 97.21%           | 96.28%          | 0.92%  | ✓ Good |
| Gradient Boosting  | 96.17%           | 96.28%          | -0.12% | ✓ Good |

**AUC‑ROC Performance**  
- Random Forest: 0.9571  
- XGBoost: 0.9554  
- Gradient Boosting: 0.9539  

---

##  Tech Stack
- **Language**: Python  
- **Machine Learning**: Scikit‑learn, XGBoost  
- **Data Analysis**: Pandas, NumPy  
- **Visualization**: Matplotlib, Seaborn  

---

##  How to Use

### Clone the repository
```bash
git clone https://github.com/mazenabdallahh/Alzheimer-s-Disease-Classification-.git
