# cv-reviewer-skills

<p align="center">
  <img alt="GitHub Release" src="https://img.shields.io/github/v/release/primordian-studio/cv-reviewer-skills?style=for-the-badge">
  <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/primordian-studio/cv-reviewer-skills/release-please.yml?style=for-the-badge">
  <img alt="GitHub License" src="https://img.shields.io/github/license/primordian-studio/cv-reviewer-skills?style=for-the-badge">
</p>

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

### ChatGPT and others

Just include the SKILL.md along with your CV and tell them to review your CV follow the SKILL specification.

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
🎯 Detected Level: Mid-level Professional (3 years experience)

...

📅 Dates
ℹ️ Unverifiable — Dates are right-aligned to the margin: Cannot verify layout from plain text.
⚠️ Warning — Digit-only date format: Dates like 01/2025, 5/2024, 9/2024, 12/2022, 06/2023, 04/2022, 09/2022, 12/2025, 03/2022 are ambiguous. Use "Jan 2025", "May 2024", etc. instead.
✅ Pass — Full years used: All dates include 4-digit years.
✅ Pass — No specific days included.
✅ Pass — No season/semester dates.
⚠️ Warning — Hyphens used instead of en dashes: Use " – " (en dash with spaces) for date ranges, not "–" or "-". E.g., Jan 2025 – Present.

💼 Work Experience
🟥 Critical — Bullets describe duties, not accomplishments: Almost every bullet describes what you did, not what you achieved. For example, "Designed and developed websites" tells the reader nothing about impact, scale, or result.
🟥 Critical — No quantified results anywhere: Outside of the dotfiles project (142+ GitHub stars), there are no metrics anywhere in your work experience. How many websites did you build? How much did performance improve? How large was the codebase? What was the traffic? Metrics are essential for mid-level candidates.
🟥 Critical — Bullets don't follow STAR/XYZ/CAR structure: None of your work experience bullets have a result or outcome. Every bullet is just an action with no consequence. Here's a before/after example:

> ❌ Before: "Collaborated with the backend team to build new features and fix bugs for Sendo's internal system"
> ✅ After: "Collaborated with backend team to build 3 new features and resolve 20+ bugs for Sendo's internal system, reducing reported issues by 30% over a 4-month internship"

✅ Pass — Digits used instead of spelled-out numbers (142+ stars).
⚠️ Warning — Weak verbs present: Phrases like "participated in supporting" and "assisted with managing" are weak constructions. Replace with strong action verbs like "Optimized", "Maintained", "Audited".
⚠️ Warning — Freelance role has only 1 bullet: "Designed and developed websites" is a single vague bullet with no detail. Add 2–3 bullets with specifics about what you built, for whom, and the results — e.g., how many clients, what stack, any measurable outcomes.
ℹ️ Unverifiable — Bullets are 1–2 lines long: Cannot verify layout from plain text.

🛠️ Skills
✅ Pass — No obvious soft skills listed in the Skills section.
⚠️ Warning — "GitHub" listed instead of "Git": In your DevOps section you list "Git" correctly, but also include platforms. "GitHub" as a platform is fine to list in tools, but make sure "Git" is the primary skill listed, not "GitHub."
⚠️ Warning — Skills section is very long: Your skills section spans many lines across Frontend, Backend, DevOps, UX/UI. For a 1-page CV this is too much. Cut it to 3 lines or fewer, focusing only on your strongest/most relevant skills.
⚠️ Warning — Skills separated by commas in some places but formatting is inconsistent across subsections. Standardize to comma-separated lists only.
✅ Pass — No proficiency descriptors like "Expert in" or "Proficient in."
⚠️ Warning — "JavaScript/TypeScript" should be separated: List as "JavaScript, TypeScript" not "JavaScript/TypeScript".

...

🟥 Critical Issues
1. Bullets describe duties not accomplishments — Rewrite using STAR/XYZ structure. Highest impact change you can make
2. No quantified results anywhere — add numbers, percentages, or scale to your bullets
3. Section order wrong for mid-level — Reorder to: Work Experience → Projects → Skills → Education

⚠️ Top Warnings
- Date ranges use hyphens instead of en dashes
- "Professional Experience" → rename to "Experience"
- Date format is digit-only (01/2025) — switch to "Jan 2025" style
- Phone number has country code — remove +84
- Summary section is long — either remove or condense to 2 lines
- Skills section is too long for a 1-page CV — trim significantly
- Freelance role has only 1 vague bullet — expand with specifics

⚡ Quick Wins
- Remove periods from all bullet points
- Fix date ranges: hyphen (-) → en dash (–)
- Change all dates from 01/2025 → Jan 2025
- Remove the 3 template placeholder projects
- Remove country code from phone number (+8488 → 088 334 4456 or just omit)
Change "JavaScript/TypeScript" → "JavaScript, TypeScript"
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
