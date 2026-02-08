# 🚗 Django Car Auction System

A Django-based web application that allows users to list cars for auction and participate in a bidding process.  
The project follows Django best practices with a clean separation between project configuration, app logic, templates, and media files.

---

## 📁 Complete Project Structure

car-auction-django/
│
├── auction/ # Main application (auction logic)
│ ├── migrations/ # Database migration files
│ │ └── init.py
│ ├── init.py
│ ├── admin.py # Admin panel configuration
│ ├── apps.py # App configuration
│ ├── models.py # Database models (Car, Bid)
│ ├── tests.py # Unit tests
│ ├── urls.py # App-level routing
│ └── views.py # Business logic & request handling
│
├── car_auction/ # Project configuration
│ ├── init.py
│ ├── asgi.py # ASGI configuration
│ ├── settings.py # Global settings
│ ├── urls.py # Root URL configuration
│ └── wsgi.py # WSGI configuration
│
├── templates/ # HTML templates
│ ├── base.html # Base layout
│ ├── home.html # Home page (auction listings)
│ ├── add_car.html # Add car form
│ ├── car_detail.html # Car details & bidding page
│ ├── login.html # Login page
│ └── signup.html # Signup page
│
├── media/ # Uploaded files
│ └── car_images/ # Uploaded car images
│
├── db.sqlite3 # SQLite database (development)
├── manage.py # Django command-line utility
└── README.md # Project documentation

## 📌 Folder & File Responsibilities

### 🔹 `auction/` (Core Application)
This app contains the **main auction logic**.

- Handles car listings and bidding
- Defines database schema
- Contains application-level URLs and views

Key files:
- `models.py` → Car and Bid models
- `views.py` → Auction flow & bid validation
- `urls.py` → Routes for auction features
- `admin.py` → Admin dashboard setup

---

### 🔹 `car_auction/` (Project Configuration)
Controls **global behavior** of the Django project.

- Application registration
- Middleware
- Database & media settings
- Root URL routing

Key files:
- `settings.py` → Central configuration
- `urls.py` → Connects apps to URLs
- `asgi.py` / `wsgi.py` → Deployment interfaces

---

### 🔹 `templates/` (Frontend Layer)
Contains all HTML templates rendered by Django views.

- Uses template inheritance via `base.html`
- No JavaScript dependency
- Styled using CSS only

---

### 🔹 `media/` (User Uploads)
Stores all uploaded images (cars listed for auction).

Configured using Django `MEDIA_ROOT` and `MEDIA_URL`.

---

### 🔹 Root Files
- `manage.py` → Run server, migrations, admin commands
- `db.sqlite3` → Development database
- `README.md` → Documentation

---

## ✅ Architecture Highlights

- Follows **Django MVT architecture**
- Modular and scalable structure
- Clean separation of concerns
- Suitable for:
  - Academic submissions
  - Internship projects
  - Portfolio demos

---

## 🚀 Conclusion

This project structure ensures:
- Maintainability
- Readability
- Scalability
- Professional Django standards

The application can be easily extended with authentication, payments, or real-time bidding features.
