<p>
  <img src="Logo-Sortirin-2.png" width="450">
</p>
<h1>Sortir.In</h1>
<p>
AI-Powered Smart Waste Classification Platform
</p>

---

## About

Sortir.In adalah platform berbasis Artificial Intelligence yang membantu masyarakat mengidentifikasi jenis sampah secara otomatis, meningkatkan kesadaran pengelolaan sampah, serta mendukung ekonomi sirkular melalui sistem poin dan edukasi lingkungan.

---

## Main Features

- Real-Time Waste Classification
- AI Waste Detection
- Reward Point System
- Waste Analytics Dashboard

---

## Technology Stack

### Frontend
- React.js
- Tailwind CSS

### Backend
- Node.js
- Express.js
- Postgre SQL

### Artificial Intelligence
- TensorFlow
- MobileNetV2
- CNN Classification Model

### Data Science
- Python
- Streamlit
- Pandas

---

## Repositories

| Repository | Description | Tech Stack |
|------------|-------------|------------|
| [front-end-sortirin](https://github.com/Sortir-In/front-end-sortirin) | Web Application | React.js, Tailwind CSS, Vite |
| [backend-sortirin](https://github.com/Sortir-In/backend-sortirin) | REST API | Node.js, Express.js, PostgreSQL |
| [ml-api-sortirin](https://github.com/Sortir-In/ml-api-sortirin) | AI Classification Service | FastAPI, MobileNetV2, TensorFlow |
| [dashboard-analytics](https://github.com/Sortir-In/dashboard-analytics) | Analytics Dashboard | Python, Streamlit, Pandas |
| [Data-Science](https://github.com/Sortir-In/Data-Science) | Machine Learning & EDA | Python, Jupyter Notebook |

---

## Team

| Nama                          | Cohort-ID      | Path             |
| ----------------------------- | -------------- | ---------------- |
| Muhammad Zaki Al Fajri        | CACC299D6Y2586 | Machine Learning |
| Ahmad Faqih                   | CACC695D6Y1347 | Machine Learning |
| Dwi Fajar Novianto            | CDCC015D6Y2112 | Data Scientist   |
| Nicholas Noverhino Ama Payong | CDCC283D6Y0731 | Data Scientist   |
| Hadi Prio Utomo               | CFCC007D6Y2273 | Full Stack Web   |
| Muhammad Hafizh Raihan        | CFCC007D6Y2266 | Full Stack Web   |

---

## Project Status

Active Development

---

## 📋 Prerequisites

Pastikan sudah terinstall di komputer Anda:

| Tools | Versi Minimum | Keterangan |
|---|---|---|
| [Node.js](https://nodejs.org/) | v18+ | Untuk Frontend & Backend |
| [npm](https://www.npmjs.com/) | v9+ | Package manager Node.js |
| [PostgreSQL](https://www.postgresql.org/) | v14+ | Database Backend |
| [Python](https://www.python.org/) | v3.9+ | Untuk ML API & Dashboard |
| [Git](https://git-scm.com/) | v2+ | Clone repository |
| [Docker](https://www.docker.com/) | v20+ | Opsional, untuk ML API |

---

## 🚀 Cara Menjalankan (Lokal)

### 1. Frontend
```bash
git clone https://github.com/Sortir-In/front-end-sortirin.git
cd front-end-sortirin
npm install
npm run dev
```
Akses di `http://localhost:5173`

---

### 2. Backend
```bash
git clone https://github.com/Sortir-In/backend-sortirin.git
cd backend-sortirin
npm install
```

Buat file `.env`:
```env
DB_USER=postgres
DB_HOST=localhost
DB_NAME=sortirin_db
DB_PASSWORD=your_password
DB_PORT=5432
JWT_SECRET=your_random_secret_key
AI_API_URL=https://klasifikasi-sampah-api-production.up.railway.app
NODE_ENV=development
PORT=5000
```

```bash
# Setup database
psql -U postgres -d sortirin_db -f migration.sql

# Jalankan server
npm run dev
```
Akses di `http://localhost:5000`

---

### 3. ML API
```bash
git clone https://github.com/Sortir-In/ml-api-sortirin.git
cd ml-api-sortirin
pip install -r requirements.txt
uvicorn app:app --host 0.0.0.0 --port 8000 --reload
```
Atau dengan Docker:
```bash
docker build -t ml-api-sortirin .
docker run -p 8000:8000 ml-api-sortirin
```
Akses di `http://localhost:8000`

---

### 4. Dashboard Analytics
```bash
git clone https://github.com/Sortir-In/dashboard-analytics.git
cd dashboard-analytics
pip install -r requirements.txt
streamlit run app.py
```
Akses di `http://localhost:8501`

---

## 🔗 URL Production

| Layanan | URL |
|---|---|
| Frontend | https://sortirin.vercel.app |
| ML API | https://klasifikasi-sampah-api-production.up.railway.app |
| ML API Docs | https://klasifikasi-sampah-api-production.up.railway.app/docs |
| Dashboard Analytics | https://dashboardpengolahansampah-fvwzbqyqs7zgmdcwvevjda.streamlit.app |

---

## 🏗️ Arsitektur Sistem

```
User (Browser/Mobile)
        ↓
  Frontend (React)
        ↓
  Backend REST API (Node.js)
     ↙        ↘
PostgreSQL    ML API (FastAPI)
                   ↓
           Model MobileNetV2
```
