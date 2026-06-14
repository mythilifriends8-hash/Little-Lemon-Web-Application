Project Title
Little Lemon Restaurant API

Description
A restaurant management backend built using Django REST Framework and MySQL.

Installation Steps
1. Install Python 3.12+.
2. Create and activate a virtual environment:
   python -m venv venv
   .\venv\Scripts\activate
3. Install dependencies:
   pip install -r requirements.txt
4. Create a MySQL database named littlelemon_db.
5. Update database credentials in littlelemon/settings.py or set environment variables.
6. Run migrations:
   python manage.py makemigrations
   python manage.py migrate
7. Create a superuser:
   python manage.py createsuperuser
8. Run the server:
   python manage.py runserver

Database Setup
- Install MySQL server.
- Create database littlelemon_db.
- Grant access to a MySQL user.

Migration Commands
python manage.py makemigrations
python manage.py migrate

Server Run Commands
python manage.py runserver

Testing Commands
python manage.py test

GitHub Instructions
git init
git add .
git commit -m "Initial Little Lemon Restaurant API"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main

API Endpoints
Home Page: /
Authentication: /api/register/ /api/login/
Menu: /api/menu/ /api/menu/{id}/
Bookings: /api/bookings/ /api/bookings/{id}/

Sample Credentials
username: admin
password: <your-password>

Insomnia Testing Instructions
Use POST /api/register/ to create a user and POST /api/login/ to retrieve a token.
Send Authorization: Token <token> for protected POST/PUT/DELETE requests.

CI / GitHub Actions
The repository includes `.github/workflows/ci.yml` to run migrations and tests on push and pull request.

Peer Review Checklist
✓ Django serves HTML
✓ MySQL Connected
✓ CRUD APIs Working
✓ Authentication Implemented
✓ Unit Tests Passing
✓ GitHub Repository Available
✓ Insomnia Compatible
