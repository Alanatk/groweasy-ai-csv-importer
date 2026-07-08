# GrowEasy AI-Powered CSV Import Pipeline

## Overview

This project is an AI-powered CRM CSV Import Pipeline built for the GrowEasy Software Developer Internship Assignment.

The application uploads a CSV file, validates records using Google Gemini AI, converts them into a standardized CRM format, and displays the final imported records.

---

## Features

- CSV Upload
- AI-powered field extraction using Google Gemini
- CRM field validation
- Skip invalid records
- Preview imported records
- Import summary
- Responsive UI
- REST API backend

---

## Tech Stack

### Frontend

- React
- Next.js
- TypeScript

### Backend

- Node.js
- Express.js
- TypeScript
- Multer
- CSV Parser
- Axios

### AI

- Google Gemini API

---

## Folder Structure

```
groweasy-assignment/
│
├── frontend/
├── backend/
├── README.md
└── .gitignore
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/groweasy-assignment.git
```

---

### Backend

```bash
cd backend
npm install
```

Create `.env`

```env
GEMINI_API_KEY=YOUR_API_KEY
PORT=5000
CLIENT_URL=http://localhost:3000
GEMINI_MODEL=gemini-2.5-flash
BATCH_SIZE=10
```

Run

```bash
npm run dev
```

---

### Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## API

### Health Check

```
GET /health
```

### Upload CSV

```
POST /upload
```

### Process Import

```
POST /process
```

---

## Sample Workflow

1. Upload CSV
2. Preview records
3. Click Confirm Import
4. Gemini validates records
5. View CRM table
6. Download/Review results

---

## AI Validation Rules

- Skip records without Email and Mobile Number
- Validate CRM Status
- Validate Data Source
- Normalize CRM fields
- Return structured JSON

---

## Author

Alan Thomas

