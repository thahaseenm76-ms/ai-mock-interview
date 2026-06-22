# ResumeAI — AI Resume Analyzer

> BCA Final Year Project | AI + NLP + Flask

Upload a resume (PDF/TXT), get an instant AI-powered analysis with section scores, ATS score, keyword gaps, and job match percentage.

---

## Tech Stack

| Layer | Tools |
|---|---|
| Backend | Python, Flask |
| AI Analysis | Rule-based NLP + OpenAI GPT (optional) |
| PDF Parsing | PyMuPDF |
| Frontend | HTML, CSS, JavaScript, Chart.js |

---

## Features

- Upload PDF or TXT resume
- Overall score (0–100)
- ATS compatibility score
- Section-by-section scoring (contact, summary, skills, experience, education, projects)
- Radar chart visualization
- Strengths and improvement suggestions
- Keyword analysis (found vs missing)
- Job description match score (paste JD to activate)
- Works offline (no API key needed) — add OpenAI key for deeper AI analysis

---

## Project Structure

```
ai-resume-analyzer/
├── backend/
│   ├── app.py         ← Flask API
│   ├── parser.py      ← PDF/TXT text extractor
│   └── analyzer.py    ← AI analysis engine
├── frontend/
│   ├── index.html     ← Upload page
│   └── dashboard.html ← Results dashboard
├── requirements.txt
└── README.md
```

---

## Setup & Run

```bash
# 1. Install packages
pip install -r requirements.txt

# 2. (Optional) Add OpenAI key for GPT analysis
set OPENAI_API_KEY=your-key-here      # Windows
export OPENAI_API_KEY=your-key-here   # Mac/Linux

# 3. Run server
python backend/app.py

# 4. Open browser
http://localhost:5001
```

---

## To Add OpenAI (Optional Upgrade)

Get a free API key from https://platform.openai.com  
Set it as environment variable before running.  
Without it, the smart rule-based analyzer runs automatically.

---

## Author

**THAHASEEN** — BCA Final Year, Mohan Babu University  
Internship: Doneswari Technologies LLP (AI & ML)  
GitHub: github.com/thahaseen76-ms

