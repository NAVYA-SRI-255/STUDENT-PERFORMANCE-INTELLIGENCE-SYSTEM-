# STUDENT-PERFORMANCE-INTELLIGENCE-SYSTEM-
---

## 📌 Project Overview

This project is a Machine Learning-based system designed to analyze and predict student academic performance using multiple regression and classification algorithms. The system integrates **Linear Regression, Logistic Regression, and Decision Tree** models to build a complete predictive analytics pipeline for education data.

The system performs:
- 📈 Prediction of final exam scores  
- 🔁 Classification of Pass/Fail outcomes  
- 🌳 Categorization of student performance levels  

---

## 📂 Dataset

The dataset used in this project is the **Student Performance Dataset** from the UCI Machine Learning Repository.

🔗 UCI Dataset  
https://archive.ics.uci.edu/ml/datasets/Student+Performance  

🔗 Kaggle Dataset  
https://www.kaggle.com/datasets/larsen0966/student-performance-data-set  

---

## 🧾 Features Used

### 📌 Input Features
- 📚 studytime → Weekly study time  
- ❌ failures → Number of past class failures  
- 🏫 absences → Number of school absences  
- 🧪 G1 → First period grade  
- 🧪 G2 → Second period grade  

### 🎯 Target Variables
- 📈 G3 → Final grade (Regression target)  
- 🔁 Pass/Fail → Binary classification target  
- 🌟 Performance Level → Multi-class classification target  

---

## 🤖 Machine Learning Models Used

---

## 📈 Linear Regression

Used to predict continuous output (final marks).

### Mathematical Model
ŷ = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ

### Cost Function
MSE = (1/n) Σ (yᵢ − ŷᵢ)²

### Optimization
β := β − α ∂J(β)/∂β

### Evaluation Metrics
- 📉 Mean Squared Error (MSE)  
- 📈 R² Score  

---

## 🔁 Logistic Regression

Used for binary classification (Pass/Fail).

### Sigmoid Function
σ(z) = 1 / (1 + e^(−z))

Where:
z = β₀ + β₁x₁ + ... + βₙxₙ

### Decision Rule
- If σ(z) ≥ 0.5 → Pass  
- If σ(z) < 0.5 → Fail  

### Cost Function
J(β) = −(1/n) Σ [y log(ŷ) + (1 − y) log(1 − ŷ)]

### Evaluation Metrics
- Accuracy Score  
- Confusion Matrix  

---

## 🌳 Decision Tree

Used for classification of student performance levels.

### Splitting Criteria
Gini Index = 1 − Σ pᵢ²  

Entropy = − Σ pᵢ log₂(pᵢ)  

Information Gain = Entropy(parent) − Entropy(children)

### Output Classes
- 🔴 Low Performance  
- 🟡 Medium Performance  
- 🟢 High Performance  

---

## 🧠 Machine Learning Pipeline

### Step 1: Data Collection
Dataset is collected from the UCI Machine Learning Repository.

### Step 2: Data Preprocessing
- Feature selection:
  - studytime, failures, absences, G1, G2  
- Target creation:
  - G3 for regression  
  - Pass/Fail for classification  
  - Performance categories  
- Train-test split (80/20)

### Step 3: Exploratory Data Analysis (EDA)
- Distribution of grades  
- Correlation analysis  
- Relationship between study habits and performance  

### Step 4: Model Training
- Linear Regression  
- Logistic Regression  
- Decision Tree Classifier  

### Step 5: Model Evaluation
- MSE, R² Score  
- Accuracy Score  
- Confusion Matrix  

### Step 6: Prediction System
Integrated system that predicts:
- Final marks  
- Pass/Fail outcome  
- Performance category  

---

## 🔄 System Workflow

Input Student Data  
↓  
Data Preprocessing  
↓  
Machine Learning Models  
↓  
Final Predictions:
- 📈 Marks Prediction  
- 🔁 Pass/Fail Prediction  
- 🌳 Performance Classification  

---

## ⚙️ Installation

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
