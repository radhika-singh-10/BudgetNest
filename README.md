# BudgeNest

- A safe, smart place for organizing your budget — warm and practical.


- A cloud-ready, multi-tenant **expense tracking application** built with **FastAPI**, **PostgreSQL**, and **SQLAlchemy**, following clean software architecture principles and utilizing classic **design patterns** like Singleton, Factory, Strategy, Observer, and Repository.

---

## 🚀 Features

- 🔐 **Multi-tenant support** for isolated team data
- 🧾 Add, view, and manage categorized expenses
- 📊 Generate custom reports (monthly, by category, etc.)
- 📬 Notifications on budget threshold breaches (Observer Pattern)
- 🧱 Clean, maintainable architecture with design patterns
- 🐘 SQL database support (PostgreSQL)
- ☁️ Cloud deployment-ready

---

budget-nest/
  
── app/

    ── main.py                  # FastAPI app entry point

    ── config.py                # App & DB config

    ── db/

       ── database.py          # DB session & connection (Singleton Pattern)

       ── models.py            # SQLAlchemy ORM models

    ── schemas/
       ── expense.py           # Pydantic schemas for validation
    ── repository/
       ── expense_repo.py      # Repository Pattern implementation
    ── services/
      ── expense_service.py   # Business logic layer
      ── notifier.py          # Observer Pattern (email alerts, etc.)
    ── patterns/
      ── factory.py           # Factory Pattern for report generation
      ── strategy.py          # Strategy Pattern for analysis methods
      ── observer.py          # Observer base & subscribers
    ── routers/
      ── expense_router.py    # Route definitions
    ── utils/
     ── auth.py              # Token-based auth utils

    ── tests/
     ── test_expense.py          # Unit tests

── requirements.txt             

── alembic.ini                 

── README.md

── .env    



🔧 Tech Stack:
Backend: Python (Flask / FastAPI)

Database: PostgreSQL (SQL)

ORM: SQLAlchemy

Hosting: AWS RDS + EC2 / Render / Railway / Supabase

Design Patterns:

Factory Pattern: For creating different types of users or reports

Repository Pattern: Abstract SQL operations

Singleton Pattern: DB connection management

Strategy Pattern: Different algorithms for budget analysis

Observer Pattern: Notify users when budget thresholds are crossed

🧱 Core Features:
✅ User registration/login (multi-tenant support)

✅ Add/view/edit expenses

✅ Expense categories

✅ Budget tracking

✅ Email alerts on threshold breach

✅ Team-level dashboards (for each tenant)

💡 Bonus Add-Ons:
Generate PDF reports using Factory pattern

Use REST API endpoints with FastAPI

Deploy to cloud and expose public API


