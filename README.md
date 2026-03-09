
# ✈️ Flight Data CLI

![Python](https://img.shields.io/badge/Python-3.11%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Bootcamp](https://img.shields.io/badge/Masterschool-Bootcamp-orange)
![Platform](https://img.shields.io/badge/Platform-Terminal-lightgrey)

> A small **flight data query CLI** built with **Python + SQLAlchemy**.
> The application allows users to search flight data from an SQLite database
> and optionally export the results to **CSV files**.

---

# 📌 Overview

This project demonstrates how to:

- Connect Python to an SQLite database
- Implement a **Data Access Layer (DAL)**
- Execute SQL queries using **SQLAlchemy**
- Retrieve and display database results in a CLI program
- Validate user input
- Export query results to CSV files

The project architecture separates **database access** from **application logic**.

    User Input (CLI Menu)
          │
          ▼
        main.py
          │
          ▼
     flights_data.py (DAL)
          │
          ▼
    SQLAlchemy Engine
          │
          ▼
    SQLite Database (flights.sqlite3)
          │
          ▼
      Results / CSV Export

---

# 🖥️ Demo Flow

1. User starts the program
2. A menu is displayed
3. User selects a query option
4. Results are printed in the terminal
5. User can optionally export the results to CSV

Example:

```bash
python main.py
```

```
Menu:
1. Show flight by ID
2. Show flights by date
3. Delayed flights by airline
4. Delayed flights by origin airport
5. Exit
```

---

# ✨ Core Features

- SQLite database integration
- SQLAlchemy engine
- Data Access Layer (DAL)
- Flight search by ID
- Flight search by date
- Delayed flights by airline
- Delayed flights by airport
- CSV export functionality
- CLI menu navigation

---

# 📂 Project Structure

```
flight-data-cli/
│
├── main.py                # CLI application
├── flights_data.py        # Data Access Layer (SQL queries)
│
├── data/
│   └── flights.sqlite3    # SQLite database
│
├── requirements.txt
└── README.md
```

---

# 🚀 Installation & Usage

## Requirements

- Python 3.10+

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Run the Program

```bash
python main.py
```

---

# 📊 CSV Export

After displaying results, the program asks:

```
Would you like to export this data to a CSV file? (y/n)
```

If the user enters **y**, the program asks for a filename and exports the data.

Example:

```
Enter file name: delayed_flights
Data exported to delayed_flights.csv
```

CSV files are saved in the current project directory.

---

# 🧠 Technical Concepts Applied

| Concept | Implementation |
|-------|-------|
| Database Connection | SQLAlchemy |
| SQL Queries | SQLite |
| Data Access Layer | flights_data.py |
| CLI Interaction | input() |
| Data Export | csv module |
| Result Handling | SQLAlchemy Row objects |

---

# 🎓 Learning Objectives

This exercise practices:

- Working with SQLAlchemy
- Structuring Python projects
- Separating logic and data access
- Building CLI tools
- Exporting structured data to CSV
- Validating user input

---

# 📈 Portfolio Upgrade Ideas

Possible improvements:

- Add **search by destination airport**
- Add **search by airline code**
- Implement **pagination for results**
- Add **unit tests**
- Implement **logging**
- Convert project into a **Flask or FastAPI web app**
- Add **Docker support**

---

# 🇩🇪 Kurzbeschreibung

Ein Python‑CLI‑Projekt zur Analyse von Flugdaten aus einer SQLite‑Datenbank.

Die Anwendung nutzt **SQLAlchemy**, eine **Data Access Layer Struktur**
und ermöglicht das Exportieren von Abfrageergebnissen als **CSV-Datei**.

---

# 📄 License

MIT License

---

# 👤 Author

Hakan Yildirim  
Python Software Developer (AI Track)  
Masterschool Bootcamp

GitHub: https://github.com/haki36  
LinkedIn: https://linkedin.com/in/hakan-yildirim-tech
