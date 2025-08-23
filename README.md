# 🎥 Peppo Video App – AI-Powered Video Idea Generator

A simple, provider-agnostic web app that helps generate **video ideas** and **optimize prompts** using AI.  
- ⚡ **FastAPI** backend + Jinja2 templates frontend (no build step)  
- ✨ **Creative idea generation** and **prompt optimization**  
- 🗂️ Clear project structure with providers & services  
- 🔑 **API key configurable** via `.env` (never hardcoded)  
- 🌍 Deployable on **Vercel / Render** with environment variables  

---

## 🌐 Demo
👉 Live App URL: [https://peppo-video-app-new.vercel.app/](https://peppo-video-app-new.vercel.app/)

---

## 📂 Project Structure

```bash
.
├── api/                # API endpoints
├── app/                # Core application logic
│   ├── providers/      # External provider integrations
│   ├── services/       # Business logic and services
│   ├── static/         # Static files (CSS, JS, images)
│   └── templates/      # HTML templates
├── .venv/              # Virtual environment (ignored in git)
└── README.md           # Project documentation

---

## ⚙️ Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/your-username/peppo-video-app.git
cd peppo-video-app

# 2. Create virtual environment
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Setup environment variables
cp .env.example .env   # then add your keys inside

# 5. Start the app
uvicorn app.main:app --reload
