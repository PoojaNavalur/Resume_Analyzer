# NextHire — AI Resume & LinkedIn Analyzer

A full‑stack project (React + Tailwind CSS on the frontend, Node.js + Express on the backend) that:
- Uploads a resume (PDF/DOCX) or accepts pasted text / LinkedIn URL*
- Generates a **Career Fit Score** for a chosen role
- Provides **ATS optimization tips**
- Suggests **AI‑powered rewrites** of resume highlights

> *Direct scraping of LinkedIn is not implemented (and is against their ToS). Enter profile text or a public export.

## Tech
- Frontend: React (Vite) + Tailwind CSS
- Backend: Node.js, Express, Multer (file uploads), pdf-parse & mammoth (basic resume text extraction)
- AI: OpenAI API (replace `OPENAI_API_KEY` in `.env`)

## Quick Start
### 1) Backend
```bash
cd backend
cp .env.sample .env   # add your OPENAI_API_KEY
npm install
npm run dev           # http://localhost:5000
```

### 2) Frontend
```bash
cd frontend
npm install
npm run dev           # http://localhost:5173
```

### 3) Use
- Upload a resume or paste text / LinkedIn content.
- Enter target role (e.g., “Frontend Developer”).
- Click **Analyze**. See score, ATS tips, and rewrite suggestions.

## Notes
- This starter favors clarity & beauty. Polish/extend as you like.
- If `pdf-parse` fails on your platform, consider using a hosted parser API.
- Do not share your API key publicly.
