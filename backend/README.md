# Backend Module

This folder contains the server-side logic for RapidResQ.

## What's here
- Django project — emergency classification logic
- Database models (SQLite for development)
- API endpoints consumed by the Flutter app (`app/`)

## Tech
- Django (Python)
- SQLite (dev database)

## Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## API docs
See `docs/api.md` (or `openapi.yaml`, once added) for endpoint contracts.
