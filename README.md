# Resume Artifacts — Drew Williams (ATS-Optimized)

This repository contains the most recent resume work tailored for Deloitte Technology, Strategy & Transformation (TS&T) plus ten additional high-fit Canadian roles. Each variant is single-page, ATS-friendly, and printable with consistent CSS.

## Contents

- **`resume/` — HTML deliverables**
  - `drew-williams-resume.html` — Polished base resume
  - `drew-williams-resume-ats.html` — Baseline ATS single-column version
  - `drew-williams-resume-ats-single.html` — Single-page condensed
  - `drew-williams-resume-ats-printclean.html` — Print-clean (no link previews on print)
  - `drew-williams-resume-ats-single-tight.html` — Tight layout
  - `drew-williams-resume-ats-single-tight-v2.html` — Tighter layout
  - `drew-williams-resume-ats-single-tight-v3.html` — Very tight layout
  - `drew-williams-resume-ats-single-tight-v4.html` — Maximum compression (recommended for single-page PDF)
  - `drew-williams-resume-ats-single-tight-v4-ascii.html` — ASCII-safe variant (plain hyphens/quotes, ideal for strict parsers)
  - `drew-williams-resume-westjet-fpa.html` — WestJet FP&A Analyst (Calgary)
  - `drew-williams-resume-transalta-corpdev.html` — TransAlta Corporate Development (Calgary)
  - `drew-williams-resume-cnrl-corpdev.html` — CNRL Corporate Development (Calgary)
  - `drew-williams-resume-cenovus-corpdev.html` — Cenovus Corporate Development (Calgary)
  - `drew-williams-resume-aimco-performance.html` — AIMCo Performance Measurement (Edmonton)
  - `drew-williams-resume-psp-manager-selection.html` — PSP External Manager Selection (Montréal)
  - `drew-williams-resume-psp-portfolio.html` — PSP Portfolio Management (Montréal)
  - `drew-williams-resume-brookfield-client-group.html` — Brookfield Global Client Group (Toronto)
  - `drew-williams-resume-palantir-deployment.html` — Palantir Deployment Strategist (Ottawa)
  - `drew-williams-resume-deloitte-ts-t.html` — Deloitte Technology Strategy & Transformation (Toronto)
- **`resume/` — Cover letters & fit memos (HTML)**
  - `drew-williams-cover-letter-<role>.html` — Tailored cover letters for each posting (WestJet, TransAlta, CNRL, Cenovus, AIMCo, PSP x2, Brookfield, Palantir, Deloitte)
  - `drew-williams-fit-memo-<role>.html` — One-page fit memos mirroring the same roles
- **`prompts/`**
  - `resume-tailoring-codex-cloud-prompt.md` (Codex Cloud runbook)
- **`job-descriptions/`**
  - `deloitte-ts-t-analyst-130388.txt`
- **`notes/`**
  - `tailoring-notes-2025-09-24.md` — competency highlights for the 10 Canadian roles
- **`pdf/`**
  - All exported PDFs (baseline variants, ASCII-safe, 10 tailored resumes, cover letters, fit memos)
- **`txt/`**
  - Plain-text exports of all resumes, cover letters, and fit memos for quick ATS copy/paste submissions

## How to Export to PDF

Use Chrome or Edge for consistent print CSS:

1. Open the desired HTML file in the browser.
2. File → Print → Destination: “Save as PDF”.
3. Paper: US Letter.
4. Margins: Default (CSS controls margins).
5. Scale: 100%.
6. Options: Background graphics ON, Headers/Footers OFF.

If content still spills onto a second page, switch to the next tighter variant (e.g., `v4`) or as a last resort reduce scale to 95% (or 90%).

## Target Role (Deloitte TS&T)

The core ATS variants are tuned to the Analyst/Consultant, Technology, Strategy & Transformation posting (Toronto, ON). Keywords emphasized:

- Technology strategy, operating model (product/platform), business–IT alignment, SDLC, agile.
- Requirements, roadmapping, portfolio management, stakeholder management, change management.
- Cloud, ERP, digital workplace.
- Excel/PowerPoint, SQL, Python, BI.
- AI tools (analysis/drafting/automation).

## Tailoring Guide (for another agent)

- Edit the Summary and Core Competencies to mirror new job keywords.
- Update location line to reflect target city (e.g., Toronto relocation).
- Maintain single-column, simple tags for ATS parsing.
- Keep numbers standardized (e.g., 2016-2020, $120K) for parsers.
- Re-export using the steps above; regenerate PDFs via the provided Chrome headless command if needed.

## Suggested Variants

- General ATS: `drew-williams-resume-ats.html`.
- Single page (most role portals): `drew-williams-resume-ats-single.html`.
- Strict single page: `drew-williams-resume-ats-single-tight-v4.html`.
- Ultra-conservative parser: `drew-williams-resume-ats-single-tight-v4-ascii.html`.
- Role-specific submissions: use the relevant `resume/drew-williams-resume-<role>.html` and matching PDF in `pdf/`.

## Notes

- These files are HTML-only, no external assets required.
- Designed to be readable by both ATS and humans.
- If a portal strips HTML, copy-paste the content into plain text using the ASCII variant.
