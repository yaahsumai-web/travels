# TravelWise

A Flask + Gemini API domain-based chatbot for **Travel**.

## Files
- `app.py` — Flask backend and Gemini API integration
- `templates/index.html` — chatbot UI
- `chatbot_config.py` — domain configuration and system prompt
- `requirements.txt` — Python dependencies
- `render.yaml` — Render deployment configuration
- `.python-version` — supported Python version
- `.env.example` — environment variable template
- `.gitignore` — keeps secrets out of Git

## Environment variable
Set this in Render:
`GEMINI_API_KEY=your_key_here`

Optional:
`GEMINI_MODEL=gemini-3.8-flash`

## Render
The included `render.yaml` uses:
- Build: `pip install -r requirements.txt`
- Start: `gunicorn app:app`

Do not commit a real API key. Use Render Environment Variables and keep `.env` local.
