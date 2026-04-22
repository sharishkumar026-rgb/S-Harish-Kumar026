Hospital API (FastAPI)
Objective
This project is a simple REST API built using FastAPI 
to manage Doctors and Patients with validation and clean code practices.

Tech Stack
Python 3.9+
FastAPI
Pydantic
Uvicorn

 Setup Instructions
1. Install dependencies
   pip install -r requirements.txt
2. Run the server
   uvicorn main:app --reload
3. Open API docs

Go to:
http://127.0.0.1:8000/docs

Features
Doctor APIs
POST /doctors → Create doctor
GET /doctors → List doctors
GET /doctors/{id} → Get doctor by ID

Patient APIs
POST /patients → Create patient
GET /patients → List patients

 Validation
Email validated using Pydantic
Age must be greater than 0
Proper error handling using HTTPException

 Storage
In-memory storage (Python lists)
