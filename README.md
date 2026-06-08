# MindMend

MindMend is a Django-based mental health support platform that includes user authentication, assessments, counsellor booking, chat, forums, and analytics features.
Deployed project: https://mindmend-1.onrender.com/

## Key Features

- User registration, login, password reset, and profile management
- Counsellor booking system with anonymous booking support
- Real-time chat and counsellor session interface using Django Channels
- Mood tracking, sleep logging, and mental health assessments
- Forum for discussion and community support
- Admin and counsellor dashboards with analytics and session management
- Google Generative AI and OpenAI integration for support features

## Technologies

- Python 3
- Django 6.x
- Django Channels
- Daphne
- Django REST Framework
- PostgreSQL support via dj-database-url
- Gunicorn for deployment
- Whitenoise for static file hosting
- Razorpay for payment integration
- Pillow and ReportLab for image and PDF handling
- Cryptography for encryption support

## Repository Structure

- MindMend/ - Django project configuration and settings
- Mind_Mend/ - Main application with models, views, serializers, forms, templates, and services
- 	emplates/ - Project-level HTML templates
- static/ - Static assets such as CSS and images
- media/ - Uploaded media files (excluded from source control)
- 
equirements.txt - Python package dependencies
- Dockerfile / docker-compose.yml - Container configuration for deployment

## Setup and Installation

1. Clone the repository:
   `ash
   git clone https://github.com/Akash-raj-INT/MindMend.git
   cd MindMend-main
   `
2. Create and activate a Python virtual environment:
   `ash
   python -m venv venv
   .\venv\Scripts\Activate
   `
3. Install dependencies:
   `ash
   pip install -r requirements.txt
   `
4. Create a .env file and configure environment variables (database, secret key, OpenAI keys, Razorpay keys, etc.)
5. Apply migrations:
   `ash
   python manage.py migrate
   `
6. Run the development server:
   `ash
   python manage.py runserver
   `

## Docker

To run with Docker:

`ash
docker compose up --build
`

## Notes

- Deployed project: https://mindmend-1.onrender.com/
- db.sqlite3 and media/ are excluded from git via .gitignore.
- Update environment variables before running in production.

## License

This project does not include a license file. Add one if you wish to publish or share it under specific terms.
