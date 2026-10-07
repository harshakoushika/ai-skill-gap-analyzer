# 🚀 AI Skill Gap Analyzer

AI Skill Gap Analyzer is a full-stack career-readiness platform that analyzes a user's resume against company and job-role requirements, identifies matched and missing skills, evaluates technical ability using MCQ, Coding, and SQL assessments, calculates job readiness, and generates personalized learning recommendations.

---

## 📌 Project Status

**Version:** v1.0  
**Status:** Development Completed & Deployment Ready

---

## 🔗 Repository

```text
https://github.com/harshakoushika/ai-skill-gap-analyzer
```

Clone:

```bash
git clone https://github.com/harshakoushika/ai-skill-gap-analyzer.git
cd ai-skill-gap-analyzer
```

---

# ✨ Features

- User Registration
- User Login
- JWT Authentication
- Resume Upload
- PDF / DOC / DOCX Parsing
- Resume Skill Extraction
- Company Selection
- Job Role Selection
- Skill Gap Analysis
- Matched Skills
- Missing Skills
- Skill Coverage Percentage
- MCQ Assessments
- Coding Assessments
- SQL Assessments
- Public Test Cases
- Hidden Test Cases
- Coding Execution
- SQL Sandbox
- Assessment Results
- Assessment Progress
- Skill-wise Analytics
- Difficulty-wise Analytics
- Job Readiness Calculation
- Weak Skill Detection
- Personalized Learning Recommendations
- YouTube Learning Resources
- Learning Roadmap
- Learning Progress Tracking
- Dockerized Backend
- MongoDB Atlas
- Render Deployment
- Vercel Deployment

---

# 🛠 Technology Stack

## Frontend

```text
React
Vite
React Router
Axios
Bootstrap
React Bootstrap
Monaco Editor
Chart.js
react-chartjs-2
HTML
CSS
```

## Backend

```text
Node.js
Express.js
MongoDB
Mongoose
JWT
bcryptjs
Multer
pdf-parse
Mammoth
better-sqlite3
```

## Coding Runtime

```text
Python 3
JavaScript / Node.js
Java 17
```

## SQL

```text
SQLite
better-sqlite3
```

## External Services

```text
MongoDB Atlas
YouTube Data API v3
Docker
Render
Vercel
GitHub
```

---

# 🔄 Application Workflow

```text
User Registration / Login
           │
           ▼
      Resume Upload
           │
           ▼
     Skill Extraction
           │
           ▼
 Company + Job Role
           │
           ▼
   Skill Gap Analysis
           │
     ┌─────┼─────┐
     ▼     ▼     ▼
    MCQ  Coding  SQL
     │     │     │
     └─────┼─────┘
           ▼
 Assessment Results
           │
           ▼
       Analytics
           │
           ▼
    Job Readiness
           │
           ▼
      Weak Skills
           │
           ▼
Learning Recommendations
           │
           ▼
 Personalized Roadmap
           │
           ▼
 Learning Progress
```

---

# 📁 Project Structure

```text
ai-skill-gap-analyzer/
│
├── ai-service/
│   ├── main.py
│   └── requirements.txt
│
├── client/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── layouts/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── styles/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   ├── vite.config.js
│   └── vercel.json
│
├── data/
│   ├── assessmentQuestions.json
│   ├── codingQuestions.json
│   ├── companies.json
│   ├── job_requirements.json
│   ├── learningResources.json
│   ├── roles.json
│   ├── skills.json
│   └── sqlQuestions.json
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── uploads/
│   ├── utils/
│   ├── Dockerfile
│   ├── package.json
│   ├── package-lock.json
│   ├── seed.js
│   ├── seedAssessments.js
│   ├── seedCodingQuestions.js
│   ├── seedLearningResources.js
│   ├── seedSQLQuestions.js
│   └── server.js
│
└── README.md
```

---

# ✅ Prerequisites

Install:

```text
Git
Node.js 22+
npm
Docker Desktop
MongoDB Atlas Account
YouTube Data API Key
```

Docker is recommended for the backend because the application uses:

```text
better-sqlite3
Python
Java
Node.js
```

---

# ⚙️ Backend Environment Variables

Create:

```text
server/.env
```

Example:

```env
PORT=5000

MONGODB_URI=mongodb+srv://USERNAME:PASSWORD@CLUSTER.mongodb.net/test

JWT_SECRET=YOUR_SECURE_JWT_SECRET

NODE_ENV=development

YOUTUBE_API_KEY=YOUR_YOUTUBE_API_KEY
YOUTUBE_ENABLED=true
YOUTUBE_CACHE_TTL_HOURS=24
YOUTUBE_MAX_RESULTS=6
YOUTUBE_REGION_CODE=IN
YOUTUBE_RELEVANCE_LANGUAGE=en
YOUTUBE_SAFE_SEARCH=strict

CLIENT_URL=http://localhost:5173
```

