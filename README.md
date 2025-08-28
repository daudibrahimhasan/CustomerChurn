# ✈️ Flight Price Prediction using K-Nearest Neighbours (KNN)

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data--Analysis-green?logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📌 Project Overview
This project applies **K-Nearest Neighbours (KNN)** machine learning algorithm using **Scikit-Learn** to predict **flight ticket prices in Bangladesh**.  

The dataset contains **57,000+ flight records**, including airline details, routes, timings, duration, and fares.  
The goal is to **predict ticket fares (Total Fare in BDT)** based on selected features like source, destination, and duration.  

---

## ⚙️ Workflow

### 1. Dataset Loading
- Dataset stored in **Google Drive** and imported with **Pandas**.  
- Contains columns such as airline, route, stopovers, base fare, tax, and total fare.  

### 2. Feature Selection & Encoding
- Features used:  
  - `Source`  
  - `Destination`  
  - `Duration (hrs)`  
  - `Total Fare (BDT)`  
- Applied **Label Encoding** on categorical features (`Source`, `Destination`).  

### 3. Data Standardization
- Standardized features using **StandardScaler** for zero mean & unit variance.  
- Important since **KNN is distance-based**.  

### 4. Train-Test Split
- Data split: **80% training** and **20% testing**.  

### 5. Model Training (KNN Regression)
- Trained models with different values of `k` (1–9).  
- Evaluated using **R² Score** and error deviation.  
- Best result: **k = 1 with R² ≈ 0.9991** 🎯  

### 6. Visualization
- Plotted **R² Score vs. Number of Neighbors (k)**.  
- Clear indication of strong predictive performance.  

---

## 📊 Results
- **Best Accuracy (R² Score):** 0.9991 with `k = 1`  
- Model achieved **extremely high accuracy** in predicting flight fares.  

---

## 🛠️ Technologies Used
- [Python](https://www.python.org/)  
- [Pandas](https://pandas.pydata.org/)  
- [NumPy](https://numpy.org/)  
- [Matplotlib](https://matplotlib.org/)  
- [Scikit-Learn](https://scikit-learn.org/stable/)  
- [Google Colab](https://colab.research.google.com/)  

---

## 🌍 Real-World Applications
- **Travel Industry:** Fare prediction and trend analysis.  
- **Airlines:** Revenue management & price optimization.  
- **Online Travel Agencies (OTAs):** Cheapest flight recommendation engines.  
- **Travelers:** Identify the best time and price to book tickets.  

---

## 🚀 Future Improvements
- Add more features: **airline, stopovers, seasonality**.  
- Compare with other ML models (**Random Forest, XGBoost, Neural Networks**).  
- Deploy as a **web app** with Flask/Django + Streamlit/Gradio.  
- Integrate **real-time flight data** using APIs.  

---

## 📂 Dataset
- `Flight_Price_Dataset_of_Bangladesh.csv`  
- 57,000 rows × 17 columns  
- Contains flight details including airline, source, destination, timings, duration, fare components, and total fare.  

---

## 🧑‍💻 Author
**Daud Ibrahim Hassan**  
📌 Data Analyst & CSE Student at BRAC University  
🔗 [LinkedIn](https://www.linkedin.com/daudibrahimhasan) | [GitHub](https://github.com/daudibrahimhasan)  

---
