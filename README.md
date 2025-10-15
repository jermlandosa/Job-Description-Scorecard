# Job Description Scorecard

> Paste a job description → get an instant, transparent score with fix suggestions. Runs 100% locally in your browser.

**Live demo:** <your GitHub Pages URL>

![badge](./assets/scorecard-badge.svg)

---

## Why this exists
Most JDs are walls of text, buzzwordy, and missing the basics (salary band, EEO, apply path). This tool gives:
- A clear **0–100 score** with 7 sub-scores
- **Red flags** (salary, location, EEO, application steps, unrealistic years, etc.)
- A **rule-based rewrite** you can copy back into your ATS

No servers, no tracking, no uploads—everything happens client-side.

---

## Features
- **Scoring (100 pts)**
  - Clarity (25) · Structure (15) · Requirements realism (15) · Inclusivity (15)
  - Transparency (15) · Readability (10) · Jargon/Buzzword load (5)
- **Red flags & concrete fixes** (e.g., "No salary/range found—add base band $X–$Y + bonus/equity")
- **Auto-Rewrite (rule-based)**: splits long sentences, replaces buzzwords, enforces headings, inserts transparency placeholders
- **Local-only**: paste stays on your device; zero network calls
- **Fast**: single-file static app; perfect for GitHub Pages

---

## Quick Start
1. **Clone** this repo or download `index.html`.
2. **Open** `index.html` in a browser (Chrome, Edge, Safari).
3. Paste any JD → **Analyze**.

> Tip: Use **Load sample** to see how scoring works.

---

## Deploy to GitHub Pages
1. Create a repo (e.g. `jd-scorecard`).
2. Put `index.html` at the root.
3. In **Settings → Pages**, choose **Deploy from Branch**, folder **/root**.
4. Your site will be live at `https://<username>.github.io/jd-scorecard/`.

---

## Scoring Details
- **Clarity (25):** outcomes, responsibilities, reporting line, 90-day success metrics, apply path
- **Structure (15):** standard headings; bullets for duties/requirements; logical order
- **Requirements realism (15):** junior vs years mismatch, excessive tech/tool sprawl
- **Inclusivity (15):** flags gendered/age-coded terms, degree gatekeeping without "or equivalent"
- **Transparency (15):** salary/range, location/remote/hybrid, benefits, EEO, visa note
- **Readability (10):** Flesch score, average sentence length, passive-voice approximations
- **Jargon load (5):** buzzword counter ("rockstar", "world-class", etc.)

The rubric is intentionally opinionated but practical. Adjust weights in the JS if your org prefers different emphasis.

---

## Privacy
This is a static, client-side app. Your pasted text does **not** leave your device. No analytics.

---

## Roadmap (nice-to-haves)
- Export report as PDF
- Custom org rubric (weights & banned phrases)
- ATS link check (Greenhouse/Lever/Workday) and broken-link detection
- Inline edit mode with side-by-side diff

---

## Contributing
PRs welcome. Please:
- Keep it **fast** (no build step; no deps)
- Keep it **local-only** (no API calls)
- Prefer **plain JS** and readable functions

---

## License
MIT © Jeremy Landers
