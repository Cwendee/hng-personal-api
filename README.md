# HNG Personal API

A minimal REST API built with Python (FastAPI) and deployed on a VPS with Nginx reverse proxy.

## Run Locally

```bash
git clone https://github.com/Cwendee/hng-personal-api.git
cd hng-personal-api
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8000
```

## Endpoints

| Method | Endpoint | Response |
|--------|----------|----------|
| GET | `/` | `{"message": "API is running"}` |
| GET | `/health` | `{"message": "healthy"}` |
| GET | `/me` | `{"name": "Prudence Anumudu", "email": "pruddyanumudu@gmail.com", "github": "https://github.com/Cwendee"}` |

## Live URL

http://136.107.152.251