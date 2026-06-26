# 🧠 Mental Health Predictor App

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://mentalhealthpredictor07.streamlit.app/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=flat&logo=github)](https://github.com/Hardikabrol8)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/hardik-abrol-639068288/)

An interactive Streamlit-powered dashboard and machine learning application designed to explore mental health trends in the tech industry and predict whether an individual might benefit from professional mental health support.

---

### 🌐 Live Application
You can access and interact with the live deployed application here:  
👉 **[https://mentalhealthpredictor07.streamlit.app/](https://mentalhealthpredictor07.streamlit.app/)**

---

## 🎯 Key Features

- **📊 Interactive EDA Dashboard**: Dive deep into demographic distributions, behavioral attributes, and statistical analyses of survey respondents from around the world.
- **🧠 Treatment Predictor Quiz**: Answer a curated, multiple-choice quiz backed by a machine learning model to estimate the probability of needing mental health support.
- **🔍 Model Interpretability & Analysis**: Explore feature importances, evaluation metrics, and the rationale behind choosing the CatBoost model.
- **🌓 Adaptive Theme**: Sleek, modern dark-mode design optimized for a comfortable visual experience.

---

## 📂 Repository Structure

```directory
├── Homepage.py                 # Main entrypoint of the Streamlit application
├── utils.py                    # Shared utility functions (model caching, preprocessing, insights)
├── requirements.txt            # Python dependencies list
├── LICENSE                     # MIT License details
├── .streamlit/
│   └── config.toml             # Streamlit theme and UI configurations (Dark Mode)
├── pages/
│   ├── Dashboard.py            # Exploratory Data Analysis page
│   ├── Mental_Health_Prediction_App.py  # MCQ-style Treatment Predictor Quiz
│   └── Model_Analysis.py       # Model features and evaluation breakdown
├── Data/
│   ├── Mental Health Dataset.csv # Raw survey data
│   ├── cleaned_dataset.csv      # Preprocessed data for modeling/EDA
│   └── chi2_cramersv_summary.csv# Precomputed statistical correlation matrix
├── models/
│   └── Mental_Health_Prediction_model2.cbm # Saved CatBoost Classifier model
└── JupyterNotebook/
    └── Mental_Health_Dataset.ipynb # Jupyter notebook containing model training and EDA workflow
```

---

## ⚙️ Local Setup Instructions

Follow these steps to run the application locally on your machine:

### Prerequisites
- Python 3.9 or higher installed

### Step-by-Step Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Hardikabrol8/Mental_Health_Predictor.git
   cd Mental_Health_Predictor
   ```

2. **Set up a Virtual Environment:**
   *On Windows:*
   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```
   *On macOS/Linux:*
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the Application:**
   ```bash
   streamlit run Homepage.py
   ```

The application will launch automatically in your default browser at `http://localhost:8501`.

---

## 📊 Model Information & Architecture

- **Algorithm**: CatBoost Classifier
- **Rationale**: Highly robust with categorical features, handles missing values naturally, and is resistant to overfitting without intensive scaling preprocessing.
- **Top Features**: Continent, Care Options, Self-Employed status, Family History of mental illness, and Comfort in interview settings.
- **Performance**: High recall score (~0.83) optimized specifically to minimize false negatives (failing to recognize individuals who need support).

---

> [!WARNING]
> ### ⚠️ Clinical Disclaimer
> This application is **not** a substitute for professional diagnosis, therapy, or medical advice. The predictions and analyses generated are based on general survey patterns and are for informational/educational purposes only. If you or someone you know is experiencing mental distress, please reach out to qualified healthcare providers or local support hotlines.

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 🪪 License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for more information.

---

## 🌐 Connect & Feedback

Feel free to connect or share your thoughts on the project!

- **GitHub**: [@Hardikabrol8](https://github.com/Hardikabrol8)
- **LinkedIn**: [Hardik Abrol](https://www.linkedin.com/in/hardik-abrol-639068288/)
