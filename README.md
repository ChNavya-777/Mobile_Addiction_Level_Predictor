# 📱 Mobile Addiction Level Predictor

## 🚀 Project Overview

This project predicts the **mobile addiction level** of a user based on behavioral, lifestyle, and psychological factors using **Machine Learning (Regression)**.

The model outputs a **continuous addiction score**, which is then categorized into:

* 🟢 Low
* 🟡 Moderate
* 🔴 High

This helps users understand their usage patterns and take **preventive actions**.

---

## 🎯 Objective

* Analyze mobile usage behavior
* Predict addiction severity using ML
* Provide **interpretable results** for awareness
* Encourage healthy digital habits

---

## 📊 Dataset Description

The dataset contains teen mobile usage data including:

* Usage patterns (screen time, app usage)
* Lifestyle factors (sleep, exercise)
* Psychological indicators (self-esteem, anxiety)

### Target Variable:

`Addiction_Level` (Continuous value: ~1–10)

---

## 🧾 Features Used

### 📱 Usage Behavior

* Daily Usage Hours
* Screen Time Before Bed
* Phone Checks Per Day
* Apps Used Daily
* Time on Social Media
* Time on Gaming
* Weekend Usage Hours

### 🧠 Lifestyle & Psychological

* Sleep Hours
* Academic Performance
* Exercise Hours
* Social Interactions
* Family Communication
* Anxiety Level
* Depression Level
* Self Esteem

### 👤 Demographic (optional)

* Age
* Gender
* School Grade

---

## ⚙️ Machine Learning Approach

### 🔹 Problem Type

**Regression with post-processing classification**

### 🔹 Models Used

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor ✅ (Best)

### 🔹 Evaluation Metrics

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* R² Score

---

## 🔄 ML Pipeline

1. Data Cleaning
2. Missing Value Handling
3. Label Encoding
4. Outlier Removal (IQR Method)
5. Feature Selection (SelectKBest)
6. Feature Scaling (StandardScaler)
7. Train-Test Split (80-20)
8. Model Training
9. Model Evaluation
10. Model Saving using Pickle

---

## 🧠 Prediction Logic

After predicting addiction score:

| Score Range | Level    |
| ----------- | -------- |
| < 4         | Low      |
| 4 – 6.9     | Moderate |
| ≥ 7         | High     |

---

## 💻 Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* Pickle
* Gradio

---

## 🖥️ User Interface

Built using **Gradio**, allowing users to:

* Enter input values
* Get real-time predictions
* View addiction level with suggestions

---

## 📦 How to Run the Project

### 1. Clone Repository

```bash
git clone <your-repo-link>
cd project-folder
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Application

```bash
python app.py
```

---

## 📈 Example Output

```
Score: 7.25  
Level: High 🔴  
Suggestion: Reduce screen time and avoid usage before sleep
```

---

## ⚠️ Limitations

* Based on self-reported data
* Not a clinical diagnosis
* Thresholds are generalized

---

## 📌 Future Improvements

* Personalized recommendations
* Deep learning models
* Mobile app integration
* Real-time usage tracking

---

## 👥 Team Members

* Your Name
* Team Member 2
* Team Member 3

---

## 📜 License

This project is for academic and research purposes only.

---

## ⭐ Final Note

This project demonstrates how machine learning can be applied to **analyze digital behavior** and promote **healthier technology usage**.
