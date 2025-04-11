# BudgeNest

- A safe, smart place for organizing your budget — warm and practical.



expense-tracker/
│
├── app/
│   ├── main.py                  # FastAPI app entry point
│   ├── config.py                # App & DB config
│   ├── db/
│   │   ├── database.py          # DB session & connection (Singleton Pattern)
│   │   └── models.py            # SQLAlchemy ORM models
│   ├── schemas/
│   │   └── expense.py           # Pydantic schemas for validation
│   ├── repository/
│   │   └── expense_repo.py      # Repository Pattern implementation
│   ├── services/
│   │   ├── expense_service.py   # Business logic layer
│   │   └── notifier.py          # Observer Pattern (email alerts, etc.)
│   ├── patterns/
│   │   ├── factory.py           # Factory Pattern for report generation
│   │   ├── strategy.py          # Strategy Pattern for analysis methods
│   │   └── observer.py          # Observer base & subscribers
│   ├── routers/
│   │   └── expense_router.py    # Route definitions
│   └── utils/
│       └── auth.py              # Token-based auth utils
│
├── tests/
│   ├── test_expense.py          # Unit tests
│
├── requirements.txt             # Python dependencies
├── alembic.ini                  # Alembic DB migrations
├── README.md
└── .env                         # Environment variables (e.g., DB URL)
