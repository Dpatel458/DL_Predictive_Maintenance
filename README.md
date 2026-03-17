# ⚙️ Predictive Maintenance using Deep Learning

A deep learning-based predictive maintenance system designed to **identify potential machine failures** using structured sensor data.  
This project leverages **neural networks** along with **advanced data augmentation techniques** to handle limited and imbalanced industrial datasets.

---

## 📌 Overview

Predictive maintenance is critical in modern industries to reduce downtime and optimize operational efficiency.

> ⚠️ *Can we accurately predict machine failures using limited real-world data?*

This project addresses that by:
- Using a **small real dataset (~10,000 rows)**
- Expanding it to **40,000–50,000 samples**
- Applying **SMOTE-based augmentation techniques**
- Training a **deep neural network (DNN)** for multiclass failure prediction

---

## 🚀 Key Features

- 🔍 Predicts multiple types of machine failures  
- 🧠 Deep Learning model (Neural Network-based)  
- 📊 Handles **class imbalance using SMOTE variants**  
- ⚙️ Real-world industrial dataset  
- 🌐 Deployment-ready structure (Flask/local interface if applicable)  

---

## 📂 Dataset Description

The dataset consists of industrial machine parameters:

- Air temperature [K]  
- Process temperature [K]  
- Rotational speed [rpm]  
- Torque [Nm]  
- Tool wear [min]  
- Product type (categorical)  

### 🎯 Target Variable:

Multiclass classification:
- No Failure  
- Power Failure  
- Heat Dissipation Failure  
- Overstrain Failure  
- Tool Wear Failure  

---

## 📈 Data Augmentation Strategy

Due to limited data (~10k rows), the dataset was expanded using:

- **SMOTE (Synthetic Minority Oversampling Technique)**  
- **SMOTENC** (for categorical + numerical features)  
- **Borderline-SMOTE**  
- Other SMOTE variants  

📊 Result:
- Original: ~10,000 samples  
- Augmented: **40,000 – 50,000 samples**  

This significantly improved class balance and model performance.

---

## 🧠 Model Architecture

- Fully Connected Neural Network (FNN)  
- Dense layers with activation functions (ReLU)  
- Dropout for regularization  
- Softmax output for multiclass classification  

---

## ⚙️ Tech Stack

### 🧠 Machine Learning / Deep Learning
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Imbalanced-Learn](https://img.shields.io/badge/Imbalanced--Learn-SMOTE%20%7C%20SMOTENC%20%7C%20Borderline--SMOTE-purple?style=for-the-badge)

---

### 📊 Data Processing & Visualization
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)

---

### 🌐 Deployment
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)

---

### 💻 Development
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-DA5B0B?style=for-the-badge&logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

## 📊 Workflow

1. Data Preprocessing  
2. Handling Missing Values  
3. Encoding Categorical Features  
4. Data Augmentation (SMOTE variants)  
5. Train-Test Split  
6. Model Training (Neural Network)  
7. Evaluation & Metrics  
8. Deployment (optional)  

---

## 📉 Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## 🧪 Results

- Improved performance after data augmentation  
- Better class balance → improved minority class prediction  
- Neural networks outperformed traditional ML models in this setup  

---

## 🔮 Future Improvements

- 🔁 Use advanced architectures (Transformers for tabular data)  
- ⚡ Hyperparameter tuning (Optuna, Grid Search)  
- 🌍 Deploy on cloud (AWS / GCP)  
- 📡 Real-time IoT integration  
- 📊 Explainability (SHAP, LIME)  



