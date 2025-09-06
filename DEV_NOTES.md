# Dev Notes (For You — NOT the README)

## Quickstart
cd db
sqlite3 app.db < schema.sql
sqlite3 app.db < seed.sql

cd ../api
pip install -r requirements.txt
uvicorn app:app --reload

## Smoke Test
GET /api/v1/health
GET /api/v1/reports/event-popularity?college_id=1
GET /api/v1/reports/attendance-summary/1/101
GET /api/v1/reports/avg-feedback/1/101
GET /api/v1/reports/student-participation?college_id=1&student_id=1
GET /api/v1/reports/top-active-students?college_id=1&limit=3
