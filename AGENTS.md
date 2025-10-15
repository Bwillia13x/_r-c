# Repository Guidelines

## Project Structure & Module Organization

This repository centers on HTML source files in `resume/`, covering resumes, cover letters, and fit memos. Exported deliverables live parallel in `pdf/`, `docx/`, and `txt/`; keep filenames aligned so each slug resolves across formats (e.g., `drew-williams-resume-ats-single-tight-v4.*`). Supporting research and tailoring notes sit in `Informational Context/`, `notes/`, and `job-descriptions/`. The root `index.html` and `README.md` provide quick navigation; avoid duplicating assets outside these folders.

## Build, Test, and Development Commands

Preview any variant locally with `open resume/drew-williams-resume-<slug>.html` (macOS) or by serving the repo via `python3 -m http.server 8000`. Run `npx prettier@latest --check resume/<file>.html` before committing to catch spacing drift; use `--write` when formatting updates are needed. Confirm print readiness through the browser dialog (US Letter, 0.25 in margins, background graphics on) so PDF exports match the baseline documented in `README.md`.

## Coding Style & Naming Conventions

Stick to two-space indentation, lowercase element/class names, and a single `<style>` block per file. Maintain the section order used across variants (`Professional Summary`, `Core Competencies`, `Experience`, `Education`, `Skills & Keywords`) so quick-nav anchors remain stable. Name artifacts `drew-williams-{resume|cover-letter|fit-memo}-<role-slug>.html` and mirror the slug in exported formats. Default to ASCII punctuation unless creating a specific print-polish variant.

## Testing Guidelines

Open each edited file in Chrome or Edge to verify it fits on one page and that anchor links resolve correctly. Use print preview to confirm margins, typography, and absence of orphan headers. Copy the rendered text into a plain editor to validate ATS readability, especially for ASCII-safe variants. When adding or updating a slug, refresh the matching exports in `pdf/`, `docx/`, and `txt/` or note outstanding conversions.

## Commit & Pull Request Guidelines

Follow existing history by leading commit subjects with `docs:` or `docs(resume):` plus a concise change summary (e.g., `docs(resume): add palantir deployment variant`). Scope commits to a single role or batch so reviewers can diff HTML against its exports. Pull requests should outline the target role, major tailoring moves, and any pending deliverables (such as PDF regeneration). Include screenshots or print checks when layout adjustments go beyond content edits.

## Agent Workflow Tips

Start from `resume/reference-ats-template-sample.html` or the closest existing variant to preserve structure and CSS. Log intake notes, JD highlights, and tailoring rationale inside `Informational Context/` with a dated folder for traceability. Update `index.html` whenever you add or rename a public-facing asset so reviewers can locate the new variant quickly.

## ATS Resume Editing Workflow (Operational Playbook)

- **[intake]** Create a dated batch folder under `Informational Context/` and per-role subfolders with `readme.md`.
  - Capture company, role title, location, posting URL, and key JD bullets (responsibilities, skills, tools).
  - Keep filenames slugged consistently across notes and resume files.

- **[stub creation]** Copy `resume/reference-ats-template-sample.html` to `resume/drew-williams-resume-<role-slug>.html`.
  - Update `<title>` and keep header/contact exactly as template.
  - Preserve sections and order: `#summary`, `#skills`, `#experience`, `#education`.

- **[summary & skills tailoring]** Use JD-specific nouns/verbs in 3 bullets for Summary and 8–12 tags for Skills.
  - Prefer ATS-friendly phrases lifted from the JD (e.g., “investment memorandums,” “pitch books/CIMs,” “earnings/quarterly reporting”).
  - Keep Skills as a short tag list; no duplicates; map to JD requirements and tools (e.g., Bloomberg/FactSet, Argus, Capital IQ).

- **[experience deepening]** Edit bullets to mirror JD workflows while staying concise (2–3 bullets per role).
  - M&A: CIM/teaser/IM, DCF/LBO/comps/precedents, diligence workstreams, owner/advisor outreach, integration planning.
  - Equity Research: publications/notes, model and database maintenance, statistical exhibits, quarterly/earnings cadence, client queries.
  - Real Estate IB: pitch books/CIMs, asset-level modeling (Argus), corporate valuations (DCF/comps/precedents), sector research.
  - Maintain documentation, version control, stakeholder cadence, and compliance language where relevant.

- **[page fit & ATS]** Keep everything to a single US Letter page.
  - Verify in browser print dialog: US Letter, ~0.35" margins, background graphics on.
  - Keep bullets one line where possible; prefer concise action-first phrasing.
  - Copy rendered text into a plain editor to confirm ATS readability (ASCII-safe).

- **[manifest & index]** Add each role to `Informational Context/10.14.2025 apps/manifest.json` and (optionally) link from `index.html`.

- **[quality checks]**
  - Run Prettier before committing: `npx prettier@latest --check resume/<file>.html` (use `--write` if needed).
  - Open locally: `open resume/drew-williams-resume-<slug>.html` and confirm anchors and layout.

- **[commit & push]** Stage only the files you touched (notes, manifest, resumes). Use messages like:
  - `docs(resume): add <Company> <Role> ATS variant; tailor JD language; deepen experience bullets; update manifest`
  - Batch commits should clearly list roles included.

- **[branding]** Use `prairiesignal.ca` for consultancy references; replace any legacy names (e.g., `valor-ivx`) with PrairieSignal.
