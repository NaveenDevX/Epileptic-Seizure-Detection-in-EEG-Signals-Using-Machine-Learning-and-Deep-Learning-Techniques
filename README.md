# Epileptic Seizure Detection in EEG Signals Using Machine Learning and Deep Learning Techniques

## Table of Contents
- [Demo](#demo)
- [Overview](#overview)
- [Motivation](#motivation)
- [Technical Aspect](#technical-aspect)
- [Installation](#installation)
- [Run](#run)
- [Deployment (Heroku)](#deployment-heroku)
- [Directory Tree](#directory-tree)
- [To Do](#to-do)
- [Bug / Feature Request](#bug--feature-request)
- [Technologies Used](#technologies-used)
- [License](#license)
- [Credits](#credits)

---

## Demo

**Web App**: [Link to Live Application](https://your-app-link.streamlit.app)  
*(Replace with your deployed Streamlit Heroku URL)*

---

## Overview

This project focuses on the automated detection of epileptic seizures using EEG (Electroencephalogram) signals.  
We have implemented both machine learning and deep learning approaches to classify seizure vs. non-seizure patterns.  
A user-friendly Streamlit web interface makes it accessible for real-time testing and deployment.

---

## Motivation

The unpredictability and severity of epileptic seizures demand fast, reliable, and scalable detection systems.  
Manual interpretation of EEG signals is time-consuming and requires domain expertise.  
This project was inspired by the need for accessible, intelligent diagnostic tools for early seizure prediction.  
By combining classical ML with advanced deep learning, we aim to provide an automated, accurate solution.  
Making this system available as a web app further reduces barriers to access in clinical or research settings.

---

## Technical Aspect

### Part 1: Machine Learning & Deep Learning Approaches

- **Dataset**: UCI Epileptic Seizure Recognition Dataset  
- **Preprocessing**:
  - Signal normalization
  - Reshaping to fit model input
  - Class balancing and label encoding
- **Machine Learning Models**:
  - Random Forest
  - Decision Tree
  - XGBoost
- **Deep Learning Models**:
  - 1D Convolutional Neural Network (CNN)
  - Fully Connected Network (DNN)
- **Evaluation Metrics**:
  - Accuracy, F1 Score, Precision, Recall, ROC-AUC, Confusion Matrix

### Part 2: Streamlit Web App

- **File Upload**: Accepts raw EEG CSV files
- **Model Prediction**: Loads pretrained ML/DL models
- **Visual Feedback**: Displays result with charts and probabilities
- **Responsive UI**: Built using Streamlit components

---

## Installation

### Step 1: Clone Repository
```bash
git clone https://github.com/yourusername/epileptic-seizure-predictor.git
cd epileptic-seizure-predictor
```

### Step 2: Setup Virtual Environment (Recommended)
```bash
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
```

### Step 3: Install Required Packages
```bash
pip install -r requirements.txt
```

---

## Run

### Linux/macOS:
```bash
streamlit run app.py
```

### Windows:
```cmd
streamlit run app.py
```

---

## Deployment (Heroku)

### Step 1: Create and Test Streamlit App Locally
Ensure your app (`app.py`) runs successfully using:
```bash
streamlit run app.py
```

### Step 2: Prepare Heroku Files
- `requirements.txt`: Contains Python packages
- `Procfile`: Tells Heroku how to run the app
  ```
  web: streamlit run app.py
  ```
- (Optional) `setup.sh`, `runtime.txt`

### Step 3: Deploy to Heroku
```bash
heroku login
heroku create seizure-predictor
git add .
git commit -m "Initial deployment"
git push heroku main
heroku open
```

---

## Directory Tree

```
epileptic-seizure-predictor/
├── app.py
├── model/
│   ├── seizure_cnn_model.h5
│   └── seizure_rf_model.pkl
├── utils/
│   ├── preprocess.py
│   └── visualization.py
├── data/
│   └── sample_eeg.csv
├── requirements.txt
├── Procfile
├── runtime.txt
├── README.md
├── assets/
│   ├── architecture_diagram.png
│   └── performance_charts/
└── LICENSE
```

---

## To Do

- Integrate real-time EEG stream input  
- Extend to multiclass seizure classification  
- Add model explainability using SHAP/LIME  
- Improve deep learning architecture using RNN/CNN hybrid models  
- Support mobile and offline web deployment

---

## Bug / Feature Request

Found a bug or want to suggest a feature? Please open an issue with the following:

- Steps to reproduce
- Expected vs actual behavior
- Suggestions or feature request format

[Open an issue](https://github.com/yourusername/epileptic-seizure-predictor/issues)

---

## Technologies Used

| Technology      | Purpose                             |
|----------------|-------------------------------------|
| Python          | Core language                       |
| NumPy           | Numerical operations                |
| Pandas          | Data handling and transformation    |
| Matplotlib      | Data visualization                  |
| Seaborn         | Statistical plots                   |
| Scikit-learn    | Machine learning models             |
| TensorFlow/Keras| Deep learning model implementation  |
| XGBoost         | Gradient boosting ML model          |
| Streamlit       | Web app development                 |
| Heroku          | App deployment                      |
| Pickle          | Model serialization                 |

---

## License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for more details.

---

## Credits

- UCI Machine Learning Repository for the EEG dataset  
- Open-source packages and frameworks  
- Research papers on epileptic seizure classification  

