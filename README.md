💼 Pro Job Portal Backend (Day 7: RBAC Edition)

This is a production-ready Job Portal Backend built with FastAPI. It features secure authentication, data validation, and Role-Based Access Control (RBAC).

🚀 Key Features (Day 7 Update)

Role-Based Access Control (RBAC): Distinction between Admin and Candidate roles.

Admin Powers: Exclusive endpoints for user management and global job moderation.

JWT Authentication: Secure user sessions using JSON Web Tokens.

Password Hashing: Industry-standard security using bcrypt.

Relational Database: Complex relationships between Users and Jobs using SQLAlchemy ORM.

🛠️ Tech Stack

Backend: FastAPI (Python)

Database: SQLite (SQLAlchemy ORM)

Security: Passlib (Bcrypt), Python-JOSE (JWT)

Documentation: Interactive Swagger UI

📂 Project Structure

app/
├── main.py          # Entry point & RBAC Routes
├── database.py      # DB Connection Logic
├── models.py        # SQLAlchemy Tables (Role field added)
├── schemas.py       # Pydantic Schemas (Role included)
└── auth_utils.py    # JWT & admin_required Logic


⚙️ Setup & Run

Install dependencies:
pip install fastapi uvicorn sqlalchemy passlib[bcrypt] python-jose[cryptography]

Run Server:
cd app
python -m uvicorn main:app --reload

Built by Omkar Kandekar during the 21-Day Job Mastery Challenge. 🚀
