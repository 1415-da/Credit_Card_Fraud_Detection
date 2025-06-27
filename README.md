# Credit Card Fraud Detection Web App

A modern, responsive web application for real-time credit card fraud detection. Built with React.js (frontend), Flask (backend), and a machine learning model trained on public datasets. The app provides actionable insights, interactive analytics, and a seamless user experience inspired by leading fintech design trends.

---

## 🚀 Features

- **Landing Page:** Minimalist hero section, app branding, and a clear call-to-action.
- **Transaction Input Form:** Clean, card-based UI for entering transaction details (V1–V28, Time, Amount) with real-time validation.
- **Prediction Results:**  
  - Fraud probability (percentage) and color-coded risk level  
  - Contextual table of similar past transactions  
  - Actionable recommendations  
  - Export/share results (PDF/CSV)
- **Analytics Dashboard (Optional):**  
  - Visualizations of fraud trends and recent predictions  
  - Table of recent transactions analyzed
- **User Experience:**  
  - Smooth transitions, loading indicators, tooltips  
  - Responsive design for desktop and mobile  
  - Modern color scheme and typography

---

## 🛠️ Tech Stack

- **Frontend:** React.js, Tailwind CSS or Material UI
- **Backend:** Flask (Python), Flask-CORS
- **ML Model:** scikit-learn (or similar), trained on public credit card fraud dataset
- **Deployment:** Vercel (frontend & backend as serverless functions)
- **Other:** Jupyter Notebook for model development, joblib for model serialization

---

## 📦 Project Structure

```
Credit_Card_Fraud_Detection/
│
├── backend/                # Flask API (serves ML model)
│   ├── app.py
│   ├── model.joblib
│   └── requirements.txt
│
├── frontend/               # React app
│   ├── src/
│   ├── public/
│   └── package.json
│
├── model_dev/              # Jupyter notebooks for EDA & model training
│   └── fraud_detection.ipynb
│
├── vercel.json             # Vercel configuration
└── README.md
```

---

## ⚡ Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Credit_Card_Fraud_Detection.git
cd Credit_Card_Fraud_Detection
```

### 2. Model Development (Jupyter Notebook)

- Navigate to `model_dev/`
- Open `fraud_detection.ipynb` in Jupyter Notebook
- Analyze data, train your model, and export it as `model.joblib` to `backend/`

### 3. Backend Setup (Flask API)

```bash
cd backend
pip install -r requirements.txt
python app.py
```

- The Flask API will load the trained model and serve prediction endpoints.

### 4. Frontend Setup (React)

```bash
cd ../frontend
npm install
npm start
```

- The React app will run locally and communicate with the Flask backend.

### 5. Deployment (Vercel)

- Ensure both `frontend/` and `backend/` are configured as Vercel projects.
- Use `vercel` CLI or connect your repo to Vercel dashboard.
- Configure `vercel.json` to route API requests to the backend.

---

## 🧩 API Endpoints

- `POST /api/predict`  
  - **Input:** JSON with transaction features  
  - **Output:** Fraud probability, risk level, recommendations

---

## 📝 License

MIT License

---

**Feel free to contribute or open issues for suggestions and improvements!**