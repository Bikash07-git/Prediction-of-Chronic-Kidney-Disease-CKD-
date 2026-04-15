# 🧠 Chronic Kidney Disease Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting **Chronic Kidney Disease (CKD)** using machine learning techniques. Early detection of CKD can significantly improve patient outcomes by enabling timely medical intervention.

The model is trained on the **UCI Machine Learning Repository CKD dataset**, which includes **24 clinical and demographic features** such as blood pressure, hemoglobin, albumin levels, and more.

The goal is to classify whether a patient has CKD (**Yes / No**) using various ML algorithms and compare their performance.

---

## 🎯 Objectives

* Perform data preprocessing and cleaning
* Train multiple machine learning models
* Evaluate models using performance metrics
* Deploy the best model with a user-friendly interface

---

## 🗂️ Project Structure

```
CKD-Prediction/
│── data/
│── notebooks/
│── src/
│── models/
│── results/
│── main.py
│── requirements.txt
│── README.md
```

---

## ⚙️ Tech Stack

* **Programming Language:** Python
* **Libraries:** pandas, numpy, matplotlib, seaborn, sklearn
* **Deep Learning:** TensorFlow, Keras
* **GUI:** tkinter

---

## 🔍 Workflow

### 1. Data Preprocessing

* Handling missing values
* Encoding categorical features
* Feature scaling and normalization

### 2. Model Training

Models used:

* Logistic Regression
* Decision Tree
* Random Forest
* Neural Network (Keras)

### 3. Model Evaluation

Evaluation metrics:

* Accuracy
* Precision
* Recall
* F1 Score

### 4. Deployment

* GUI-based application built using **tkinter**
* Allows users to:

  * Train model
  * Test model on new data

---

## 📊 Results

* Compared multiple models to identify best performance
* Random Forest / Neural Network achieved highest accuracy *(update this if needed)*

---

## 💻 Installation & Setup

### Step 1: Clone Repository

```bash
git clone https://github.com/Bikash07-git/chronic-kidney-disease-prediction.git
cd chronic-kidney-disease-prediction
```

### Step 2: Create Virtual Environment

```bash
python -m venv venv
```

#### Activate Environment

* Windows:

```bash
venv\Scripts\activate
```

* Linux/Mac:

```bash
source venv/bin/activate
```

---

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

---

### Step 4: Run Application

```bash
python main.py
```

---

## 🖥️ Usage

* Launch the application
* Choose:

  * **Train Model** → trains and saves model
  * **Test Model** → predicts CKD on new input

---

## 📈 Future Improvements

* Add web deployment (Flask / FastAPI)
* Improve model performance using feature engineering
* Add real-time prediction API
* Use advanced models like XGBoost / LightGBM

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙏 Acknowledgments

* Dataset: UCI Machine Learning Repository
* Contributors: Open-source community


---
