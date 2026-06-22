# 🤖 AI HR Resume Screening Agent

An AI-powered automation that screens job applications, scores candidates against job requirements using Google Gemini AI, and automatically shortlists qualified candidates — reducing manual resume screening time from hours to minutes.

## 📋 Problem Statement

HR teams receive hundreds of resumes per job posting and spend 6-8 hours manually screening candidates. This agent automates that process end-to-end.

## ⚙️ How It Works

1. **Candidate applies** via a simple job application form (name, email, phone, role, resume)
2. **n8n workflow triggers** automatically on form submission
3. **PDF resume is extracted** to plain text
4. **Google Gemini AI** analyzes the resume against the job description and assigns a score (1-10) with detailed reasoning
5. **Conditional logic** filters candidates — only those scoring 7+ proceed
6. **Google Sheets** logs every candidate result for record-keeping
7. **Gmail** automatically notifies HR with shortlisted candidate details

## 🛠️ Tech Stack

- **n8n** — workflow automation (no-code)
- **Google Gemini API** — AI resume analysis and scoring
- **Google Sheets** — candidate data logging
- **Gmail API** — automated HR notifications

## 📊 Tested Results

| Candidate Profile | Score | Outcome |
|---|---|---|
| Strong (relevant experience + skills) | 10/10 | ✅ Shortlisted |
| Average (partial skill match) | 4/10 | ❌ Rejected with reasoning |

The AI provides detailed, honest reasoning for every decision — not just a score, but *why* (matched skills, missing skills, and a recommendation).

## 📁 Repository Contents

- `workflow.json` — Full exported n8n workflow (importable)
- `sample_resumes/` — Test resumes used for demo (strong/average candidates)
- `screenshots/` — Workflow diagram and execution outputs

## 🎯 Business Impact

- Reduces screening time from **8 hours to under 2 minutes** per batch
- Consistent, bias-free initial screening
- Scales to hundreds of applications without additional HR effort

## 👤 Author

**Bolagani Mahesh**
[LinkedIn](https://linkedin.com/in/mahesh-bolagani-39ab31356) | maheshbolagani225@gmail.com

---
*Built as a self-driven project to demonstrate practical AI automation and agentic workflow skills.*
