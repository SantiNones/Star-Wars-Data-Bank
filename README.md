# 🌌 Star Wars REST API

> **A robust backend API built with Python and Flask to manage complex data relationships for a Galactic Encyclopedia.**

![Project Status](https://img.shields.io/badge/Status-Backend_Ready-success)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Tech](https://img.shields.io/badge/Stack-Python_Flask_SQLAlchemy-blue)

## 📖 About the Project

This repository hosts the **Server-Side logic and Database Schema** for the Star Wars Data Bank application.

The core focus of this project is **Data Modeling** and **API Architecture**. I designed a relational database capable of handling complex interactions between users, characters, planets, and vehicles, exposing this data through a structured RESTful API.

### 💡 The Engineering Challenge
The goal was to move away from static data and build a dynamic system where:
1.  **Relationships matter:** Planets have residents, characters drive vehicles.
2.  **User persistence:** Users can manage a private list of "Favorites" stored in the database.
3.  **Efficiency:** Optimized SQL queries using SQLAlchemy ORM.

---

## ✨ Key Features

* **🗂️ Advanced Data Modeling:** Normalized database schema handling One-to-Many and Many-to-Many relationships.
* **🔌 RESTful Endpoints:** Fully functional API supporting GET, POST, and DELETE operations.
* **🛡️ Error Handling:** Structured HTTP responses for reliable client-side consumption.
* **👤 User Management:** Backend logic to handle user creation and their specific associations (Favorites).
* **🎛️ Admin Panel:** Integration with Flask-Admin for quick database management and visualization.

---

## 🛠️ Tech Stack

* ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) **Python 3**
* ![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white) **Flask**: API Framework.
* ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-black?style=flat&logo=python&logoColor=white) **SQLAlchemy**: ORM for Python.
* **PostgreSQL**: Production Database.
* **Pipenv**: Dependency management.

---

## 📡 API Documentation

Here are the main endpoints available in this API:

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/people` | Retrieve a list of all characters. |
| `GET` | `/people/<int:id>` | Retrieve details of a specific character. |
| `GET` | `/planets` | Retrieve a list of all planets. |
| `GET` | `/planets/<int:id>` | Retrieve details of a specific planet. |
| `GET` | `/users` | List all users. |
| `GET` | `/users/favorites` | Get all favorites for the current user. |
| `POST` | `/favorite/planet/<int:planet_id>` | Add a planet to favorites. |
| `POST` | `/favorite/people/<int:people_id>` | Add a character to favorites. |
| `DELETE` | `/favorite/planet/<int:planet_id>` | Remove a planet from favorites. |

---

## 💻 Installation & Local Setup

**1. Clone the repository**
```bash
