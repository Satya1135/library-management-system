# 📚 Library Management System

A web-based **Library Management System** developed using **Python and Django**. The application provides separate interfaces for administrators and students to manage library operations such as books, student registration, book issuing, due dates, and fine calculation.

## 🚀 Features

### 👨‍💼 Admin

* Admin registration and login
* Add new books
* View available books
* Issue books to students
* View issued books
* View registered students
* Calculate overdue fines
* Role-based access control

### 👨‍🎓 Student

* Student registration and login
* Student profile information
* View issued books
* View book issue and expiry dates
* View applicable fines

### 📖 Book Management

* Add books with:

  * Book name
  * ISBN
  * Author
  * Category
* Support for multiple book categories
* Track issued books

### 💰 Fine Management

The system calculates fines for overdue books.

* Standard borrowing period: **15 days**
* Fine after the due period: **₹10 per additional day**

## 🛠️ Technologies Used

* **Python**
* **Django**
* **SQLite**
* **HTML5**
* **CSS3**
* **JavaScript**
* **Bootstrap / Django Widget Tweaks**

## 🏗️ Project Structure

```text
library-management-system/
│
├── library/
│   ├── migrations/
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── librarymanagement/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── static/
├── templates/
├── manage.py
├── requirements.txt
└── README.md
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/library-management-system.git
```

### 2. Navigate to the project

```bash
cd library-management-system
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

#### Windows

```bash
venv\Scripts\activate
```

#### Linux / macOS

```bash
source venv/bin/activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Apply database migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 7. Create an administrator account

```bash
python manage.py createsuperuser
```

Follow the prompts to create the admin account.

### 8. Start the development server

```bash
python manage.py runserver
```

Open the application in your browser:

```text
http://127.0.0.1:8000/
```

## 🔐 Authentication

The system uses Django's authentication framework and separates users into:

* **ADMIN**
* **STUDENT**

Access to administrative functions is restricted to users belonging to the administrator group.

## 🗃️ Database Models

The application contains three primary models:

### StudentExtra

Stores additional student information such as:

* Enrollment number
* Branch
* User account

### Book

Stores:

* Book name
* ISBN
* Author
* Category

### IssuedBook

Stores:

* Student enrollment
* Book ISBN
* Issue date
* Expiry date

## 🎯 Project Objective

The main objective of this project is to digitize common library operations and provide a simple platform for managing students, books, and book circulation.

## 🔮 Future Enhancements

Possible future improvements include:

* Online book search
* Book availability tracking
* Email notifications for due dates
* Automatic overdue reminders
* Advanced search and filtering
* Book reservation system
* Dashboard with library statistics
* REST API integration
* PostgreSQL/MySQL database support
* Deployment using a cloud platform

## 👨‍💻 Author

**G. S. N. Gupta**

B.Tech – Information Technology
Interested in Cybersecurity, Networking and Web Development.

## 📄 License

This project is intended for educational and portfolio purposes.
