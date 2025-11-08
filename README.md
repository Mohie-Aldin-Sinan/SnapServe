<div align="center">

# 📸 SnapServe

### ⚡ A Full-Stack FastAPI + Streamlit App Managed with `uv`

![Python](https://img.shields.io/badge/Python-3.11%2B-blue?logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?logo=fastapi)
![Streamlit](https://img.shields.io/badge/Streamlit-Frontend-FF4B4B?logo=streamlit)
![uv](https://img.shields.io/badge/uv-Dependency%20Manager-4B8BBE?logo=python)
![ImageKit](https://img.shields.io/badge/ImageKit-Integrated-00C4CC?logo=imagekit)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

</div>

---

## 🧠 About SnapServe

**SnapServe** is a modern **FastAPI + Streamlit** web app for uploading and viewing photos with user authentication and cloud media storage via **ImageKit**. It combines the power of **FastAPI (async backend)**, **SQLAlchemy ORM**, and a **Streamlit frontend**, managed with **uv** — making it a clean, fast, and developer-friendly full-stack project.

---

## 🚀 Features

✅ **User Authentication** — Register, Login, JWT (FastAPI Users)  
✅ **Image Uploads** — Upload media with captions (via ImageKit)  
✅ **Dynamic Feed** — View photos sorted by upload time  
✅ **Async Database** — Fast performance using async SQLAlchemy  
✅ **Modular Design** — Clean separation between backend & frontend  
✅ **Streamlit UI** — Lightweight and interactive dashboard  
✅ **uv Managed** — Fast, reproducible environment setup  

---

## 🧰 Tech Stack

| Layer | Technology |
|-------|-------------|
| 🌐 **Frontend** | Streamlit |
| ⚙️ **Backend** | FastAPI |
| 🧠 **Database** | SQLite + SQLAlchemy (Async) |
| 🔐 **Authentication** | FastAPI Users (JWT) |
| ☁️ **Storage** | ImageKit Cloud |
| 🧩 **Dependency Manager** | uv |

---

## ⚙️ Installation & Setup
```bash
### 1️⃣ Clone the repository
git clone https://github.com/Mohie-Aldin-Sinan/SnapServe.git
cd SnapServe

### 2️⃣ Install dependencies
uv sync

### 3️⃣ Create a `.env` file
DATABASE_URL=sqlite+aiosqlite:///./test.db
SECRET=your-secret-key
IMAGEKIT_PRIVATE_KEY=your-private-key
IMAGEKIT_PUBLIC_KEY=your-public-key
IMAGEKIT_URL_ENDPOINT=https://ik.imagekit.io/your-id

### 4️⃣ Run the FastAPI backend
uv run main.py
# Docs: http://localhost:8000/docs

### 5️⃣ Run the Streamlit frontend
uv run streamlit run frontend.py
# App: http://localhost:8501

## 📁 Project Structure
SnapServe/
│
├── app/
│   ├── app.py         # FastAPI main app
│   ├── db.py          # Async DB setup
│   ├── models.py      # User & Post models
│   ├── users.py       # Auth and user logic
│   ├── schemas.py     # Pydantic schemas
│   ├── images.py      # Upload/feed endpoints
│   └── ...
│
├── frontend.py        # Streamlit frontend
├── pyproject.toml     # uv dependencies
├── uv.lock
├── .env
└── README.md

## 🧠 Notes
- Fully async backend built with FastAPI + SQLAlchemy
- Integrated with ImageKit for seamless image hosting
- Ready for deployment (Render / Railway + Streamlit Cloud)
- Clean modular structure — easy to extend or modify
