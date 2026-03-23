# 🚀 Fullstack PaaS Platform Starter

> A fullstack mock PaaS platform built with **Vue + Django**, integrated with **Tencent BlueKing (BK) ecosystem**, designed as a teaching-oriented platform scaffold.

---

## 📌 Overview

This project is a **fullstack PaaS (Platform-as-a-Service) simulation system** that includes both a frontend management console and a backend service architecture.

It is built based on the development paradigm of **Tencent BlueKing (BK) PaaS ecosystem**, aiming to simulate real-world platform development, deployment, and API interaction.

The project provides:

- A Vue-based admin dashboard
- A Django-based backend service
- BlueKing API Gateway SDK integration
- Local mock server and PaaS API simulation layer

> 🏫 This project was developed as part of an academic/experimental project in collaboration with Tencent BlueKing development concepts.

---

## 🧱 Tech Stack

### Frontend
- Vue.js
- Vue Router
- Vuex
- PostCSS
- Component-based architecture (Auth / Exception / Dashboard)
- Local mock-server and paas-server for API simulation

```
frontend/
├── src/
│   ├── api/            # API layer
│   ├── components/     # Shared components (Auth / Exception)
│   ├── views/          # Pages (Dashboard / Examples)
│   ├── router/         # Routing
│   ├── store/          # State management
│   └── common/         # Utilities
├── mock-server/        # Mock API server
├── paas-server/        # Local PaaS simulation layer
```

---

### Backend
- Python
- Django
- Gunicorn
- Tencent BlueKing SDK (API Gateway integration)

```
backend/
├── home_application/   # Main application module
├── blueking/           # BlueKing SDK
├── core/               # Middleware
├── config/             # Environment configs (dev/prod/stag)
├── templates/          # Server-side templates
├── static/             # Static assets
├── manage.py
└── wsgi.py
```

---

## ☁️ Tencent BlueKing Integration

This project integrates with the **Tencent BlueKing (BK) PaaS ecosystem**, including:

- BlueKing API Gateway SDK
- Standard PaaS application structure (`app_desc.yaml`)
- Multi-environment configuration (dev / stag / prod)
- Gunicorn-based deployment

### Notes
- The backend structure follows BlueKing PaaS application conventions
- Suitable for learning enterprise-level PaaS development patterns
- Simulates real-world API gateway usage and deployment workflow

---

## ✨ Features

- 📊 Dashboard system
- 🔐 Authentication component (Auth)
- ⚠️ Exception handling pages (e.g., 404)
- 🧪 Example modules (Example1–Example4)
- 🔌 Mock API layer (mock-server)
- ☁️ PaaS API simulation (paas-server)
- 🗄️ Backend API & database models (Django)

---

## 🚀 Getting Started

### 1️⃣ Backend Setup

```bash
cd backend
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Or run with Gunicorn:

```bash
gunicorn wsgi -w 4 -b :8000
```

---

### 2️⃣ Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 📦 Deployment

This project supports standard PaaS-style deployment:

- Uses `app_desc.yaml` for application definition
- Backend served via Gunicorn
- Supports multiple environments (dev / prod / stag)

---

## 🎯 Project Purpose

This project is suitable for:

- 🧑‍💻 Fullstack development practice (Vue + Django)
- ☁️ Understanding PaaS platform architecture
- 🏫 Academic coursework / lab projects
- 🧱 Platform-style application scaffolding

---

## ⚠️ Disclaimer

- This is a teaching/demo project and does not include full production-level security or permission systems
- BlueKing-related integrations are simplified and intended for learning purposes

---

## 👨‍💻 Author

- GitHub: ZijinTuTu

---

## 📄 License

MIT License

---

## 📈 Resume Highlight (Optional)

> Built a fullstack mock PaaS platform based on Tencent BlueKing architecture using Vue and Django, including a dashboard system, API simulation layer, and backend deployment pipeline.
