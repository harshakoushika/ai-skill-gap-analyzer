# 🚀 AI Skill Gap Analyzer

### AI-Powered Full-Stack Career Readiness Platform

AI Skill Gap Analyzer is a full-stack career-readiness platform that analyzes a user's resume against company and job-role requirements, identifies matched and missing skills, evaluates technical ability through **MCQ, Coding, and SQL assessments**, calculates **job readiness**, and generates **personalized learning recommendations**.

<p align="center">
  <a href="https://ai-skill-gap-analyzer-gamma.vercel.app/login">
    <strong>🌐 Live Demo</strong>
  </a>
  &nbsp;&nbsp;•&nbsp;&nbsp;
  <a href="https://github.com/harshakoushika/ai-skill-gap-analyzer">
    <strong>📦 GitHub Repository</strong>
  </a>
</p>

---

## ✨ Overview

Preparing for a technical role often involves understanding what skills a job requires, identifying gaps in a candidate's current skill set, testing those skills, and knowing what to learn next.

**AI Skill Gap Analyzer brings these steps together into a single platform.**

The application follows an end-to-end career preparation workflow:

```text
Resume
   ↓
Skill Extraction
   ↓
Company + Job Role Selection
   ↓
Skill Gap Analysis
   ↓
MCQ / Coding / SQL Assessments
   ↓
Assessment Results
   ↓
Analytics
   ↓
Job Readiness Score
   ↓
Weak Skill Detection
   ↓
Personalized Learning Recommendations
   ↓
Learning Roadmap
   ↓
Learning Progress
```

---

## 🎯 Key Features

### 🔐 Authentication

- User registration
- User login
- JWT-based authentication
- Protected API routes
- Password hashing using bcrypt

### 📄 Resume Analysis

- Resume upload
- Support for PDF, DOC, and DOCX files
- Resume parsing
- Skill extraction
- Company selection
- Job-role selection
- Job requirement comparison

### 🎯 Skill Gap Analysis

- Identify matched skills
- Identify missing skills
- Calculate skill coverage percentage
- Compare extracted resume skills against target job requirements

### 🧪 Technical Assessments

The platform evaluates technical ability through three assessment types:

- **MCQ Assessments**
- **Coding Assessments**
- **SQL Assessments**

Assessment capabilities include:

- Public test cases
- Hidden test cases
- Automated coding execution
- SQL query execution
- Assessment submission
- Assessment results
- Progress tracking

### 💻 Coding Assessment Engine

Supports code execution for:

- Python 3
- JavaScript / Node.js
- Java 17

The coding environment evaluates submitted solutions against test cases and supports both public and hidden test cases.

### 🗄️ SQL Assessment Engine

The platform includes a SQL sandbox powered by:

- SQLite
- better-sqlite3

Users can execute SQL queries against assessment data and receive evaluation results.

### 📊 Analytics & Job Readiness

The platform provides:

- Assessment progress
- Skill-wise analytics
- Difficulty-wise analytics
- Assessment results
- Weak skill detection
- Final job-readiness calculation

### 📚 Personalized Learning

Based on identified skill gaps and assessment performance, the platform provides:

- Personalized learning recommendations
- Skill-specific learning resources
- YouTube learning resources
- Personalized learning roadmap
- Learning progress tracking

### ☁️ Deployment

The application supports:

- Dockerized backend
- MongoDB Atlas
- Render backend deployment
- Vercel frontend deployment

---

## 🛠️ Technology Stack

### Frontend

| Technology | Purpose |
|---|---|
| React | UI development |
| Vite | Frontend build tool |
| React Router | Client-side routing |
| Axios | API communication |
| Bootstrap | UI styling |
| React Bootstrap | React-based UI components |
| Monaco Editor | Code editor |
| Chart.js | Data visualization |
| react-chartjs-2 | React Chart.js integration |
| HTML5 | Structure |
| CSS3 | Styling |

### Backend

| Technology | Purpose |
|---|---|
| Node.js | Backend runtime |
| Express.js | REST API framework |
| MongoDB | Database |
| Mongoose | MongoDB ODM |
| JWT | Authentication |
| bcryptjs | Password hashing |
| Multer | File uploads |
| pdf-parse | PDF parsing |
| Mammoth | DOC/DOCX processing |
| better-sqlite3 | SQL execution |

### Coding Runtime

```text
Python 3
JavaScript / Node.js
Java 17
```

### SQL

```text
SQLite
better-sqlite3
```

### External Services & Deployment

```text
MongoDB Atlas
YouTube Data API v3
Docker
Render
Vercel
GitHub
```

---

## 🔄 Application Workflow

```text
                    ┌─────────────────────┐
                    │   User Registration │
                    │      / Login        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Resume Upload    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Skill Extraction  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Company + Job Role  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │  Skill Gap Analysis │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┼─────────────┐
                 ▼             ▼             ▼
              ┌─────┐      ┌───────┐      ┌─────┐
              │ MCQ │      │Coding │      │ SQL │
              └──┬──┘      └───┬───┘      └──┬──┘
                 │             │             │
                 └─────────────┼─────────────┘
                               ▼
                    ┌─────────────────────┐
                    │ Assessment Results  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     Analytics       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Job Readiness     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Weak Skills      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Learning Recommend. │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Personalized Roadmap│
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Learning Progress   │
                    └─────────────────────┘
```

---

## 🏗️ System Architecture

```text
                    ┌───────────────────┐
                    │    React + Vite   │
                    │     Frontend      │
                    └─────────┬─────────┘
                              │
                         REST APIs
                              │
                              ▼
                    ┌───────────────────┐
                    │  Node.js +        │
                    │    Express.js     │
                    │     Backend      │
                    └───────┬───┬───────┘
                            │   │
              ┌─────────────┘   └─────────────┐
              ▼                               ▼
     ┌─────────────────┐             ┌─────────────────┐
     │   MongoDB Atlas │             │   AI Service    │
     │   Application   │             │ Resume/Skills   │
     │      Data       │             │    Analysis     │
     └─────────────────┘             └─────────────────┘
              │
              ▼
     ┌──────────────────────────────────────────────┐
     │              Assessment Engines              │
     │                                              │
     │      MCQ       Coding        SQL             │
     │       │           │           │              │
     │       └───────────┼───────────┘              │
     │                   ▼                          │
     │              Evaluation                     │
     └───────────────────┬──────────────────────────┘
                         │
                         ▼
                ┌─────────────────┐
                │    Analytics    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Job Readiness   │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
