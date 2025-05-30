# 🧠 Epileptic Seizure Detection in EEG Signals Using Machine Learning and Deep Learning Techniques

## 📑 Table of Contents
- [🔗 Demo](#-demo)
- [📌 Overview](#-overview)
- [🚀 Motivation](#-motivation)
- [🧪 Technical Aspect](#-technical-aspect)
- [⚙️ Installation](#️-installation)
- [▶️ Run](#-run)
- [🌍 Deployment (Heroku)](#-deployment-heroku)
- [📂 Directory Tree](#-directory-tree)
- [📈 To Do](#-to-do)
- [🐛 Bug / Feature Request](#-bug--feature-request)
- [🧰 Technologies Used](#-technologies-used)
- [📜 License](#-license)
- [🙌 Credits](#-credits)

---

## 🔗 Demo
**Live Web App**: [Click here to try the app](https://your-app-link.streamlit.app) *(Replace this with your real link after deployment)*

---

## 📌 Overview
This project focuses on early detection of epileptic seizures using EEG signal data.  
We developed both machine learning and deep learning models to classify seizure vs. non-seizure signals.  
A Streamlit-based web interface makes it accessible and interactive for public use.

---

## 🚀 Motivation
Epileptic seizures are often unpredictable and life-threatening if not addressed quickly.  
The motivation behind this project was to build a lightweight, accurate system to detect seizure activity from EEG data.  
We aimed to use machine learning and deep learning for their rapid and scalable analysis capability.  
Deploying this solution as a web app allows healthcare professionals or patients to access predictions easily.  
It’s a step toward using AI for real-world health applications that can make a difference.

---

## 🧪 Technical Aspect

### 🔹 Part 1: Machine Learning & Deep Learning
- **Dataset Used**: UCI Epileptic Seizure Recognition Dataset  
- **Preprocessing**: Normalization, reshaping EEG segments, label encoding  
- **ML Models**: Random Forest, Decision Tree  
- **DL Models**: Convolutional Neural Networks (CNNs), Fully Connected Networks (FCNs)  
- **Evaluation**: Accuracy, confusion matrix, precision-recall  

### 🔸 Part 2: Streamlit Web App
- Built a clean UI using Streamlit  
- Allows file upload (CSV EEG data)  
- Performs prediction using trained ML/DL models  
- Displays prediction and insights interactively  

---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/epileptic-seizure-predictor.git
cd epileptic-seizure-predictor
```

### 2. Create virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

---

## ▶️ Run

### For Linux and macOS users:
```bash
streamlit run app.py
```

### For Windows users:
```cmd
streamlit run app.py
```

---

## 🌍 Deployment (Heroku)

### ✅ Prerequisite: Working Streamlit Web App

### Step 1: Prepare for deployment
- Create a `requirements.txt` file:
  ```bash
  pip freeze > requirements.txt
  ```
- Create a `Procfile` with:
  ```
  web: streamlit run app.py
  ```
- Optional: Add `setup.sh`, `runtime.txt` for specific Python version

### Step 2: Deploy to Heroku
1. Login to Heroku:
   ```bash
   heroku login
   ```
2. Create a new Heroku app:
   ```bash
   heroku create seizure-predictor
   ```
3. Push code to Heroku:
   ```bash
   git add .
   git commit -m "Deploy Streamlit app"
   git push heroku main
   ```
4. Open your app:
   ```bash
   heroku open
   ```

---

## 📂 Directory Tree

```
epileptic-seizure-predictor/
├── app.py
├── model/
│   ├── seizure_cnn_model.h5
│   └── seizure_rf_model.pkl
├── utils/
│   └── preprocess.py
├── data/
│   └── sample_eeg.csv
├── requirements.txt
├── Procfile
├── README.md
└── assets/
    └── demo.gif
```

---

## 📈 To Do
- Improve accuracy with hybrid CNN-LSTM model  
- Integrate real-time EEG data processing  
- Add feature to visualize EEG signals before prediction  
- Deploy on multiple cloud platforms  
- Add feedback loop for continuous learning  

---

## 🐛 Bug / Feature Request

If you find a bug (e.g., crash or invalid result), kindly open an [issue here](https://github.com/yourusername/epileptic-seizure-predictor/issues) with:
- Your input EEG file  
- Expected output  
- Actual behavior  

If you’d like to request a new feature, feel free to do so by opening an issue and describing:
- What it should do  
- How it helps  
- Sample input/output if possible  

---

## 🧰 Technologies Used

| Tech Stack | Description |
|------------|-------------|
| ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) | Core programming language |
| ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white) | Web app framework |
| ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn&logoColor=white) | ML models |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white) | Deep learning framework |
| ![Heroku](https://img.shields.io/badge/Heroku-430098?logo=heroku&logoColor=white) | Deployment platform |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white) | Data manipulation |
| ![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white) | Scientific computation |

---

## 📜 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🙌 Credits

Thanks to:
- UCI for the EEG Seizure dataset  
- Open-source contributors of Streamlit, TensorFlow, and scikit-learn  
# Epileptic-Seizure-Detection-in-EEG-Signals-Using-Machine-Learning-and-Deep-Learning-Techniques