For production:

```env
NODE_ENV=production

CLIENT_URL=https://YOUR-VERCEL-PROJECT.vercel.app
```

---

# ⚛️ Frontend Environment Variables

Create:

```text
client/.env.local
```

Local:

```env
VITE_API_URL=http://localhost:5000/api
```

Production:

```env
VITE_API_URL=https://YOUR-RENDER-SERVICE.onrender.com/api
```

In Vercel, add `VITE_API_URL` as a normal **Config** environment variable.

---

# 💻 Local Development

## Clone Project

```bash
git clone https://github.com/harshakoushika/ai-skill-gap-analyzer.git

cd ai-skill-gap-analyzer
```

---

# 🐳 Run Backend Using Docker

Go to backend:

```bash
cd server
```

Build:

```bash
docker build -t ai-skill-gap-server .
```

Force clean rebuild:

```bash
docker build --no-cache -t ai-skill-gap-server .
```

Run backend:

```bash
docker run --name ai-skill-gap-backend --env-file .env -e PORT=10000 -p 5000:10000 ai-skill-gap-server
```

Temporary container:

```bash
docker run --rm --env-file .env -e PORT=10000 -p 5000:10000 ai-skill-gap-server
```

Backend:

```text
http://localhost:5000
```

Health:

```text
http://localhost:5000/api/health
```

---

# ⚛️ Run Frontend

Open another terminal:

```bash
cd client
```

Install:

```bash
npm install
```

Start:

```bash
npm run dev
```

Frontend:

```text
http://localhost:5173
```

---

# 🌐 Local Testing URLs

```text
Frontend
http://localhost:5173

Backend
http://localhost:5000

Backend API
http://localhost:5000/api

Health
http://localhost:5000/api/health
```

---

# 🌍 Production URLs

Replace these URLs after creating the new Render and Vercel deployments.

```text
Frontend
https://YOUR-VERCEL-PROJECT.vercel.app

Backend
https://YOUR-RENDER-SERVICE.onrender.com

API
https://YOUR-RENDER-SERVICE.onrender.com/api

Health
https://YOUR-RENDER-SERVICE.onrender.com/api/health
```

---

# 🔐 Authentication APIs

## Register

```http
POST /api/auth/register
```

Body:

```json
{
    "name": "Test User",
    "email": "test@example.com",
    "password": "TestPassword123"
}
```

---

## Login

```http
POST /api/auth/login
```

Body:

```json
{
    "email": "test@example.com",
    "password": "TestPassword123"
}
```

---

## Current User

```http
GET /api/auth/me
```

Authorization:

```text
Bearer JWT_TOKEN
```

---

# 🏢 Reference Data APIs

```http
GET /api/companies

GET /api/job-roles

GET /api/skills

GET /api/job-requirements
```

---

# 📄 Resume APIs

## Upload Resume

```http
POST /api/resumes/upload
```

Authorization:

```text
Bearer JWT_TOKEN
```

Postman:

```text
Body → form-data
```

Fields:

```text
resume  = File
company = Text
role    = Text
```

---

## Analyze Resume

```http
POST /api/resumes/:resumeId/analyze
```

---

## Skill Gap Analysis

```http
POST /api/resumes/:resumeId/skill-gap
```

---

# 🧪 Assessment APIs

## Create Assessment

```http
POST /api/assessments/create
```

### MCQ

```json
{
    "resumeId": "RESUME_ID",
    "type": "mcq"
}
```

### Coding

```json
{
    "resumeId": "RESUME_ID",
    "type": "coding"
}
```

### SQL

```json
{
    "resumeId": "RESUME_ID",
    "type": "sql"
}
```

Supported types:

```text
mcq
coding
sql
```

---

# ▶️ Start Assessment

```http
POST /api/assessments/:assessmentId/start
```

---

# 💻 Run Coding Question

```http
POST /api/assessments/:assessmentId/run-code
```

Example:

```json
{
    "questionId": "QUESTION_ID",
    "code": "print('Hello World')"
}
```

---

# 🗄 Run SQL Query

```http
POST /api/assessments/:assessmentId/run-sql
```

Body:

```json
{
    "questionId": "QUESTION_ID",
    "query": "SELECT * FROM employees;"
}
```

---

# ✅ Submit Assessment

```http
POST /api/assessments/:assessmentId/submit
```

Example:

```json
{
    "answers": [
        {
            "questionId": "QUESTION_ID",
            "answer": "ANSWER_OR_CODE"
        }
    ]
}
```

---

# 📊 Assessment Result

```http
GET /api/assessments/:assessmentId/result
```

