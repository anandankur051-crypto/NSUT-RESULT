Student Rank Management System (FastAPI)
A FastAPI backend that allows students to check overall and branch-wise ranks using their roll number.
Rank data is stored in CSV files and served through REST APIs.
Features-
1) Student rank lookup by roll number
2) Branch-wise rank list retrieval
3) FastAPI with Swagger UI
4) CSV-based data (no database)
   

project structure-
rank_backend/
├── app.py
├── final_rank_list.csv
└── branch_wise_ranks/
    ├── MAC_rank_list.csv
    ├── Mechanical_rank_list.csv
    └── ...
API Endpoints-
1) Get student rank
2) GET /user/rank/{roll_no}
3) Get branch rank list
4)GET /branch/{branch_name}
to Run Locally-
Bash
pip install fastapi uvicorn pandas
uvicorn app:app --reload
Open: http://127.0.0.1:8000/docs
Author
Ankur Anand
