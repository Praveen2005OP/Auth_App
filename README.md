# Flask Authentication App

## 📌 Project Overview

This project is a simple authentication system built using Flask. It
allows users to register, log in, access a protected dashboard, and log
out securely.

The application uses SQLite as the database and bcrypt for password
hashing.

------------------------------------------------------------------------

## 🚀 Features

-   User Registration
-   Secure Login System
-   Password Hashing using bcrypt
-   Session-based Authentication
-   Protected Dashboard
-   Logout Functionality
-   SQLite Database Integration
-   Bootstrap 5 UI

------------------------------------------------------------------------

## 🛠 Technologies Used

-   Python
-   Flask
-   Flask-SQLAlchemy
-   SQLite
-   bcrypt
-   Bootstrap 5
-   Gunicorn (for deployment)

------------------------------------------------------------------------

## 📂 Project Structure

FlaskAuth_app/ │ ├── app.py ├── requirements.txt ├── Procfile ├──
instance/ ├── templates/ │ ├── base.html │ ├── index.html │ ├──
login.html │ ├── register.html │ └── dashboard.html └── README.md

------------------------------------------------------------------------

## ⚙️ Installation & Setup

### 1. Clone the Repository

git clone https://github.com/your-username/FlaskAuth_app.git cd
FlaskAuth_app

### 2. Create Virtual Environment

python -m venv venv

Activate it:

Windows: venv`\Scripts`{=tex}`\activate`{=tex}

Mac/Linux: source venv/bin/activate

### 3. Install Dependencies

pip install -r requirements.txt

### 4. Run the Application

python app.py

The app will run on: http://127.0.0.1:5000/

------------------------------------------------------------------------

## 🗄 Database

-   SQLite database file: database.db
-   Tables are automatically created on first run.

------------------------------------------------------------------------

## 🔐 Authentication Flow

1.  User registers with name, email, and password.
2.  Password is hashed using bcrypt before storing.
3.  User logs in using email and password.
4.  Session stores the logged-in user.
5.  Dashboard is accessible only after login.
6.  Logout clears the session.

------------------------------------------------------------------------

## 🌐 Deployment

To run using Gunicorn:

gunicorn app:app

------------------------------------------------------------------------

## ⚠️ Note

For production use: - Change the secret key in app.py - Use environment
variables - Use a production database like PostgreSQL - Enable HTTPS

------------------------------------------------------------------------

## 📜 Author

Praveen Kumar Sharma
Created as part of an academic assignment.