---

# 📈 Assessment Progress

```http
GET /api/assessments/progress/:resumeId
```

---

# 📉 Assessment Analytics

```http
GET /api/assessments/analytics/:resumeId
```

---

# 🎯 Final Job Readiness

```http
GET /api/assessments/final-readiness/:resumeId
```

---

# 📚 Learning Recommendations

```http
GET /api/learning/plan/:resumeId
```

Example:

```text
/api/learning/plan/RESUME_ID?maxSkills=5&resourcesPerSkill=6
```

---

# 📦 Backend Commands

```bash
cd server
```

Install:

```bash
npm install
```

Clean install:

```bash
npm ci
```

Development:

```bash
npm run dev
```

Production:

```bash
npm start
```

---

# 🌱 Seeder Commands

Base data:

```bash
npm run seed
```

MCQ:

```bash
npm run seed:assessments
```

Coding:

```bash
npm run seed:coding
```

SQL:

```bash
npm run seed:sql
```

Learning resources:

```bash
node seedLearningResources.js
```

Recommended order:

```text
npm run seed

npm run seed:assessments

npm run seed:coding

npm run seed:sql

node seedLearningResources.js
```

Do not run seed scripts against production unless you know whether the script modifies or replaces existing data.

---

# ⚛️ Frontend Commands

```bash
cd client
```

Install:

```bash
npm install
```

Run:

```bash
npm run dev
```

Build:

```bash
npm run build
```

Preview:

```bash
npm run preview
```

Lint:

```bash
npm run lint
```

Production build directory:

```text
client/dist
```

---

# 🐳 Docker Commands

Build:

```bash
docker build -t ai-skill-gap-server .
```

Images:

```bash
docker images
```

Running containers:

```bash
docker ps
```

All containers:

```bash
docker ps -a
```

Start backend:

```bash
docker start ai-skill-gap-backend
```

Stop:

```bash
docker stop ai-skill-gap-backend
```

Remove:

```bash
docker rm ai-skill-gap-backend
```

Logs:

```bash
docker logs ai-skill-gap-backend
```

Live logs:

```bash
docker logs -f ai-skill-gap-backend
```

Enter container:

```bash
docker exec -it ai-skill-gap-backend sh
```

Check Node:

```bash
docker exec ai-skill-gap-backend node --version
```

Check Python:

```bash
docker exec ai-skill-gap-backend python3 --version
```

Check Java:

```bash
docker exec ai-skill-gap-backend java -version
```

---

# ☁️ Render Backend Deployment

Go to:

```text
Render Dashboard
→ New
→ Web Service
→ Connect GitHub
```

Select:

```text
harshakoushika/ai-skill-gap-analyzer
```

Configuration:

```text
Branch:
main

Root Directory:
server

Runtime:
Docker

Health Check Path:
/api/health
```

Environment variables:

```text
MONGODB_URI
JWT_SECRET
NODE_ENV=production

YOUTUBE_API_KEY
YOUTUBE_ENABLED=true
YOUTUBE_CACHE_TTL_HOURS=24
YOUTUBE_MAX_RESULTS=6
YOUTUBE_REGION_CODE=IN
YOUTUBE_RELEVANCE_LANGUAGE=en
YOUTUBE_SAFE_SEARCH=strict
```

Do not manually create a `PORT` environment variable.

Render provides it automatically.

After deployment you will receive:

```text
https://YOUR-RENDER-SERVICE.onrender.com
```

Test:

```text
https://YOUR-RENDER-SERVICE.onrender.com/api/health
```

---

# ▲ Vercel Frontend Deployment

Go to:

```text
Vercel
→ Add New
→ Project
→ Import Git Repository
```

Select:

```text
harshakoushika/ai-skill-gap-analyzer
```

Configuration:

```text
Framework Preset:
Vite

Root Directory:
client

Build Command:
npm run build

Output Directory:
dist

Install Command:
npm install
```

Environment variable:

```text
VITE_API_URL
```

Value:

```text
https://YOUR-RENDER-SERVICE.onrender.com/api
```

Then deploy.

---

# 🔗 Connect Frontend and Backend

After Vercel deployment, copy:

```text
https://YOUR-VERCEL-PROJECT.vercel.app
```

Go to:

```text
Render
→ Backend Service
→ Environment
```

Add:

```env
CLIENT_URL=https://YOUR-VERCEL-PROJECT.vercel.app
```

Save and redeploy Render.

Final architecture:

```text
GitHub
   │
   ├───────────────┐
   ▼               ▼
Vercel           Render
Frontend         Backend
   │               │
   └───────┬───────┘
           ▼
     MongoDB Atlas
```

---

# 📮 Postman Configuration

Local:

```text
baseUrl = http://localhost:5000/api
```

