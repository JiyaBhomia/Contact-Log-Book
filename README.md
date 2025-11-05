# Contact Log Book - Full Stack Project

This is a full-stack, decoupled contact management application.

* The **Backend** is a Django REST Framework API that handles all data, logic, and user authentication.
* The **Frontend** is a separate Django project that serves HTML/JavaScript and consumes the backend API.

---

## 🚀 How to Run the Project

To run this application, you **must run both servers at the same time** in two separate terminals.

### 1. Backend Server (Port 8001)

1.  Clone this repository (`contact-book-drf`).
2.  Navigate into the `contact_api_backend` folder.
3.  Create a virtual environment and activate it.
4.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
5.  Run database migrations:
    ```bash
    python manage.py migrate
    ```
6.  Create a superuser to log in with:
    ```bash
    python manage.py createsuperuser
    ```
7.  Run the server:
    ```bash
    python manage.py runserver 8001
    ```

### 2. Frontend Server (Port 8000)

1.  In a **new terminal**, clone the frontend repository.
2.  Navigate into the `contact_project` folder.
3.  Create a virtual environment and activate it.
4.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
5.  Run the server:
    ```bash
    python manage.py runserver 8000
    ```

---

## 🛠️ Technology Used

* **Backend:**
    * Python
    * Django
    * Django REST Framework
    * Simple JWT (for token authentication)
    * SQLite3

* **Frontend:**
    * Django (to serve templates)
    * HTML
    * JavaScript (using `fetch` to consume the API)
