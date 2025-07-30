Perfect! Here are the exact commands to run the project:

## Backend (Django) Setup

**Path:** `django_backend/`

```bash
# 1. Create and activate virtual environment
python -m venv backend-env
source backend-env/bin/activate  # On Windows: backend-env\Scripts\activate

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run migrations
python manage.py migrate

# 4. Start the Django server
python manage.py runserver
```

The backend will run on `http://localhost:8000`

## Frontend (React) Setup

**Path:** `frontend/`

```bash
# 1. Install dependencies
pnpm install

# 2. Start the development server
pnpm dev
```

The frontend will run on `http://localhost:5173` (or another port if 5173 is busy)

## Summary

1. **Terminal 1** (Backend): Navigate to `django_backend/` and run the Django commands
2. **Terminal 2** (Frontend): Navigate to `frontend/` and run the React commands

Both servers need to be running simultaneously for the full application to work. The frontend will communicate with the backend API at `http://localhost:8000`.