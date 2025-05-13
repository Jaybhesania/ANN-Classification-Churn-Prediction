# ANN Classification: Customer Churn Prediction with Streamlit

A simple yet powerful **Artificial Neural Network (ANN)** based solution for predicting customer churn using structured banking data. This project includes full preprocessing, model training, evaluation, and a sleek **Streamlit web app** for real-time predictions!

---

## About the Project

This project focuses on predicting whether a customer will leave a bank (churn) using an ANN model built with TensorFlow. It includes:

* Data preprocessing (encoding, scaling)
* ANN model building & training
* Real-time predictions with a Streamlit UI
* TensorBoard integration for training visualization

---

## Live Streamlit App

**Title:** `Customer Churn Predictor: Powered by ANN`

> Predict customer churn probability using a clean, interactive UI. Input customer details, and get real-time churn predictions instantly!

---

## Project Structure

```
.
├── Churn_Modelling.csv              
├── app.py                           # Streamlit Web App
├── experiments.ipynb                # Preprocessing + Model Training
├── prediction.ipynb                 # Manual Prediction Script
├── label_encoder_gender.pkl         
├── onehot_encoder_geo.pkl           
├── scaler.pkl                       
├── model.h5                         # Trained ANN Model
├── requirements.txt                
└── README.md                        
```

---

## Model Architecture

* **Input Layer** → 11 features (after encoding)
* **Hidden Layers**:

  * Dense(64) + ReLU
  * Dense(32) + ReLU
* **Output Layer**:

  * Dense(1) + Sigmoid (for binary classification)

---

## Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/yourusername/ANN-Classification-Churn-Prediction.git
   cd ANN-Classification-Churn-Prediction
   ```

2. **Install dependencies**
   *(Recommended: Use a virtual environment)*

   ```bash
   pip install -r requirements.txt
   ```

3. **Run Streamlit App**

   ```bash
   streamlit run app.py
   ```

---

## Sample Prediction Logic

Pass customer details → Encode → Scale → Predict with `.h5` model → Output churn probability

---

## Key Highlights

*  Fully working ANN churn predictor
*  Custom preprocessing with encoders & scalers saved
*  Real-time predictions via Streamlit
*  Clean and extensible codebase for future ML ideas

---
