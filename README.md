# Blood Donor Finder

A lightweight blood donor finder web app built with FastAPI and a static frontend. It allows donors to register, patients to search for eligible donors by blood group and city, and administrators to manage donor records and blood requests.

## Features

- Donor registration form
- Smart donor search with 3-month eligibility rule
- Urgent emergency blood request posting
- Admin dashboard for donors and emergency requests
- Local SQLite database for quick setup and running

## Run locally

1. Create a virtual environment if needed.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Start the app:

   ```bash
   python -m uvicorn app.main:app --host 0.0.0.0 --port 8001 --app-dir "."
   ```

4. Open the app in a browser:

   ```text
   http://localhost:8001
   ```

## Main files

- `app/main.py` – FastAPI backend and API logic
- `static/index.html` – website UI
- `static/styles.css` – styling
- `static/app.js` – frontend interactions

## Notes

This project is configured to run locally with SQLite for simplicity. The data model and API structure are aligned with a PostgreSQL-based deployment pattern, so it can be adapted to PostgreSQL later with minimal change.
