# Resume Artifacts — Drew Williams (ATS-Optimized)

This repository contains the most recent resume work tailored for Deloitte Technology, Strategy & Transformation (TS&T). It includes multiple single-page, ATS-friendly HTML variants with progressively tighter layouts so you can export clean, one-page PDFs across different printers and portals.

## Contents
- `resume/` — HTML deliverables
  - `drew-williams-resume-ats.html` — Baseline ATS single-column version
  - `drew-williams-resume-ats-single.html` — Single-page condensed
  - `drew-williams-resume-ats-printclean.html` — Print-clean (no link previews on print)
  - `drew-williams-resume-ats-single-tight.html` — Tight layout
  - `drew-williams-resume-ats-single-tight-v2.html` — Tighter
  - `drew-williams-resume-ats-single-tight-v3.html` — Very tight
  - `drew-williams-resume-ats-single-tight-v4.html` — Maximum compression (recommended for single-page PDF)
  - `drew-williams-resume-ats-single-tight-v4-ascii.html` — ASCII-safe variant (plain hyphens/quotes, ideal for strict parsers)

## How to Export to PDF
Use Chrome/Edge for consistent print CSS:
1. Open one of the HTML files in your browser
2. File → Print → Destination: "Save as PDF"
3. Paper: US Letter
4. Margins: Default (CSS sets page margins)
5. Scale: 100%
6. Options: Background graphics ON, Headers/Footers OFF

If content still spills onto a second page:
- Switch to the next tighter variant (e.g., `v4`).
- As a last resort, reduce scale to 95% (or 90%).

## Target Role (Deloitte TS&T)
These variants are tuned to the posting for Analyst/Consultant, Technology, Strategy & Transformation (Toronto, ON). Keywords emphasized:
- Technology strategy, operating model (product/platform), business–IT alignment, SDLC, agile
- Requirements, roadmapping, portfolio mgmt, stakeholder mgmt, change mgmt
- Cloud, ERP, digital workplace
- Excel/PowerPoint, SQL, Python, BI
- AI tools (analysis/drafting/automation)

## Quick Tailoring Guide (for another agent)
- Edit the Summary and Core Competencies to mirror new job keywords
- Update location line to reflect target city (e.g., Toronto relocation)
- Maintain single-column, simple tags for ATS parsing
- Keep numbers standardized (e.g., 2016-2020, $120K) for parsers
- Re-export using the steps above

## Suggested Variants
- General ATS: `drew-williams-resume-ats.html`
- Single page (most role portals): `drew-williams-resume-ats-single.html`
- Strict single page: `drew-williams-resume-ats-single-tight-v4.html`
- Ultra-conservative parser: `drew-williams-resume-ats-single-tight-v4-ascii.html`

## Notes
- These files are HTML-only, no external assets required
- Designed to be readable by both ATS and humans
- If a portal strips HTML, copy-paste the content into plain text using the ASCII variant
