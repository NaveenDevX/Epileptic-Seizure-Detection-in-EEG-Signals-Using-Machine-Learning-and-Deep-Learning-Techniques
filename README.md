# 🧠 Epileptic Seizure Detection in EEG Signals Using Machine Learning and Deep Learning Techniques

## 📑 Table of Contents
- [🚀 Demo](#-demo)
- [📘 Overview](#-overview)
- [🎯 Motivation](#-motivation)
- [🔍 Technical Aspect](#-technical-aspect)
- [⚙️ Installation](#️-installation)
- [▶️ Run](#️-run)
- [🚢 Deployment (Heroku)](#-deployment-heroku)
- [🗂️ Directory Tree](#️-directory-tree)
- [📌 To Do](#-to-do)
- [🐞 Bug / Feature Request](#-bug--feature-request)
- [🧰 Technologies Used](#-technologies-used)
- [📄 License](#-license)
- [🙌 Credits](#-credits)

---

## 🚀 Demo

🔗 **Live Web App**: [Visit here](https://your-app-link.streamlit.app)  
*(Replace with your deployed Streamlit Heroku URL)*

---

## 📘 Overview

This project is designed to detect epileptic seizures from EEG (Electroencephalogram) signals using a combination of machine learning and deep learning models.  
The application performs data preprocessing, model prediction, and offers an intuitive web interface for real-time use.  
The goal is to assist medical professionals and researchers with a tool for early and accurate seizure detection.

---

## 🎯 Motivation

Seizures can occur unpredictably, and timely detection is crucial for medical intervention and patient safety.  
Manual EEG interpretation requires trained neurologists and can be error-prone due to subjectivity.  
With AI and data science, there's an opportunity to automate and standardize seizure recognition.  
This project was inspired by the potential of AI to democratize access to neurological diagnostics.  
A deployable web interface further enables wide-scale usage in both urban and rural healthcare settings.

---

## 🔍 Technical Aspect

### 🔹 Part 1: Machine Learning & Deep Learning Pipeline

- **Dataset**: UCI Epileptic Seizure Recognition Dataset  
- **Preprocessing Steps**:
  - Signal normalization
  - Dimensionality reduction
  - Feature extraction
  - Label encoding and class balancing

- **Machine Learning Models Used**:
  - Random Forest
  - XGBoost
  - Decision Tree
  - Logistic Regression

- **Deep Learning Models Used**:
  - 1D Convolutional Neural Network (CNN)
  - Deep Neural Network (DNN)

- **Evaluation Metrics**:
  - Accuracy, Precision, Recall, F1-Score
  - ROC-AUC Curve
  - Confusion Matrix

---

### 🔹 Part 2: Streamlit Web App

- Upload EEG CSV files
- Backend loads pretrained ML/DL models
- Real-time inference with result display
- Visualization of input signal and prediction results
- Interactive and responsive frontend using Streamlit

---

## ⚙️ Installation

### Step 1: Clone Repository
```bash
git clone https://github.com/yourusername/epileptic-seizure-predictor.git
cd epileptic-seizure-predictor
```

### Step 2: Create Virtual Environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate    # macOS/Linux
venv\Scripts\activate       # Windows
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

---

## ▶️ Run

### 🐧 For Linux/macOS:
```bash
streamlit run app.py
```

### 🪟 For Windows:
```bash
streamlit run app.py
```

---

## 🚢 Deployment (Heroku)

### 💡 Step-by-step Guide

#### 1️⃣ Prepare Streamlit App
Ensure your `app.py` runs successfully using:
```bash
streamlit run app.py
```

#### 2️⃣ Create Heroku App Files
- `requirements.txt` – Python packages
- `Procfile` – Heroku entry point  
  ```bash
  web: streamlit run app.py
  ```
- `runtime.txt` – (Optional) Define Python version
- Optional: `setup.sh` if required for Streamlit

#### 3️⃣ Push to Heroku
```bash
heroku login
heroku create seizure-predictor-app
git add .
git commit -m "Initial commit for deployment"
git push heroku main
heroku open
```

---

## 🗂️ Directory Tree

```
epileptic-seizure-predictor/
├── app.py
├── model/
│   ├── cnn_model.h5
│   └── rf_model.pkl
├── utils/
│   ├── preprocess.py
│   └── predict.py
├── data/
│   └── sample_eeg.csv
├── assets/
│   └── architecture.png
├── requirements.txt
├── Procfile
├── README.md
└── LICENSE
```

---

## 📌 To Do

- Real-time EEG data stream integration
- Extend support for multi-class classification of seizure types
- Model explainability with SHAP and LIME
- Mobile-friendly UI deployment (Streamlit Sharing / Flutter)
- REST API support for external integration

---

## 🐞 Bug / Feature Request

If you encounter a bug or want to request a feature:

- [Open an issue](https://github.com/yourusername/epileptic-seizure-predictor/issues)
- Include steps to reproduce or expected features
- Include relevant input files or screenshots

---

## 🧰 Technologies Used

| Technology            | Badge |
|-----------------------|-------|
| ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white) | Core programming language |
| ![NumPy](https://img.shields.io/badge/-NumPy-013243?logo=numpy&logoColor=white) | Numerical computations |
| ![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas&logoColor=white) | Data manipulation |
| ![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?logo=plotly&logoColor=white) | Plotting library |
| ![Scikit-Learn](https://img.shields.io/badge/-Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white) | ML models and tools |
| ![XGBoost](https://img.shields.io/badge/-XGBoost-EC252D?logo=xgboost&logoColor=white) | Gradient boosting |
| ![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?logo=tensorflow&logoColor=white) | Deep learning framework |
| ![Keras](https://img.shields.io/badge/-Keras-D00000?logo=keras&logoColor=white) | High-level neural network API |
| ![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?logo=streamlit&logoColor=white) | UI development |
| ![Heroku](https://img.shields.io/badge/-Heroku-430098?logo=heroku&logoColor=white) | Web deployment |
| ![Pickle](https://img.shields.io/badge/-Pickle-6A737D?logo=python&logoColor=white) | Model serialization |

---

## 📄 License

This project is released under the [MIT License](LICENSE).  
You are free to use, modify, and distribute this software with proper attribution.

---

## 🙌 Credits

- **UCI Machine Learning Repository** for providing the EEG dataset  
- Open-source contributors for Python ML/DL packages  
- Research papers on EEG signal processing and seizure detection  
- Community support from Stack Overflow and GitHub Discussions

---

> Developed with dedication to assist healthcare innovation through AI ❤️
