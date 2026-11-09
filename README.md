# Blog App

A Django blog with full post CRUD and user sign-up, built while following a Django course/book.

## Features

- List, detail, create, update, and delete blog posts using class-based views
- `Post` model (title, author, body) linked to Django's built-in `User`
- User registration via a `SignUp` view, plus Django's login/logout auth URLs
- Static files served with WhiteNoise; deployment config for Render (`render.yaml`, `build.sh`, Gunicorn)

## Built with

- Django 5.1
- `dj-database-url` (SQLite by default, PostgreSQL via `psycopg2-binary`)
- Gunicorn, Uvicorn, WhiteNoise

## Run it

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Learning project.
