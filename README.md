# 🧠 Chronic Kidney Disease Prediction Using Machine Learning (Decision Tree)

A machine learning project for predicting **Chronic Kidney Disease (CKD)** using clinical and demographic patient data. The project implements data preprocessing, exploratory data analysis, feature transformation, model training, prediction, and performance comparison using traditional machine learning algorithms.

The complete workflow is implemented in a **Jupyter Notebook** using Python and Scikit-learn.

---

## 📌 Project Overview

Chronic Kidney Disease is a major health condition that can be difficult to identify in its early stages. This project explores the application of machine learning classification techniques to predict CKD from patient health-related attributes.

The project uses the **UCI Chronic Kidney Disease dataset**, containing clinical and demographic features such as:

* Age
* Blood Pressure
* Specific Gravity
* Albumin
* Sugar
* Blood Glucose
* Blood Urea
* Serum Creatinine
* Sodium
* Potassium
* Hemoglobin
* Packed Cell Volume
* White Blood Cell Count
* Red Blood Cell Count
* Hypertension
* Diabetes Mellitus
* Coronary Artery Disease
* Appetite
* Pedal Edema
* Anemia
* Other clinical indicators

The target variable classifies patients into:

```text
CKD
Not CKD
```

---

## 🎯 Project Objectives

* Analyze the CKD dataset
* Understand the structure and characteristics of the data
* Identify missing and inconsistent values
* Perform data cleaning and preprocessing
* Analyze important clinical features through EDA
* Convert categorical variables into numerical representations
* Prepare features for machine learning
* Train multiple classification algorithms
* Generate predictions on test data
* Evaluate and compare model performance
* Identify the best-performing model based on the experiments

---

# 🔄 Machine Learning Execution Flow

```text
┌───────────────────────────────────────────┐
│              CKD DATASET                  │
│       UCI Chronic Kidney Disease          │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│          DATA UNDERSTANDING               │
│                                           │
│  • Shape                                  │
│  • Features                               │
│  • Data Types                             │
│  • Statistical Information                │
│  • Target Distribution                    │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│             DATA CLEANING                 │
│                                           │
│  • Missing Values                         │
│  • Duplicate/Invalid Values               │
│  • Data Type Correction                   │
│  • Inconsistent Categories                │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│        EXPLORATORY DATA ANALYSIS          │
│                                           │
│  • Feature Distributions                  │
│  • Target Distribution                    │
│  • Correlation Analysis                   │
│  • Statistical Analysis                   │
│  • Data Visualization                     │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│          DATA PREPROCESSING               │
│                                           │
│  • Missing Value Treatment                │
│  • Categorical Encoding                   │
│  • Feature Transformation                 │
│  • Feature Scaling                        │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│           TRAIN-TEST SPLIT                │
│                                           │
│        Training Data | Test Data          │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
          ┌───────────┴───────────┐
          │                       │
          ▼                       ▼
┌───────────────────┐   ┌───────────────────┐
│ LOGISTIC          │   │ DECISION TREE     │
│ REGRESSION        │   │ CLASSIFIER        │
└─────────┬─────────┘   └─────────┬─────────┘
          │                       │
          └───────────┬───────────┘
                      │
                      ▼
            ┌───────────────────┐
            │   RANDOM FOREST   │
            │    CLASSIFIER     │
            └─────────┬─────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│            MODEL PREDICTION               │
│                                           │
│     Predictions on Unseen Test Data       │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│          MODEL PERFORMANCE                │
│                                           │
│  • Accuracy                               │
│  • Precision                              │
│  • Recall                                 │
│  • F1 Score                               │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│          MODEL COMPARISON                 │
│                                           │
│  Compare classification performance       │
│  and identify the best-performing model   │
└─────────────────────┬─────────────────────┘
                      │
                      ▼
┌───────────────────────────────────────────┐
│          CKD PREDICTION                   │
│                                           │
│        CKD  /  NOT CKD                    │
└───────────────────────────────────────────┘
```

---

## 🗂️ Dataset

### Dataset Source

**Chronic Kidney Disease Dataset — UCI Machine Learning Repository**

The dataset contains **400 patient records** and **24 input features** related to clinical and demographic characteristics.

### Feature Categories

#### Demographic Features

* Age

#### Clinical Measurements

* Blood Pressure
* Specific Gravity
* Albumin
* Sugar
* Blood Glucose Random
* Blood Urea
* Serum Creatinine
* Sodium
* Potassium
* Hemoglobin
* Packed Cell Volume
* White Blood Cell Count
* Red Blood Cell Count

#### Clinical Conditions

* Hypertension
* Diabetes Mellitus
* Coronary Artery Disease
* Pedal Edema
* Anemia

#### Other Clinical Indicators

* Red Blood Cells
* Pus Cell
* Pus Cell Clumps
* Bacteria
* Appetite

### Target

```text
ckd      → Chronic Kidney Disease
notckd   → No Chronic Kidney Disease
```

---

## 🧹 Data Preprocessing

The dataset requires preprocessing before it can be used for machine learning.

The notebook performs the following preprocessing operations:

* Identification of missing values
* Handling missing numerical values
* Handling missing categorical values
* Removal of unnecessary columns
* Cleaning inconsistent values
* Conversion of categorical values
* Encoding categorical features
* Numerical feature transformation
* Feature scaling where required
* Separation of features and target variable

---

## 📊 Exploratory Data Analysis

The notebook performs exploratory analysis to understand the dataset and identify relationships between features.

EDA includes:

* Dataset structure analysis
* Descriptive statistics
* Missing-value analysis
* Target-class distribution
* Numerical feature distributions
* Categorical feature analysis
* Feature correlation
* Relationship between clinical variables
* Visualization of important features

### Visualization Libraries

* Matplotlib
* Seaborn

---

## 🤖 Machine Learning Models

The project implements and compares the following machine learning algorithms:

### Logistic Regression

Used as a classification model for predicting the binary CKD target.

### Decision Tree Classifier

A tree-based classification algorithm used to identify decision patterns between clinical features and the target.

### Random Forest Classifier

An ensemble classification algorithm consisting of multiple decision trees.

---

## ⚙️ Model Training

After preprocessing, the dataset is divided into training and testing subsets.

The training process consists of:

```text
Preprocessed Dataset
        │
        ▼
Feature / Target Separation
        │
        ▼
Train-Test Split
        │
        ▼
Model Initialization
        │
        ▼
Model Training
        │
        ▼
Test Data Prediction
        │
        ▼
Performance Evaluation
```

Each machine learning model is trained using the prepared training dataset and evaluated against the test dataset.

---

## 📈 Model Performance Comparison

The performance of the trained models is compared using:

* Accuracy
* Precision
* Recall
* F1 Score

The experiments showed that the **Decision Tree model achieved the highest observed accuracy, approximately in the 87%–93% range**, depending on the experimental configuration.

The notebook contains the model-specific evaluation outputs and comparison of the implemented algorithms.

---

## 🧪 Prediction Workflow

Once the models are trained, the test dataset is passed through the trained models.

```text
┌───────────────────────┐
│    New Patient Data   │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│ Same Preprocessing    │
│ Transformation        │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│ Trained ML Model      │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│      Prediction       │
├───────────────────────┤
│     CKD / NOT CKD     │
└───────────────────────┘
```

---

## 📓 Jupyter Notebook

The entire implementation is contained within the Jupyter Notebook.

The notebook covers:

```text
01. Import Libraries
02. Load Dataset
03. Dataset Inspection
04. Data Cleaning
05. Missing Value Analysis
06. Exploratory Data Analysis
07. Data Preprocessing
08. Feature Encoding
09. Feature Scaling
10. Train-Test Split
11. Logistic Regression
12. Decision Tree
13. Random Forest
14. Model Predictions
15. Model Evaluation
16. Model Comparison
17. CKD Classification
```
---

## 🛠️ Tech Stack

| Category                  | Technology       |
| ------------------------- | ---------------- |
| Language                  | Python           |
| Environment               | Jupyter Notebook |
| Data Manipulation         | Pandas           |
| Numerical Computing       | NumPy            |
| Visualization             | Matplotlib       |
| Statistical Visualization | Seaborn          |
| Machine Learning          | Scikit-learn     |

---

## 📦 Python Libraries

The project primarily uses:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

## ⚙️ Installation & Setup

### Clone the Repository

```bash
git clone https://github.com/Bikash07-git/chronic-kidney-disease-prediction.git
```

```bash
cd chronic-kidney-disease-prediction
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Linux / macOS

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
CKD_Prediction.ipynb
```

Run the notebook cells sequentially to reproduce the analysis and machine learning workflow.

---

## 📌 Key Project Components

```text
┌───────────────────────────────────────────────┐
│              PROJECT COMPONENTS               │
├───────────────────────────────────────────────┤
│                                               │
│  ✓ Healthcare Dataset Analysis               │
│  ✓ Data Cleaning                             │
│  ✓ Missing Value Handling                    │
│  ✓ Exploratory Data Analysis                 │
│  ✓ Categorical Feature Encoding              │
│  ✓ Feature Scaling                           │
│  ✓ Train-Test Data Splitting                 │
│  ✓ Multiple ML Classification Models         │
│  ✓ Model Prediction                          │
│  ✓ Performance Evaluation                    │
│  ✓ Model Comparison                          │
│                                               │
└───────────────────────────────────────────────┘
```

---

## 🔮 Future Improvements

* Hyperparameter tuning
* K-Fold cross-validation
* Advanced feature selection
* Improved handling of class imbalance
* ROC-AUC analysis
* Precision-Recall curve analysis
* Feature importance analysis
* Model explainability
* Experiment with additional ML algorithms
* Model serialization for future predictions
* Web-based deployment
* REST API integration
  
---

## 📚 References

* UCI Machine Learning Repository — Chronic Kidney Disease Dataset
* Scikit-learn Documentation
* Pandas Documentation
* NumPy Documentation
* Matplotlib Documentation
* Seaborn Documentation

---

## 👨‍💻 Author

**Bikash Sagar Koiri**

Data Analyst | Machine Learning | AI & Research

---

⭐ If you found this project useful, consider giving the repository a star.
