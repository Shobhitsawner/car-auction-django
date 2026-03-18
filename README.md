# 🏎️ AutoBid: Django Car Auction Engine
**A robust, MVT-based auction platform featuring dynamic bidding logic and automated media management.**

[![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

---

## 🌟 Overview
AutoBid is a comprehensive web solution for car enthusiasts and dealers. Built on the **Django MVT (Model-View-Template) architecture**, it provides a secure environment for listing vehicles and participating in competitive bidding. The project emphasizes clean code separation, scalable folder structures, and professional backend standards.

### ✨ Key Features
* **🔨 Dynamic Bidding System:** Real-time-style bidding logic with validation to ensure every bid is higher than the last.
* **🖼️ Automated Media Handling:** Structured image upload system for vehicle listings using Django `MEDIA_ROOT`.
* **🛡️ Secure Auction Flow:** Robust backend views to handle car detail retrieval and bid submissions safely.
* **📂 Modular Architecture:** Clean separation between core project configuration (`car_auction`) and business logic (`auction`).
* **🎨 Template Inheritance:** A DRY (Don't Repeat Yourself) frontend approach using a `base.html` master layout.

---

## 🛠️ Tech Stack
| Layer | Technology |
| :--- | :--- |
| **Framework** | Django 4.x / 5.x |
| **Language** | Python 3.10+ |
| **Database** | SQLite (Development) / PostgreSQL Ready |
| **Architecture** | Model-View-Template (MVT) |
| **Styling** | Semantic HTML5 & Custom CSS3 |

---

## 📂 Project Anatomy
```text
car-auction-django/
├── auction/             # Core Business Logic (Car & Bid Models)
│   ├── models.py        # Database Schema: Car, Bid, User
│   ├── views.py         # Auction logic & Validation
│   └── urls.py          # App-specific routing
├── car_auction/         # Global Project Settings & ASGI/WSGI
├── templates/           # Clean UI with Template Inheritance
├── media/               # User-uploaded Vehicle Gallery
├── manage.py            # Django CLI Utility
└── db.sqlite3           # Local Development Database
