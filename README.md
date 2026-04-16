# HNG Personal API

A minimal REST API built with **FastAPI**, deployed on a VPS using **Nginx reverse proxy** and managed with **systemd** for persistent uptime.

---

## 🚀 Live URL

http://136.107.152.251

---

## 📌 Endpoints

### GET /

Returns:

```json
{"message": "API is running"}
```

### GET /health

Returns:

```json
{"message": "healthy"}
```

### GET /me

Returns:

```json
{
  "name": "Prudence Anumudu",
  "email": "pruddyanumudu@gmail.com",
  "github": "https://github.com/Cwendee"
}
```

---

## 🛠️ Run Locally

```bash
git clone https://github.com/Cwendee/hng-personal-api.git
cd hng-personal-api

python3 -m venv venv
source venv/bin/activate

pip install -r requirements.txt
uvicorn main:app --host 127.0.0.1 --port 8000
```

---

## ⚙️ Deployment Overview

* Application runs on a **private port (8000)**
* **Nginx** handles incoming HTTP traffic on port 80
* Requests are reverse proxied to the FastAPI app
* **systemd service** ensures the API stays running automatically

---

## ✅ Key Features

* Fast response time (<500ms)
* JSON responses with correct headers
* Persistent background service
* Reverse proxy setup for secure exposure
