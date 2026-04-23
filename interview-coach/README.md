# 🎯 Interview Coach — Claude Skill

A Claude skill that turns your resume into a personalized mock interview experience, with real-time answer feedback and a final performance report.

## Features

- 📄 **Resume parsing** — Upload a PDF/DOCX or paste your resume text
- 🎯 **Tailored questions** — 10–20 questions based on your actual experience + target JD
- 💬 **Real-time feedback** — Score and coaching after every answer
- 📊 **Final report** — Radar chart, score breakdown, strengths/gaps, and readiness verdict
- 🌐 **Bilingual** — Supports Chinese and English

## How to Install

1. Download `interview-coach.skill`
2. In Claude.ai, go to **Settings → Skills**
3. Upload the `.skill` file

## How to Use

Just tell Claude:
> "帮我模拟面试，我要面 [岗位名称]" 

Or in English:
> "I want to practice interviewing for a Senior Frontend Engineer role"

Then upload your resume or paste your resume text. Claude will guide you through the rest.

## What You'll Need

- Your resume (PDF, DOCX, or text)
- Target job title and seniority level
- Job description (optional but recommended for more targeted questions)

## Skill Structure

```
interview-coach/
├── SKILL.md                        # Main skill instructions
├── LICENSE.txt
├── README.md
└── references/
    ├── report-template.md          # Report scoring rubric + HTML template
    └── question-bank.md            # Question patterns by role type
```

## Example Output

After completing a mock interview, you'll receive a report with:
- Overall score (e.g., 78/100)
- Radar chart across 6 competency areas
- Per-question score table
- Top 3 strengths and improvement areas
- Personalized study recommendations
- Interview readiness verdict (🔴 / 🟡 / 🟢 / ⭐)

## License

MIT
