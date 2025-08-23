# Peppo AI – Minimal Prompt→Video App

A tiny, provider-agnostic web app that takes a text prompt and returns a short video.
- **FastAPI** backend + minimal HTML frontend (no build step)
- **Style presets** and **RAG-lite prompt composer**
- **Caching** by prompt hash
- **Mock provider** guarantees end-to-end even if rate-limited
- Deployable to **Render/Railway** with env vars (no keys in Git)

## Demo
Public URL: (add after deploy)

## Stack
FastAPI, Jinja2 templates, vanilla JS, Render (or Railway)

## Run locally
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env
uvicorn app.main:app --reload
