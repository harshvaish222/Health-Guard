# 🩺 Health-Guard

**Health-Guard** is a smart health prediction web application powered by **Streamlit** and **Machine Learning**.  
It predicts the likelihood of **Diabetes** and **Heart Disease** using user-input health data, helping raise awareness about potential health risks.

> ⚠️ This tool is for **educational purposes only** — not a replacement for professional medical advice.

---

## 🌟 Features

✅ **Diabetes Prediction** – based on glucose, BMI, insulin, etc.  
✅ **Heart Disease Prediction** – based on cholesterol, blood pressure, age, etc.  
✅ **Streamlit-based UI** – clean, responsive, and interactive  
✅ **Real-time Predictions** – get instant results  
✅ **Pre-trained Models** – efficient `.sav` model loading for fast performance  

---

## 🧠 Tech Stack

| Category | Technologies Used |
|-----------|------------------|
| Frontend | Streamlit |
| Backend | Python |
| ML Algorithms | Logistic Regression, Random Forest (via scikit-learn) |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |

---

## 📁 Project Structure

Health-Guard/
│
├── app3.py # Streamlit web application
├── diabetes_model.sav # Trained Diabetes model
├── heart_disease_model.sav # Trained Heart Disease model
├── Diabetes Prediction.ipynb # Model training notebook (Diabetes)
├── Heart Disease Prediction.ipynb # Model training notebook (Heart Disease)
├── diabetes.csv # Dataset for Diabetes model
├── heart.csv # Dataset for Heart Disease model
├── requirements.txt # Project dependencies
└── README.md # Documentation file


---

## ⚙️ Installation & Running Locally

### 1️⃣ Clone the repository

git clone https://github.com/harshvaish222/Health-Guard.git
cd Health-Guard

### 2️⃣ Install dependencies
pip install -r requirements.txt

### 3️⃣ Run the Streamlit app
streamlit run app3.py


### 4️⃣ Open in browser

Visit: 👉 http://localhost:8501


Prediction Logic runs the data through the trained model

Results are displayed instantly with color-coded feedback


