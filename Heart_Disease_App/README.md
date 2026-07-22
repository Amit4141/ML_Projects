# Heart Disease Prediction App ❤️

A machine learning web app built with **Streamlit** that predicts the risk of heart disease based on patient health data.

## Project Structure

```
Heart_Disease_App/
├── app.py                  # Streamlit web application
├── heart.csv               # Dataset used for training
├── heart.ipynb             # Jupyter notebook (EDA + model training)
├── LG_heart_model.pkl      # Trained Logistic Regression model
├── LR_scaler.pkl           # Fitted StandardScaler
├── LG_columns.pkl          # Expected input columns after one-hot encoding
└── README.md               # Project documentation
```

## Features

- Takes user inputs like Age, Sex, Chest Pain Type, Cholesterol, etc.
- Preprocesses inputs using the saved scaler and column structure
- Predicts whether the patient is at **High Risk** or **Low Risk** of heart disease

## Tech Stack

- **Python**
- **Scikit-learn** – Logistic Regression model
- **Streamlit** – Web UI
- **Pandas** – Data handling
- **Joblib** – Model serialization

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/ML_Projects.git
   cd ML_Projects/Heart_Disease_App
   ```

2. Install dependencies:
   ```bash
   pip install streamlit pandas scikit-learn joblib
   ```

3. Run the app:
   ```bash
   streamlit run app.py
   ```

## Input Features

| Feature | Description |
|---|---|
| Age | Patient's age |
| Sex | M / F |
| ChestPainType | ATA / NAP / TA / ASY |
| RestingBP | Resting blood pressure (mm Hg) |
| Cholesterol | Serum cholesterol (mg/dL) |
| FastingBS | Fasting blood sugar > 120 mg/dL (1 = Yes) |
| RestingECG | Normal / ST / LVH |
| MaxHR | Maximum heart rate achieved |
| ExerciseAngina | Exercise-induced angina (Y / N) |
| Oldpeak | ST depression induced by exercise |
| ST_Slope | Slope of peak exercise ST segment (Up / Flat / Down) |

## Model

Logistic Regression trained on the [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction).

---
Made by **Amit**
