# SkillSpree

SkillSpree is a personalized education platform that provides tailored learning goals, dynamically generated assessments, and personalized course recommendations.

## Tech Stack
- **Backend:** Python, Flask (Application Factory pattern)
- **Database:** MongoDB
- **AI:** Google Gemini API
- **Other:** YouTube API, Jinja templates

## Project Structure

```
.
├── .env.example          # Environment variables template
├── README.md             # Project documentation
├── app/                  # Main application package
│   ├── __init__.py       # App factory and configuration
│   ├── main/             # Main blueprint
│   │   ├── __init__.py   # Blueprint initialization
│   │   └── routes.py     # All application routes
│   ├── ml_utils.py       # Gemini AI integration logic
│   ├── templates/        # Jinja HTML templates
│   └── youtube_utils.py  # YouTube API logic
├── config.py             # Centralized settings
├── requirements.txt      # Pinned project dependencies
└── run.py                # Application entry point
```

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/adityapandereio6-sketch/SKILLSPREE.git
   cd SKILLSPREE
   ```

2. **Create and activate a virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate
   ```

3. **Install the dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   ```bash
   cp .env.example .env
   ```
   Then edit `.env` and set `SECRET_KEY`, `MONGO_URI`, `DB_NAME`, and `GOOGLE_API_KEY`.
   Update `MONGO_URI` if MongoDB isn't running on localhost.

5. **Start the application**:
   ```bash
   python run.py
   ```
   The server starts on `http://localhost:5000`.

## Authors
Built by Aditya Pandere and Vinit Chougale.
