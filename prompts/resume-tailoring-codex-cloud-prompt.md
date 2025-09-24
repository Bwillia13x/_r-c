# Codex Cloud Prompt: ATS Resume Tailoring Pipeline

## Objective
Generate ATS-optimized, single-page resume variants tailored to a specific job description, plus a cover letter and a one-page fit memo. Maintain strict single-page PDF fit with print CSS, and produce an ASCII-safe variant for strict parsers.

## Inputs
- Candidate info (name, contact, location preferences)
- Master resume content (baseline HTML)
- Target Job Description (JD) text
- Target location (e.g., Toronto) and constraints (single page)

## Constraints & Style
- Single-column, simple semantic HTML (h1/h2/p/ul/li)
- US Letter page size; margins 0.25–0.5in via `@page`
- Font: Arial/Helvetica; base 8.9–10pt; line-height ~1.14–1.35
- Avoid complex tables or multi-column layouts
- Standardize numerics (e.g., 2016-2020, $120K)
- Include an ASCII-safe variant (plain hyphens/quotes)

## Deliverables
- `resume-ats.html` (baseline ATS)
- `resume-ats-single.html` (single-page condensed)
- `resume-ats-single-tight-v1..v4.html` (progressively tighter)
- `resume-ats-printclean.html` (no link previews in print)
- `resume-ats-single-tight-v4-ascii.html` (ASCII-safe)
- `cover-letter.html` (role-targeted)
- `fit-memo.html` (one-page, why-this-role, impact, approach, capabilities)

## Execution Plan
1. Parse JD: extract role keywords (technology strategy, operating model, business–IT alignment, SDLC/agile, requirements, roadmapping, portfolio mgmt, cloud/ERP/digital workplace, Excel/PowerPoint, AI tools, communication, ambiguity, collaboration).
2. Update Summary and Core Competencies to mirror JD language. Keep it concise and outcomes-focused.
3. Ensure Experience bullets emphasize: requirements elicitation, roadmapping, operating model exposure, stakeholder mgmt, executive storytelling, Excel/PowerPoint, analytics tooling, AI productivity.
4. Confirm location line aligns to target city (e.g., open to Toronto relocation).
5. Generate variants, progressively reducing margins, font size, and line-height until single-page fits (v1→v4). Provide ASCII-safe variant.
6. Provide print-to-PDF instructions (Chrome/Edge: Letter, Scale 100%, Background ON, Headers/Footers OFF). If slight overflow persists, advise 95% scale.
7. Produce cover letter and fit memo aligned to JD. Keep letter to ~1 page and memo to crisp bullets.

## Validation
- Visual check in browser
- Print dialog check (1 page)
- Keyword scan against JD

## Handoff
- Commit outputs under `resume/` and `README.md` with export steps.
- Keep edits isolated to resume artifacts.
