# 🎓 Django Student Management System

A web-based Student Management System built using Django. This project allows users to perform **CRUD operations (Create, Read, Update, Delete)** on student records through both the **web interface** and the **Django admin panel**. The project uses Django models to manage the database and implements CSRF protection for secure form submissions.

---

## 📌 Features

- Add, view, edit, and delete student details
- Perform CRUD operations via:
  - Web interface
  - Django Admin panel
- Uses Django Models for database management
- CSRF token implemented for security
- Clean and responsive user interface (can be extended with Bootstrap)

---

## ⚙️ Technologies Used

- Python 3.x
- Django 4.x (or your version)
- SQLite3 (default database; can be changed)
- HTML/CSS (for frontend)
- Django Templating Language

---

## 🗃️ Database Schema

The data is managed using Django’s ORM via a `Student` model. Each student record contains:

- Full Name
- Email Address
- Roll Number
- Course / Department
- Additional Fields (if any)

You can define this model in `models.py`.

---

## 🔐 Security

- **CSRF Token** is used to protect all form submissions from cross-site request forgery attacks.
- Admin access is protected by Django’s built-in authentication system.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Student-Management-System.git
cd Student-Management-System
2. Create Virtual Environment & Install Dependencies
bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
3. Apply Migrations & Create Superuser
bash
Copy
Edit
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
4. Run the Server
bash
Copy
Edit
python manage.py runserver
Visit http://127.0.0.1:8000/ for the frontend interface and http://127.0.0.1:8000/admin/ for the admin panel.

📁 Project Structure
cpp
Copy
Edit
student_management/
├── student_app/
│   ├── migrations/
│   ├── templates/
│   ├── static/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── forms.py
├── student_management/
│   ├── settings.py
│   ├── urls.py
├── db.sqlite3
├── manage.py
└── README.md
