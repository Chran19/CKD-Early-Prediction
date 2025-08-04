# 🩺 Early Detection of Chronic Kidney Disease (CKD) Using Machine Learning

**A SmartInternz Internship Project**

---

## 📌 Overview

Chronic Kidney Disease (CKD) is a progressive condition that, if diagnosed early, can be effectively managed or even reversed. This project applies **machine learning techniques** to routine medical data in order to predict CKD risk, assist healthcare professionals with early diagnosis, and support patient survival analysis and disease monitoring.

Built during a machine learning internship at **SmartInternz**, this solution combines real-world medical scenarios with an end-to-end deployment pipeline using Flask and Python.

---

## 🔍 Key Use Cases

### 1. **Routine Test-Based Early Detection**

A patient undergoes a standard health check-up. Slight deviations in **creatinine**, **albumin**, or **hemoglobin** levels are picked up by the model, signaling early CKD risk.

### 2. **Personalized Treatment Planning**

Using past patient records, the system predicts the **severity** of CKD and estimates **survival chances**, helping physicians personalize treatment strategies.

### 3. **Long-Term Disease Monitoring**

For diagnosed patients, the model monitors **biomarker trends** across visits and alerts clinicians if deterioration is detected, prompting timely intervention.

---

## 🧠 Technologies Used

* **Python**
* **Pandas, NumPy, scikit-learn**
* **Flask (Web App Framework)**
* **Jupyter Notebook (Model Training & Analysis)**
* **Random Forest Classifier**
* **Pickle (Model Persistence)**

---

## 🗂️ Project Layout

```
├── Flask/                      # Web application interface
│   ├── app.py                  # Flask server
│   ├── templates/              # HTML UI
│   ├── static/                 # Styling assets
│   ├── CKD.pkl                 # Trained ML model
│   └── scaler.pkl              # Preprocessing pipeline
├── Training/
│   └── Chronic_kidney_disease_analysis.ipynb  # Data exploration & model training
├── dataset/
│   └── kidney_disease.csv     # Source medical dataset
├── test_ckd.py                # Automated testing script
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ckd-detection.git
cd ckd-detection
```

### 2. Create and Activate Virtual Environment

```bash
python -m venv .venv
source .venv/bin/activate      # On Windows: .venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Getting Started

### 🧪 Model Training

Launch the notebook in Jupyter:

```bash
cd Training
jupyter notebook Chronic_kidney_disease_analysis.ipynb
```

Run all cells to clean the dataset, train the model, and export `CKD.pkl` and `scaler.pkl`.

---

### 🌐 Running the Web App

```bash
cd Flask
python app.py
```

Then, open your browser and visit: [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

---

### 🧬 Automated Testing

From the project root:

```bash
python test_ckd.py
```

This script will send mock test data to the app and return predicted outcomes and probabilities.

---

## 📈 Results & Analysis

* Achieved **perfect accuracy** on internal test sets.
* Real-world test cases revealed minor **false positives/negatives**, indicating dataset bias or imbalance.
* Demonstrates strong potential for use in clinical decision support systems, with room for improvement in generalization.

---

## 🔧 Future Improvements

* Curate a larger, more balanced and representative dataset.
* Apply **cross-validation** and **ROC-AUC** analysis for better metric coverage.
* Explore **XGBoost**, **Ensemble Models**, or **SMOTE** for improved recall on minority classes.
* Build in **real-time data ingestion** for dynamic patient monitoring.

---

## 🎓 Internship Acknowledgment

This project was developed as part of the **SmartInternz Experiential Learning Program**, designed to bridge academic learning and real-world problem-solving in healthcare technology.

---

## 🤝 Contributing

If you're passionate about ML in healthcare and want to build on this foundation, feel free to fork the repo and contribute. PRs are welcome!

