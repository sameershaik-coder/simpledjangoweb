# Simple Django Web Application

A basic Django web application with a landing page.

## Setup Instructions

1. **Create a virtual environment:**
   ```bash
   python -m venv venv
   ```

2. **Activate the virtual environment:**
   - Windows PowerShell:
     ```powershell
     .\venv\Scripts\Activate.ps1
     ```
   - Windows CMD:
     ```cmd
     venv\Scripts\activate.bat
     ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run migrations:**
   ```bash
   python manage.py migrate
   ```

5. **Start the development server:**
   ```bash
   python manage.py runserver
   ```

6. **Access the application:**
   Open your browser and navigate to `http://127.0.0.1:8000/`

## Project Structure

```
simpledjangoweb/
├── config/              # Project configuration
│   ├── settings.py      # Django settings
│   ├── urls.py          # Main URL configuration
│   └── wsgi.py          # WSGI configuration
├── home/                # Home app
│   ├── templates/       # HTML templates
│   ├── views.py         # View functions
│   └── urls.py          # App URL patterns
├── manage.py            # Django management script
└── requirements.txt     # Python dependencies
```

## Features

- Landing page with modern design
- SQLite database (default)
- Admin interface available at `/admin/`

## Development

To create a superuser for the admin interface:
```bash
python manage.py createsuperuser
```

## Notes

- This is a basic setup intended for development
- Remember to change the `SECRET_KEY` in production
- Set `DEBUG = False` in production
- Configure `ALLOWED_HOSTS` for production deployment
