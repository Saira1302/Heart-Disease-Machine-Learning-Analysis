# ❤️ Heart Disease Machine Learning Analysis

## 📌 Project Overview

This project applies **machine learning techniques to the Heart Disease dataset** to explore patterns in patient health data and compare different machine learning approaches.

The project covers the complete machine learning workflow, including **data understanding, preprocessing, feature encoding, feature scaling, regression, classification, clustering, dimensionality reduction, visualization, and model evaluation**.

Multiple machine learning models were trained and evaluated to compare their performance in predicting the presence of heart disease.

> **Note:** This project was completed as part of a university machine learning assignment for educational purposes. The models are not intended for medical diagnosis or clinical use.

---

## 🎯 Objectives

The main objectives of this project are to:

* Understand and preprocess the heart disease dataset
* Identify and handle missing values
* Clean and transform categorical variables
* Apply feature encoding and scaling
* Build and compare multiple machine learning models
* Evaluate classification performance using different metrics
* Apply regression to predict a continuous health variable
* Explore unsupervised learning using K-Means clustering
* Apply PCA for dimensionality reduction
* Analyze feature importance
* Compare the performance of different machine learning approaches

---

## 📊 Dataset

The project uses the **Heart Disease dataset**, containing patient health and clinical attributes.

Important features include:

* `age` — Age of the patient
* `sex` — Sex
* `cp` — Chest pain type
* `trestbps` — Resting blood pressure
* `chol` — Serum cholesterol
* `fbs` — Fasting blood sugar
* `restecg` — Resting electrocardiographic results
* `thalach` — Maximum heart rate achieved
* `exang` — Exercise-induced angina
* `oldpeak` — ST depression
* `slope` — Slope of the peak exercise ST segment
* `ca` — Number of major vessels
* `thal` — Thalassemia
* `target` — Heart disease target variable

---

# 🔄 Machine Learning Workflow

```text
Dataset
   ↓
Data Understanding
   ↓
Missing Value Handling
   ↓
Data Cleaning
   ↓
Categorical Encoding
   ↓
Feature Scaling
   ↓
Train/Test Split
   ↓
Machine Learning Models
   ↓
Model Evaluation
   ↓
Clustering & PCA
   ↓
Model Comparison
```

---

## 🧹 1. Data Understanding & Preprocessing

The dataset was first inspected to understand:

* Dataset dimensions
* Column data types
* Summary statistics
* Missing values
* Numerical and categorical features

Possible missing values represented by `?` were converted to `NaN` before further processing.

### Missing Value Handling

For numerical variables, missing values were handled using **median imputation**.

For categorical variables, **most frequent value imputation** was used.

---

## 🔤 2. Categorical Encoding

Several numerical columns represent categorical information.

The following variables were treated as categorical:

```text
sex
cp
fbs
restecg
exang
slope
ca
thal
```

Multi-class categorical variables were converted using **One-Hot Encoding**, while binary categorical variables were retained as binary values.

---

## ⚖️ 3. Feature Scaling

`StandardScaler` was used to standardize numerical features.

Feature scaling was particularly important for algorithms such as:

* K-Nearest Neighbors
* Artificial Neural Network

Tree based models generally do not require feature scaling.

---

# 🤖 Machine Learning Models

Several supervised and unsupervised learning techniques were implemented.

## 1. Linear Regression

Linear Regression was used as a regression model to predict **serum cholesterol (`chol`)** as a continuous target.

The model was evaluated using:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

---

## 2. Logistic Regression

Logistic Regression was used as a classification model to predict whether a patient belongs to the heart disease class.

---

## 3. Decision Tree

A Decision Tree Classifier was trained to identify patterns in the patient data.

A maximum depth was applied to control model complexity and reduce overfitting.

The decision tree was also visualized to understand its top-level decision rules.

---

## 4. Random Forest

A Random Forest Classifier was trained using multiple decision trees.

The model was also used to calculate **feature importance**, helping identify which features contributed most to the model's predictions.

---

## 5. K-Nearest Neighbors

KNN was tested with different values of `k`:

```text
k = 3
k = 5
k = 7
```

The accuracy of each configuration was compared and the best performing value of `k` was selected.

---

## 6. Naive Bayes

Gaussian Naive Bayes was implemented as another classification approach.

This provided a fast probabilistic baseline for comparison with the other classification models.

---

## 7. Artificial Neural Network

A simple Artificial Neural Network was implemented using **TensorFlow/Keras**.

The network contains:

* Input layer
* Dense hidden layer
* ReLU activation
* Dropout layer
* Sigmoid output layer

The model was trained for **50 epochs** using the Adam optimizer and binary cross-entropy loss.

Training and validation curves were also visualized.

---

# 🔬 Unsupervised Learning

## 8. K-Means Clustering

K-Means clustering was applied to selected numerical health features.

Two different cluster configurations were explored:

```text
k = 2
k = 3
```

The resulting clusters were visualized to explore patterns within the patient data.

---

## 9. Principal Component Analysis (PCA)

PCA was applied to reduce the dimensionality of the numerical features.

The explained variance ratio of the principal components was calculated to understand how much information each component retained.

The first two principal components were visualized and colored according to the target variable.


# 📏 Model Evaluation

The classification models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

A comparison table was created to compare the performance of the different classification algorithms.

For the regression model, the following metrics were used:

* R²
* MAE
* RMSE



## 📊 Models Compared

| Model                     | Type                     |
| ------------------------- | ------------------------ |
| Linear Regression         | Regression               |
| Logistic Regression       | Classification           |
| Decision Tree             | Classification           |
| Random Forest             | Classification           |
| KNN                       | Classification           |
| Naive Bayes               | Classification           |
| Artificial Neural Network | Classification           |
| K-Means                   | Clustering               |
| PCA                       | Dimensionality Reduction |



## 🛠️ Technologies & Libraries

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow
* Keras

### Environment

* Kaggle Notebook
* Jupyter Notebook

---

## 📈 Key Concepts Demonstrated

This project demonstrates practical experience with:

**Data Preprocessing**
**Missing Value Imputation**
**Categorical Encoding**
**Feature Scaling**
**Regression**
**Classification**
**Ensemble Learning**
**KNN**
**Naive Bayes**
**Artificial Neural Networks**
**Clustering**
**Dimensionality Reduction**
**Model Evaluation**
**Data Visualization**


---

## ⚠️ Disclaimer

This project is intended **for educational and academic purposes only**.

The predictions generated by the machine learning models should not be interpreted as medical advice, diagnosis, or a substitute for professional medical evaluation.

---


