🌐 Flask To-Do List (SQLite Version)

A web-based To-Do List application built using Flask and SQLite.
This project is a web version of the desktop Tkinter To-Do app, upgraded with persistent database storage.

🚀 Features

Add new tasks

Delete tasks

Store tasks in SQLite database

Auto-create database table if it doesn't exist

Clean server-side routing

Simple and lightweight web interface

🛠 Tech Stack

Python 3

Flask

SQLite3

HTML (Jinja2 Templates)

📦 Project Structure
project-folder/
│
├── app.py
├── database.db (auto-created)
│
└── templates/
    └── index.html
🧠 How It Works

Flask handles routing and HTTP requests

SQLite stores tasks in a local database file (database.db)

The table is created automatically if it doesn't exist

Tasks are retrieved and displayed dynamically using Jinja2 templates

Each task has a unique ID for deletion

▶️ Installation & Setup
1️⃣ Create Virtual Environment (Recommended)
python -m venv venv

Activate it:

Windows

venv\Scripts\activate

Mac/Linux

source venv/bin/activate
2️⃣ Install Dependencies
pip install flask
3️⃣ Run The App
python app.py
4️⃣ Open in Browser

Go to:

http://127.0.0.1:5000/
🧾 Database Schema
CREATE TABLE users (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    task TEXT NOT NULL
);
📌 Routes Overview
Route	Method	Description
/	GET	Display all tasks
/add	POST	Add new task
/delete/<id>	GET	Delete task
🧠 What This Project Demonstrates

Flask routing

Form handling with request

SQLite database integration

SQL parameterized queries (safe from SQL injection)

CRUD operations

MVC-style structure (Routes + Templates)

🔮 Future Improvements

Add task completion status

Add edit/update task feature

Add user authentication

Add REST API version

Deploy on Render / Railway / PythonAnywhere

📄 License

This project is open-source and built for learning purposes.