Production:

```text
baseUrl = https://YOUR-RENDER-SERVICE.onrender.com/api
```

Useful Postman variables:

```text
baseUrl
token
resumeId
assessmentId
questionId
```

Protected endpoints:

```text
Authorization
Type: Bearer Token
Token: {{token}}
```

---

# 🧪 Recommended API Testing Order

```text
GET  /health

POST /auth/register

POST /auth/login

GET  /auth/me

GET  /companies

GET  /job-roles

POST /resumes/upload

POST /resumes/:resumeId/analyze

POST /resumes/:resumeId/skill-gap

POST /assessments/create

POST /assessments/:assessmentId/start

POST /assessments/:assessmentId/run-code
or
POST /assessments/:assessmentId/run-sql

POST /assessments/:assessmentId/submit

GET /assessments/:assessmentId/result

GET /assessments/progress/:resumeId

GET /assessments/analytics/:resumeId

GET /assessments/final-readiness/:resumeId

GET /learning/plan/:resumeId
```

---

# 🔄 Git Commands

Check status:

```bash
git status
```

Check remotes:

```bash
git remote -v
```

Pull:

```bash
git pull origin main
```

Stage:

```bash
git add .
```

Commit:

```bash
git commit -m "update project"
```

Push:

```bash
git push origin main
```

Repository:

```text
https://github.com/harshakoushika/ai-skill-gap-analyzer.git
```

---

# 🔐 Security

Never commit:

```text
server/.env

client/.env

client/.env.local
```

Never expose:

```text
MongoDB username/password
MongoDB URI
JWT secret
YouTube API key
JWT bearer tokens
User passwords
```

Check whether `.env` is tracked:

```bash
git ls-files server/.env
```

Expected:

```text
No output
```

If it is tracked:

```bash
git rm --cached server/.env

git commit -m "security: remove environment file"

git push origin main
```

Rotate any credentials that have previously been exposed.

---

# 🛠 Troubleshooting

## Port 5000 Already Used

```powershell
netstat -ano | findstr :5000
```

Check Docker:

```bash
docker ps
```

Stop old container:

```bash
docker stop CONTAINER_ID
```

---

## MongoDB URI Undefined

Error:

```text
The uri parameter to openUri() must be a string, got undefined
```

Make sure:

```env
MONGODB_URI=...
```

exists.

Docker must be started with:

```bash
--env-file .env
```

---

## Frontend Calling localhost in Production

Wrong:

```text
http://localhost:5000/api
```

Correct Vercel variable:

```env
VITE_API_URL=https://YOUR-RENDER-SERVICE.onrender.com/api
```

Redeploy Vercel after changing the value.

---

## CORS Error

Add the exact Vercel URL to Render:

```env
CLIENT_URL=https://YOUR-VERCEL-PROJECT.vercel.app
```

Then redeploy Render.

---

# ✅ Production Testing Checklist

```text
[ ] Backend health endpoint works

[ ] Frontend loads

[ ] Register works

[ ] Login works

[ ] Authentication works

[ ] Companies load

[ ] Job roles load

[ ] Resume upload works

[ ] Resume analysis works

[ ] Skill-gap analysis works

[ ] MCQ assessment works

[ ] Coding assessment works

[ ] Run Code works

[ ] SQL assessment works

[ ] Run Query works

[ ] Assessment submission works

[ ] Results load

[ ] Progress loads

[ ] Analytics loads

[ ] Job readiness loads

[ ] Learning recommendations load

[ ] YouTube resources load

[ ] Learning progress works

[ ] Direct route refresh works

[ ] Mobile layout works
```

---

# ⚡ Quick Start

Backend:

```bash
cd server

docker build -t ai-skill-gap-server .

docker run --name ai-skill-gap-backend --env-file .env -e PORT=10000 -p 5000:10000 ai-skill-gap-server
```

Frontend:

```bash
cd client

npm install

npm run dev
```

Open:

```text
http://localhost:5173
```

Health check:

```text
http://localhost:5000/api/health
```

---

# 🎯 Final Architecture

```text
React + Vite
     │
     ▼
   Vercel
     │
     ▼
Node.js + Express
     │
     ▼
Render + Docker
     │
     ▼
MongoDB Atlas
```

---

## 📌 Conclusion

AI Skill Gap Analyzer provides an end-to-end career preparation workflow:

```text
Resume
  ↓
Skill Extraction
  ↓
Skill Gap
  ↓
MCQ / Coding / SQL
  ↓
Assessment Results
  ↓
Analytics
  ↓
Job Readiness
  ↓
Learning Recommendations
  ↓
Learning Progress
```

The application supports local Docker-based development and production deployment using **Vercel + Render + MongoDB Atlas**.
