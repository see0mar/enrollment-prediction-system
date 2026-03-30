# Student Enrollment Prediction System

## Project Overview
A production-ready machine learning system that predicts student enrollment probability with 92% precision, achieving 186% improvement over baseline while reducing resource waste by 66%. Built during a 5-week data science internship in collaboration with Saint Louis University admissions data.

## Key Results
- **Precision:** 92.1% (when focusing on high-priority students)
- **ROC-AUC:** 0.996 (near-perfect discrimination)
- **Improvement:** +186% over traditional random outreach
- **Resource Efficiency:** 66% reduction in wasted outreach efforts

## Repository Structure
├── data/ # Raw and processed data (PII masked)
├── notebooks/ # Jupyter notebooks with full analysis
│ └── enrollment_prediction.ipynb
├── models/ # Saved model artifacts
│ └── enrollment_predictor.pkl
├── outputs/ # Visualizations and reports
├── deployment/ # Production-ready prediction module
│ └── predictor.py
├── requirements.txt # Python dependencies
└── README.md


## Installation
```bash
git clone https://github.com/yourusername/enrollment-prediction.git
cd enrollment-prediction
pip install -r requirements.txt
Usage
python
from deployment.predictor import EnrollmentPredictor

# Load model
predictor = EnrollmentPredictor.load('models/enrollment_predictor.pkl')

# Predict for new students
probabilities = predictor.predict_proba(student_data)
Methodology
Data Cleaning & Feature Engineering – 7 optimal features identified

Model Comparison – Logistic Regression, Random Forest, Gradient Boosting, SVM

Production Deployment – Encapsulated predictor with confidence scoring

Business Impact – Quantified resource optimization and success lift

Technologies Used
Python 3.12

pandas, numpy, scikit-learn, matplotlib, seaborn

Google Colab Notebook, joblib

Author
Omar Eltokhy – LinkedIn

License
This project is for portfolio demonstration. Data used with permission from Excelerate supported by Saint Louis University (PII masked).
