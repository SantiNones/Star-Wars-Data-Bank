# 🌌 Star Wars Data Bank

> **A comprehensive Galactic Encyclopedia built with React and Python. Browse the galaxy, discover characters, and manage your favorite assets.**

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Tech](https://img.shields.io/badge/Stack-PERN-blueviolet)

## 📖 About the Project

**Star Wars Data Bank** is a Full Stack web application that interacts with a complex relational database to display detailed information about the Star Wars universe.

Unlike a simple static page, this project focuses on **Data Modeling**. I designed a robust REST API capable of handling relationships between **Planets, Characters, and Vehicles**, while allowing users to interact with this data by saving items to their personal "Favorites" list via a Global State.

### 💡 Why I built this?
This project was a deep dive into **SQLAlchemy** and **Relational Databases**. The main challenge was to architect a backend that serves connected data efficiently and a frontend that manages that data dynamically without refreshing the page.

---

## ✨ Key Features

* **🗂️ Complex Data Models:** Explore interconnected data. See which characters belong to which planets and what vehicles they drive.
* **❤️ Favorites System:** A dynamic "Like" feature allowing users to add People, Planets, or Vehicles to their personal dashboard using **React Context API**.
* **🔎 Detailed Views:** dedicated views for every entity in the database with specific attributes (Climate, Population, Model, Class, etc.).
* **🚀 RESTful API:** A custom-built API handling GET, POST, and DELETE requests for data persistence.

---

## 🛠️ Tech Stack

### Frontend
* ![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB) **React.js**: Functional components & Hooks.
* **Context API**: For global state management (Flux architecture).
* ![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=flat&logo=bootstrap&logoColor=white) **Bootstrap**: For responsive grid layout and cards.

### Backend
* ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) **Python 3**: Server-side logic.
* ![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white) **Flask**: Lightweight framework for the API.
* ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-black?style=flat&logo=python&logoColor=white) **SQLAlchemy**: ORM for handling relationships (One-to-Many, Many-to-Many).
* **PostgreSQL**: Database for production.
---

## 💻 Installation & Local Setup

**1. Clone the repository**
```bash

2. Backend Setup Navigate to the backend folder to set up the Python environment and database.

cd src
pipenv install
pipenv shell

# Run migrations to create the tables in your database
pipenv run migrate
pipenv run upgrade

# Start the server
pipenv run start

3. Frontend Setup Open a new terminal, navigate to the frontend folder.

cd src/front
npm install
npm run start
