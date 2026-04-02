# University Biometric Attendance System

This repository contains the backend project structure for a biometric attendance system using FastAPI and PostgreSQL.

## Project Structure

```
class/
├── app/
│   ├── __init__.py
│   ├── main.py            # Entry point of the FastAPI application
│   ├── models/
│   │   ├── __init__.py
│   │   ├── attendance.py   # Attendance model
│   │   ├── user.py         # User model
│   │   └── biometric.py     # Biometric data model
│   ├── schemas/
│   │   ├── __init__.py
│   │   ├── attendance.py     # Pydantic schemas for attendance
│   │   ├── user.py          # Pydantic schemas for users
│   │   └── biometric.py      # Pydantic schemas for biometric data
│   ├── services/
│   │   ├── __init__.py
│   │   ├── biometric_service.py # Abstracts for biometric services
│   │   └── attendance_service.py # Attendance logic
│   └── database/
│       ├── __init__.py
│       └── db.py           # Database connection and setup
├── requirements.txt          # Project dependencies
└── README.md                 # Project documentation
``` 

## Setup Instructions
1. Clone the repository.
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the application:
   ```
   uvicorn app.main:app --reload
   ```

## Database Models
- **User:** Represents the user of the biometric system.
- **Attendance:** Captures attendance records for each user.
- **Biometric:** Stores biometric data associated with users.

## Services
- **AttendanceService:** Manages attendance-related operations.
- **BiometricService:** Abstracts the operations related to biometric data.
\n
### Author: kinyanjuiwilson10-arch