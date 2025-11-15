# ResumeIQ-ats-resume-analyzer-
NLP-based ATS Resume Analyzer using React + FastAPINLP-based ATS Resume Analyzer using React + FastAPI



⭐ ResumeIQ – ATS Resume Analyzer (NLP + AI Project)

A full-stack AI-powered ATS (Applicant Tracking System) that analyzes resumes, extracts key information, and matches candidates with job descriptions using NLP, keyword extraction, and rule-based scoring.
This tool automates resume screening, identifies skills, calculates experience, matches job requirements, and gives an ATS score — just like a real recruitment platform.
🚀 Features
✅ 1. Resume Parsing (NLP-based)
Extract skills, experience, certifications, and education
Supports PDF & text-based resumes
Uses custom Python extraction logic (not basic regex)
✅ 2. Job–Resume Matching
Calculates:
Matched Skills
Missing Skills
Total Experience (in years)
Resume ATS Score
Score is based on keyword matching + experience + skill relevance

✅ 3. Full-Stack Application
Frontend (React + Tailwind)
Clean UI
Resume upload input
Job description input
Light/Dark mode
Backend (FastAPI + Python NLP)
Extracts features
Calculates match score
Processes resume text and job description
Returns structured results as JSON

🧠 Tech Stack
Frontend
React.js
Vite
TailwindCSS
Backend
FastAPI (Python)
Custom NLP logic (skills, experience extractor)
Regex matching
JSON REST APIs
Others.....
Node.js
SQL (SQLite DB for job schemas)
Git & GitHub


🧪 How It Works (Pipeline)
1️⃣ Upload Resume (PDF/Text)
Frontend sends file → backend extracts raw text.

2️⃣ NLP Parsing
Python scripts:
Extract skills (extract.py)
Extract work experience (features.py)
Extract certifications
Extract education

3️⃣ Job Description Analysis
Extract required keywords and compare with resume.

4️⃣ Scoring Engine (rank.py)
Score =
✔ Matched skills
✔ Missing skills
✔ Total experience
✔ Keyword relevance
5️⃣ Final Output
Backend returns JSON → frontend displays it beautifully.


How to Install...

Create venv environment....
python -m venv venv

Activate venv....
venv\Scripts\activate

Install backend requirements....
create a file = pip install -r requirements.txt  (paste list)
list of requirements =
fastapi
uvicorn
python-multipart
pydantic
numpy
pandas
scikit-learn
spacy
nltk
regex
PyPDF2
pdfplumber
joblib
python-dotenv
tqdm
sqlalchemy
sqlite3




📦 Installation & Running Locally
🟦 Backend (FastAPI)
cd Automatic resume score(in this have backend you can confirm)
pip install -r requirements.txt
uvicorn main:app --reload


Server runs at:

http://127.0.0.1:8000

🟩 Frontend (React)
cd ats-frontend
npm install
npm run dev
