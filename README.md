# cv-reviewer-skills

A collection of agent skills focused on helping you craft a strong CV and land more interviews. Each skill is a standalone `SKILL.md` file — install it once, then just talk to Claude naturally.

---

## 📦 Skills

| Skill | Description |
|-------|-------------|
| [cv-reviewer](./skills/cv-reviewer/SKILL.md) | Reviews your CV against 60+ best practices with severity-tiered feedback |

*More coming soon — cover letter writer, job description matcher, LinkedIn bio optimizer.*

---

## 🚀 Installation

### Claude.ai
1. Go to [claude.ai](https://claude.ai) → **Settings** → **Skills**
2. Click **Import Skill** and select the `SKILL.md` from the skill folder you want
3. Done — Claude will automatically use the skill when relevant

### Claude Code
```bash
git clone https://github.com/primordian-studio/cv-reviewer-skills
```
Point Claude Code at the `skills/` directory.

---

## 📄 cv-reviewer skill

Reviews your CV against 60+ best practices and returns structured, severity-tiered feedback across every section. Adapts automatically to your experience level — student, mid-level professional, or senior engineer.

Once installed, paste or upload your CV and ask something like:

> "Can you review my CV?"
> "What's wrong with my resume?"
> "Is my CV good enough to apply?"

### Severity Levels

| Icon | Meaning |
|------|---------|
| ✅ | Pass — looks good |
| ⚠️ | Warning — minor issue, worth fixing |
| 🟥 | Critical — must fix before applying |
| ℹ️ | Unverifiable — needs manual check (layout, fonts, spacing) |

### Sample Output

```
🎯 Detected Level: Mid-level Professional (4 years experience)

📐 Formatting & Layout
✅ Single-column layout — clean, ATS-friendly structure
✅ No icons or graphics
ℹ️ Font type and size — cannot verify from plain text, ensure you're using Calibri/Arial at 10.5pt+
⚠️ Resume appears to be 2 pages — consider trimming to 1 page for a mid-level candidate

📅 Dates
✅ Uses "Present" correctly
⚠️ Date ranges use hyphens (Jun 2022 - Present) — use en dashes with spaces: Jun 2022 – Present
✅ Full years used, no digit-only formats

💼 Work Experience
✅ Section correctly named "Experience"
🟥 Bullets describe duties, not accomplishments — rewrite using STAR/XYZ format
   Before: "Responsible for maintaining the company database"
   After:  "Reduced query response time by 40% by optimizing indexes across 12 core tables"
⚠️ 3 bullets end with periods — remove them

...

🟥 Critical Issues
1. Bullets describe duties not accomplishments — highest impact change you can make
2. No quantified results anywhere — add numbers, percentages, or scale to your bullets

⚠️ Top Warnings
1. Date ranges use hyphens instead of en dashes
2. "Professional Experience" → rename to "Experience"

⚡ Quick Wins
- Remove periods from all bullet points
- Fix date ranges: hyphen (-) → en dash (–)
```

### Checklist Coverage

| Category | What's Checked |
|----------|----------------|
| 📐 Formatting & Layout | Column layout, fonts, colors, spacing, page length |
| 📅 Dates | Format, alignment, en dashes, abbreviations |
| 📋 Section Order & Naming | Correct order for experience level, English titles |
| 📬 Contact Information | Email provider, URLs, phone, bias-causing details |
| 💼 Work Experience | Bullet style, accomplishments vs duties, pronouns |
| 🔫 Bullet Point Quality | Action verbs, STAR/XYZ/CAR structure, metrics |
| 🎓 Education | GPA rules, dates, coursework, awards |
| 🛠️ Skills | Naming, formatting, soft skills, categories |
| 📁 Projects | Titles, links, bullet style, ordering |

### Best Practices Source

Checklist is based on the [r/EngineeringResumes wiki](https://www.reddit.com/r/EngineeringResumes/wiki/index/) — one of the most thorough and battle-tested resume guides available. Originally written for engineering roles, the principles apply broadly across industries.

---

## 🤝 Contributing

Found a missing rule, disagree with a severity level, or want to propose a new skill? Open an issue with:
- What you'd like to add or change
- Why it matters
- A source or reference if you have one

PRs are welcome.

---

## 📄 License

MIT — free to use, share, and modify.
