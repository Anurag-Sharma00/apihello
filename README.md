# 🌐 Django Project Setup Guide

## ⚙️ **Project Structure**

```
myproject/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── manage.py
└── myproject/
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    └── api/
        ├── __init__.py
        ├── views.py
        └── urls.py
```

---

## 🔧 **Step 1: Django Setup Instructions**

### 💻 Prerequisites:

- Install Python from [Python Official Website](https://www.python.org/downloads/)

### 🔗 Install Required Dependencies:

1. Open your terminal or command prompt.
2. Run the following commands to install Django and additional packages:

```bash
pip install django
pip install mysqlclient
pip install djangorestframework
```

### 🎮 Create Your Django Project:

1. Create a new Django project by running:
   ```bash
   django-admin startproject myproject
   ```
2. Move into the project directory:
   ```bash
   cd myproject
   ```

---

## 🛠️ **Running the Project Without Docker**

### 🌐 Create a Virtual Environment:

1. Create a virtual environment:
   ```bash
   python -m venv venv
   ```
2. Activate the virtual environment:
   - **Windows**:
     ```bash
     venv\Scripts\activate
     ```
   - **Mac/Linux**:
     ```bash
     source venv/bin/activate
     ```

### 📊 Install Required Packages:

```bash
pip install -r requirements.txt
```

### 🏢 Apply Migrations:

```bash
python manage.py migrate
```

### ⚙️ Run the Server:

```bash
python manage.py runserver
```

- Your project will now be available at: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
- And your API will now be available at: [http://127.0.0.1:8000/api/hello](http://127.0.0.1:8000/api/hello/)

---

## 🛠️ **Running the Project with Docker**

### ⚓ Build and Run the Docker Containers:

1. Use the following command to build and start your Docker containers:
   ```bash
   docker-compose up --build
   ```
2. Your project will now be available at the URL specified in your `docker-compose.yml` file.

---

## 📊 **Useful Notes**:

- Ensure that `requirements.txt` contains all necessary dependencies for your project.
- Configure your `settings.py` file for database settings if you're using MySQL.

---

🛡️ **Happy Coding!** 🚀

Developed by Anurag 
