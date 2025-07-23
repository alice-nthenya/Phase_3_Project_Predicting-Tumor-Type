- **Student Name:** Alice N. Muia  
- **Student Pace:** Part-time  
- **Scheduled Project Review Date/Time:** 23-07-2025  
- **Instructor Name:** George Kamundia  
- **Blog Post URL:** 


# Predicting Tumor Type (Benign vs. Malignant) Using Diagnostic Dat

## Overview
This project focuses on building machine learning models to classify breast tumors as **benign** or **malignant** based on diagnostic measurements. The goal is to support clinical decision-making by developing accurate, interpretable models that can assist medical professionals in early detection and treatment planning.

## Business and Data Understanding
Breast cancer remains a leading cause of death among women worldwide. Early diagnosis is crucial for improving survival rates. Healthneers, our stakeholders, are a group of healthcare innovators seeking data-driven solutions to enhance diagnostic workflows.

The dataset used in this project is the **Breast Cancer Wisconsin (Diagnostic) dataset**, which contains 569 records with features derived from digitized images of fine needle aspirate (FNA) tests. Each sample includes 30 numerical features describing tumor characteristics and a diagnosis label: `M` for malignant and `B` for benign.

## Modeling
We developed and evaluated three classification models:
- **Logistic Regression** (with `class_weight='balanced'` to handle class imbalance)
- **Decision Tree Classifier**
- **Random Forest Classifier**

The dataset was split into training and testing sets (80/20), and **feature scaling** was applied to improve performance for models sensitive to scale. For each model, we evaluated performance using standard classification metrics.

## Evaluation
Model performance was measured using:
- **Confusion Matrix**
- **Accuracy, Precision, Recall, F1-score**
- **ROC Curve and AUC**

All three models performed well, with **Random Forest** achieving the best overall performance:
- **Accuracy**: 96%
- **Precision & Recall**: 98% and 93% (for malignant class)
- **AUC**: High, indicating excellent model discrimination

## Conclusion
Machine learning models can be powerful tools in supporting medical diagnosis.  
- Logistic Regression offered a solid baseline with balanced results.  
- The Decision Tree was interpretable and still accurate.  
- **Random Forest** outperformed both, making it the **recommended model** for deployment.

We recommend that Healthneers integrate the Random Forest model into their diagnostic tools to improve early detection and treatment outcomes.