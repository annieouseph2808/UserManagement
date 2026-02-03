## User Management System (Django)

## 📌 Project Overview

This is a **User Management System** built using **Django** that implements **JWT (JSON Web Token)–based authentication**.
User authentication is performed using **email instead of username**, and all APIs are documented and testable using **Swagger UI**.

The project includes:

* Secure user authentication using JWT
* Email-based login
* API documentation with Swagger
* Necessary configurations in `urls.py` and `settings.py`

---

**Authorization Header Format:**

```
Authorization: Bearer <your_access_token>
```

---

## 📄 API Documentation (Swagger)

Swagger is integrated to display all required APIs.

Once the server is running, access Swagger UI at:

```
http://127.0.0.1:8000/swagger/
```

This interface allows you to:

* View all available APIs
* Test authentication and protected endpoints
* Understand request and response formats

---

## ⚙️ Configuration Changes

The following files were updated for JWT authentication and Swagger integration:

* **`settings.py`**

  * JWT authentication settings
  * Swagger configuration
  * Installed apps and middleware changes

* **`urls.py`**

  * JWT authentication endpoints
  * Swagger URLs
  * API route configurations

---

## ▶️ How to Run the Project

Follow these steps to run the project locally:

### 1️⃣ Clone the Repository

```bash
git clone <repository_url>
```

### 2️⃣ Navigate to the Project Directory

```bash
cd <project_folder_name>
```

### 3️⃣ (Optional but Recommended) Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 5️⃣ Run Database Migrations

```bash
python manage.py migrate
```

### 6️⃣ Start the Development Server

```bash
python manage.py runserver
```

### 7️⃣ Open in Browser

```
http://127.0.0.1:8000/
```

For API documentation:

```
http://127.0.0.1:8000/swagger/
```

---

## 🛠️ Technologies Used

* **Django**
* **Django REST Framework**
* **JWT Authentication**
* **Swagger (drf-yasg / similar)**
* **Python**

---
