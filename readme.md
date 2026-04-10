# 💊 Affordable Medicine Intelligence Platform

## 🚨 Problem

Medicines with the same active ingredient are sold under different brand names at drastically different prices. Patients often overpay due to lack of awareness of cheaper generic alternatives.

---

## 🎯 Solution

A full-stack platform that:

* Identifies medicine composition (salt, dosage, form)
* Finds equivalent generic and branded alternatives
* Compares prices and highlights savings
* (Optional) Shows nearby availability

---

## 🏗️ Project Structure

```
root/
│
├── frontend/        # React UI
├── backend/         # API server
├── data/            # JSON datasets (Jan Aushadhi, Kaggle)
└── README.md
```

---

## ⚙️ Tech Stack

### Frontend

* React.js
* Tailwind CSS
* Axios (API calls)

### Backend

* Node.js + Express *(or FastAPI)*
* REST APIs
* JSON-based data processing

---

## 🔌 API Endpoints (Backend)

### 1. Search Medicine

```
GET /api/search?name=acugesic
```

### 2. Get Alternatives

```
GET /api/alternatives?generic=tramadol
```

### 3. Price Comparison

```
GET /api/compare?name=acugesic
```

---

## 🧠 How It Works

1. User searches medicine (or uploads prescription)
2. Backend:

   * Normalizes name
   * Identifies generic (salt)
   * Matches all equivalent drugs
3. Returns:

   * Active ingredient
   * Alternatives
   * Price comparison
4. Frontend displays:

   * Clean comparison UI
   * Savings highlight

---

## ▶️ Running the Project

### 1. Clone Repo


git clone <https://github.com/Shiva9801/Dynamic_Devs>
cd project-folder


---

### 2. Run Backend

```
cd backend
npm install
npm start
```

Server runs on:

```
http://localhost:5000
```

---

### 3. Run Frontend

```
cd frontend
npm install
npm run dev
```

Frontend runs on:

```
http://localhost:5173
```

---

## 🔗 Frontend ↔ Backend Connection

Frontend calls backend APIs like:

```
http://localhost:5000/api/search
```

Make sure CORS is enabled in backend.

---

## 📊 Example Output

**Input:** Acugesic Injection

**Output:**

* Generic: Tramadol HCl
* Price: ₹4.69
* Alternatives:

  * Amadol → ₹25
  * Actodol → ₹24.5

💰 Save up to **80%**

---

## 📂 Data Sources

* Jan Aushadhi dataset (generic medicine pricing)
* Kaggle pharmaceutical datasets

---

## 🚀 Future Scope

* Live pharmacy inventory integration
* Prescription OCR (image → text)
* Government approval verification
* Mobile app

---

## ⚠️ Disclaimer

For informational purposes only. Always consult a doctor before changing medication.

---

## 👨‍💻 Team

* Your Name(s)

---
