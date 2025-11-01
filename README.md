# 🩺 ClinIQ – Doctor Appointment Scheduling App

ClinIQ is a minimal full-stack SaaS application designed to help individual doctors manage their one-person clinics efficiently.  
It allows doctors to set their availability, patients to book appointments online, and doctors to track completed and missed visits.

---

## 🚀 Features

- Doctor can set available time slots  
- Patients can book appointments based on doctor’s availability  
- Doctor can view and manage all appointments  
- Mark appointments as **Completed** or **No-show**  
- FastAPI backend with **automated testing and HTML reports**  
- Clean, modular structure for scalability  

---

## 🧩 Tech Stack

### **Backend**
- FastAPI  
- SQLModel / SQLite  
- Pytest + pytest-html  

### **Frontend**
- React  
- Axios  
- Tailwind CSS  

---

## 🗂 Folder Structure

```
ClinIQ/
├── backend/
│   ├── main.py              # FastAPI backend entry point
│   ├── test.py              # Pytest test cases
│   ├── reports/             # Folder where pytest HTML report is generated
│   │   └── report.html
│   ├── requirements.txt     # Python dependencies
│   └── __init__.py (optional)
│
├── frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/           # React pages
│   │   └── App.jsx / App.js
│   ├── public/
│   │   └── index.html
│   ├── package.json         # Frontend dependencies
│   ├── vite.config.js / webpack.config.js
│   └── README.md (optional)
│
├── README.md                # Main project documentation (this file)
└── THINKING-ALOUD.md        # Design decisions and trade-offs
```

---

## ⚙️ Setup Instructions

### 🖥️ 1️⃣ Clone the Repository

```bash
git clone https://github.com/rakshicharvik/ClinIQ-App.git
cd ClinIQ-App
```

---

### ⚡ 2️⃣ Run the Backend

```bash
cd backend
python -m venv venv
venv\Scripts\activate      # On Windows
uvicorn main:app --reload
```

Backend runs at 👉 **http://127.0.0.1:8000**

API documentation 👉 **http://127.0.0.1:8000/docs**

---

### 🌐 3️⃣ Run the Frontend

```bash
cd ../frontend
npm install
npm run dev
```

Frontend runs at 👉 **http://localhost:5173**

---

## 🧪 Testing & HTML Report

To run test cases:

```bash
pytest --html=reports/report.html --self-contained-html
```

✅ This will generate a detailed test report at:
```
backend/reports/report.html
```

Open it in any browser to view results.

---

## 💭 Design Decisions & Trade-offs

- Focused on a **simple, working MVP** for single-doctor clinics.  
- No authentication for faster appointment flow.  
- SQLModel chosen for easy ORM integration with FastAPI.  
- Separated frontend and backend for modularity.  

---

## 🌱 Future Enhancements

- Add authentication for doctors  
- Implement email/SMS reminders for patients  
- Add analytics dashboard for appointments  
- Deploy using Docker + Render/Vercel  

---

## 👩‍💻 Author
**Rakshitha K**  
