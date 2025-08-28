# ✈️ Flight Price Prediction using K-Nearest Neighbours (KNN)

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data--Analysis-green?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-informational?logo=python)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📌 Project Overview
This project builds a **machine learning model** using the **K-Nearest Neighbours (KNN)** algorithm to predict **flight ticket prices in Bangladesh**.  

The dataset includes **57,000+ flight records** with information such as airline, route, timings, duration, stopovers, and fare details.  

The primary objective is to **predict the total fare (in BDT)** by learning patterns from features like **source, destination, and flight duration**.  
This approach demonstrates the use of **distance-based regression** for solving real-world airline pricing problems.

---

## ⚙️ Workflow

### 1. Data Loading & Exploration
- Dataset loaded from **Google Drive** into a Pandas DataFrame.  
- Shape: `57,000 rows × 17 columns`.  

### 2. Feature Engineering
- Selected features:  
  - `Source`  
  - `Destination`  
  - `Duration (hrs)`  
  - `Total Fare (BDT)`  
- Applied **Label Encoding** on categorical features (`Source`, `Destination`).  

### 3. Preprocessing
- Normalized features using **StandardScaler** to ensure KNN handles distance calculations effectively.  

### 4. Train-Test Split
- Data split into **80% training** and **20% testing** using `train_test_split`.  

### 5. Model Training
- Implemented **KNN Regression** (`KNeighborsRegressor`).  
- Trained across multiple values of `k` (1–9).  
- Evaluated using **R² Score** and standard error.  

### 6. Evaluation & Visualization
- Best performance at **k = 1** with **R² ≈ 0.9991**.  
- Plotted **R² Score vs. k** to visualize model performance.  

---

## 📊 Results
✅ **Best Accuracy (R² Score):** 0.9991 with `k = 1`  
✅ High predictive power achieved with only a few features.  
✅ Strong indication that **route and duration have significant influence** on ticket pricing.  

---

## 🛠️ Tools & Technologies
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Scikit-Learn  
- **Environment:** Google Colab (with Drive integration)  

---

## 🌍 Real-World Applications
- **Airlines** → Revenue management & demand-based dynamic pricing.  
- **Online Travel Agencies (OTAs)** → Price prediction and recommendation systems.  
- **Travelers** → Identify the best time and route for affordable tickets.  
- **Market Analysts** → Seasonal and route-based price forecasting.  

---

## ⚖️ Limitations & Future Work
Although the model achieves near-perfect accuracy, it is important to acknowledge:  
- **Feature limitations:** Only a subset of features (source, destination, duration) was used.  
- **Overfitting risk:** KNN with `k=1` may memorize rather than generalize.  
- **Data bias:** Dataset is region-specific (Bangladesh).  

🔮 **Planned Improvements**:
- Incorporate richer features (airline, stopovers, booking source, seasonality).  
- Compare performance with advanced models (Random Forest, XGBoost, Neural Networks).  
- Perform **hyperparameter tuning** with `GridSearchCV`.  
- Deploy as an interactive **web application** (Streamlit/Django).  
- Explore integration with **real-time flight APIs**.  

---

## 📂 Dataset
- **File:** `Flight_Price_Dataset_of_Bangladesh.csv`  
- **Size:** 57,000 rows × 17 columns  
- **Columns:** Airline, Source, Destination, Duration, Aircraft Type, Class, Booking Source, Base Fare, Tax, Total Fare, Seasonality, Days Before Departure, etc.  

---

## 🧑‍💻 Author
**Daud Ibrahim Hassan**  
📌 Data Analyst & Computer Science Student (BRAC University)  
🔗 [LinkedIn](https://www.linkedin.com) | [GitHub](https://github.com)  

---
