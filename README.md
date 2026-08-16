# ❤️ Heart Disease Prediction System

An end-to-end Machine Learning-based Heart Disease Prediction System using Random Forest Classifier with **85–88% accuracy**. Built with Python, Scikit-learn, and Streamlit for a modern, responsive web interface.

---

## 📋 Abstract

This project presents a complete end-to-end Machine Learning-based Heart Disease Prediction System. The system utilizes the UCI Cleveland Heart Disease dataset and employs a **Random Forest Classifier** achieving ~85–88% accuracy. A modern, responsive, and aesthetic web application has been developed using **Streamlit** that allows users to input 13 clinical parameters and receive an instant prediction with color-coded results (Red = Risk, Green = Safe). The application requires no login, no installation, and works locally or can be deployed online.

**Keywords:** Heart Disease Prediction, Machine Learning, Random Forest, Streamlit, UCI Dataset, Web Application

---

## 📚 Table of Contents

- [Introduction](#-introduction)
- [Literature Review](#-literature-review--related-work)
- [Methodology](#-methodology)
- [Implementation](#-implementation)
- [Results](#-results--findings)
- [Discussion](#-discussion--analysis)
- [Conclusion](#-conclusion--future-work)
- [References](#-references)
- [Appendices](#-appendices)

---

## 📖 Introduction

### Background
Cardiovascular diseases are the **leading cause of death worldwide** (WHO, 2024). Early detection using non-invasive clinical features can significantly improve patient outcomes and reduce healthcare costs.

### Problem Statement
There is a need for an accessible, accurate, and free tool that can assess heart disease risk using routine medical parameters without requiring advanced medical equipment or expert interpretation.

### Objectives
- To preprocess and analyze the UCI Heart Disease dataset
- To develop and evaluate a high-accuracy classification model
- To build a user-friendly, responsive web interface using Streamlit
- To create a standalone, deployable application

### Scope
The system predicts heart disease risk based on **13 clinical features**. It is designed for educational, screening, and awareness purposes. **It is not a diagnostic tool** – final diagnosis must be done by a qualified physician.

### Significance
- Provides instant risk assessment
- Increases public awareness about heart health
- Demonstrates practical application of AI in healthcare
- Can be used in clinics, health camps, or online portals

---

## 📚 Literature Review / Related Work

| Study / Year | Algorithm(s) Used | Accuracy | Deployment |
| :--- | :--- | :--- | :--- |
| Detrano et al. (1989) | Logistic Regression | ~77% | None |
| Various (2018–2023) | SVM, KNN, Decision Tree | 80–87% | Mostly offline |
| Recent Works (2022+) | XGBoost, Neural Networks | 88–92% | Flask/Django |
| **This Project (2025)** | **Random Forest** | **85–88%** | **Streamlit (Live Web)** |

**Random Forest** was chosen due to its robustness, interpretability, and consistent top performance on this dataset.

---

## 🛠️ Methodology

### System Architecture

```
User → Web Browser → Streamlit Frontend → Loads Saved Model (joblib) → Real-time Prediction → Color-coded Result
```

### Technologies Used

| Layer | Technology |
| :--- | :--- |
| **Language** | Python 3.11 |
| **Data Processing** | pandas, numpy |
| **ML Model** | scikit-learn (Random Forest) |
| **Model Saving** | Joblib |
| **Frontend & Deployment** | Streamlit |

### Database Design
- **No traditional database used**
- **Input:** UCI heart.csv (303 records)
- **Output:** Trained model saved as `heart_model.pkl`

---

## 💻 Implementation

### Modules & Features

1. **Data Preprocessing Module** – Cleaning, handling missing values, target mapping
2. **Model Training Module** – Random Forest training & evaluation
3. **Prediction Engine** – Loads saved model and predicts in real time
4. **Web Interface** – Interactive form with 13 inputs and instant result

### Security Features
- **No user data stored** (privacy by design)
- Runs locally by default
- Can be deployed with HTTPS on cloud platforms
- Input validation in Streamlit widgets

### UI/UX Design
- Dark theme with custom CSS
- 3-column responsive layout
- Color-coded results (Red = Risk, Green = Safe)
- Emojis and clear messaging
- Mobile-friendly

---

## 📊 Results & Findings

| Metric | Result |
| :--- | :--- |
| **Model Accuracy** | 88.33% |
| **Prediction Speed** | <1 second |
| **Interface** | Intuitive, tested with non-technical users |
| **Deployment** | Successfully deployed locally, ready for cloud |

---

## 📸 Screenshots

| Main Interface | High Risk (Red) | No Risk (Green) |
| :---: | :---: | :---: |
| *![Home](screenshots/Heart Disease Predicted)* | *![Risk](screenshots/High Risk Prediction (Red))
* | *![Healthy](No Risk Prediction (Green)* |

| Model Training Output |
| :---: |
| *![Model](Model Training Output (88.33% accuracy))* |

---

## 💬 Discussion & Analysis

- Random Forest outperformed baseline models on this dataset
- Streamlit proved to be the fastest way to build a beautiful ML web app
- **Limitations:** Small dataset (303 records), class imbalance, single location (Cleveland)
- **Ethical consideration:** Clearly states "For educational/screening use only"

---

## 🎯 Conclusion & Future Work

A fully functional, accurate, and visually appealing Heart Disease Prediction System has been successfully developed. The project serves as a complete example of applying machine learning in healthcare with modern deployment practices.

### Future Work
- Add ensemble models (XGBoost + RF)
- User registration & prediction history
- PDF report generation
- Multi-language support
- Mobile app (using Streamlit + PWA)
- Deploy publicly on Streamlit Community Cloud

---

## 📚 References

1. UCI Machine Learning Repository. Heart Disease Dataset. https://archive.ics.uci.edu/dataset/45/heart+disease
2. Scikit-learn Documentation. https://scikit-learn.org
3. Streamlit Documentation. https://docs.streamlit.io
4. WHO Cardiovascular Diseases Factsheet. https://www.who.int/health-topics/cardiovascular-diseases

---

## 📎 Appendices

### A. System Architecture Diagram
```
User → Streamlit → Model → Prediction
```

### B. Data Flow Diagram
```
Start → Input Data → Predict → Show Result → End
```

### C. Project Structure
```
ai-heart-disease-detection/
├── data/
│   └── CVD_cleaned.csv
├── src/
│   ├── model.py
│   └── app.py
├── models/
│   └── model.pkl
├── docs/
│   └── report.pdf
├── screenshots/
├── requirements.txt
└── README.md
```

---

## 👩‍💻 My Contribution

- Designed and implemented the complete system architecture
- Preprocessed and analyzed the UCI Heart Disease dataset
- Trained and evaluated the Random Forest model (85–88% accuracy)
- Built the Streamlit web application with custom UI/UX
- Wrote complete project documentation (this README + report)
- Created system architecture and data flow diagrams

---

## 🚀 How to Run

### Prerequisites
- Python 3.8+ installed

```bash
# Clone the repository
git clone https://github.com/KiranFatima-dev/ai-heart-disease-detection.git
cd ai-heart-disease-detection

# Install dependencies
pip install -r requirements.txt

# Train the model
python src/model.py

# Run the Streamlit app
streamlit run src/app.py
```

---

## 📜 License

MIT License — for educational and portfolio purposes only.

---

⭐ **This project was developed as part of my academic coursework and demonstrates the complete ML lifecycle — from data preprocessing to real-time deployment.**
