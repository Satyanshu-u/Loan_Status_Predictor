# 🏦 Loan Status Prediction using Machine Learning (Gradio + SVM)

This project is a machine learning model that predicts whether a loan application will be *approved or rejected, based on user details like income, credit history, and employment. It uses "Support Vector Machine (SVM)" for prediction and provides a simple web interface using "Gradio".



## 📌 Features

- Preprocessing of raw loan data (missing values, categorical encoding)
- Trains an 'SVM classification model'
- Launches an interactive 'Gradio app' for real-time loan status prediction
- Visualizes relationships between features and loan status using Seaborn
- Runs entirely in 'Google Colab'



## 📁 Files in This Repository

| File | Description |
|------|-------------|
| Loan_Status_Prediction.ipynb | Main Colab notebook with training and Gradio interface |
| requirements.txt | List of Python packages used |
| README.md | Project overview and instructions |
| train_u6lujuX_CVtuZ9i.csv |



## 📊 Dataset Description

- Source: [Loan Prediction Dataset - Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)
- Target variable: Loan_Status (Y = Approved, N = Not Approved)
- Features include:
  - Gender, Married, Dependents, Education
  - Applicant Income, Coapplicant Income
  - Loan Amount, Loan Term, Credit History
  - Property Area, Employment Type

---

## 🧠 Machine Learning Model

- "Algorithm": Support Vector Machine (SVM) from sklearn
- "Preprocessing":
  - Dropped rows with missing values
  - Converted categorical variables using replace()
  - Converted Loan_Status to 0 (Not Approved) and 1 (Approved)
- "Evaluation":
  - Model accuracy printed after training
  - Can be further evaluated using a confusion matrix or cross-validation



## 🧪 Gradio Interface

The Gradio UI allows users to enter loan details manually and get an instant prediction.

### Sample Interface:
```python
gr.Interface(fn=predict_loan_status, inputs=[...], outputs="text").launch()

> After running the final cell in the notebook, a link will appear. Click it to launch the app.





🚀 How to Run

1. Open the notebook in Google Colab: 


2. Install dependencies (first cell already includes this):

!pip install gradio pandas numpy seaborn scikit-learn


3. Run all cells to:

Preprocess data

Train SVM model

Launch Gradio app






📦 Requirements

Install dependencies using:

pip install -r requirements.txt

Contents of requirements.txt:

gradio
pandas
numpy
seaborn
scikit-learn






🙋‍♂ Author

Created by a beginner in machine learning as a practice project using:

Google Colab

Gradio

Scikit-learn

