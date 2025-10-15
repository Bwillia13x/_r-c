# ATS Resume Variant Playbook

## 1. Intake checklist
- **Capture job context**: company, role title, location, work modality, seniority, requirements. Store supporting research notes inside `Informational Context/`.
- **Clarify positioning**: confirm target headline, priority skills, metrics to highlight, and any sponsor projects.
- **Identify resume source**: choose the closest existing variant in `resume/` to repurpose.

## 2. Template baseline
- **Start from reference file**: copy `resume/reference-ats-template-sample.html` into a new role-specific file `resume/drew-williams-resume-<slug>.html`.
- **Preserve structure**: keep header, quick-nav, sections (`summary`, `skills`, `experience`, `education`, `additional`). Maintain tag list markup under `#skills`.
- **Update metadata**: set `<title>` to `Drew Williams — <Role>` and adjust the contact tagline (`Analyst / Consultant — …`) to match the role.

## 3. Section guidance
- **Summary**: 3 connected sentences (scope → strengths → signature impact). Mention PrairieSignal when relevant. Include target company/role in muted trailing clause if space allows.
- **Skills (tag list)**: group 10–12 tags mixing competencies, tools, and methodologies tied to the JD keywords. Avoid duplicates across variants on same page.
- **Experience**:
  - Order reverse chronological.
  - Each item: keep `.item` wrapper, `.item-header` grid, and `<ul class="bullets">`.
  - Bullets follow *action + lever + quantified/qualitative impact*. Mirror employer vocabulary (e.g., “portfolio governance”, “AI automation”).
  - Surface 3–4 bullets per role; prune or condense to preserve one-page fit.
- **Education**: keep single item with GPA, honors, scholarships. Update metadata if degree details change.
- **Additional**: optional bulleted list for certifications, availability, work authorization, or differentiators.

## 4. Formatting rules
- **Typography**: leave CSS variables untouched unless size tweaks are absolutely necessary. If adjusting for overflow, prefer toggling `body` class to `dense`.
- **Quick-nav**: ensure IDs exist for every link; adjust anchor labels when sections renamed.
- **Spacing**: use provided `.section + .section` separators. No extra `<br>` elements.
- **Branding**: always cite `prairiesignal.ca` (never “valor-ivx”).

## 5. Quality checks
- **Visual**: open in browser (`open resume/drew-williams-resume-<slug>.html`) to confirm layout, no orphaned headers, single page.
- **ATS text scan**: copy rendered text into a plain editor to confirm linear reading order and tag readability.
- **Keyword alignment**: cross-check bullets and tags against the top JD requirements; add missing synonyms where space allows.
- **Version control**: stage only the new/changed resume file and related context notes, then commit with message `Add ATS resume variant for <Company Role>`.

## 6. Delivery
- **Provide review instructions**: share quick-nav highlights and notable tailoring decisions in chat.
- **Export reminder**: user converts to PDF after approving content; recommend system print dialog with background graphics enabled if color accents used.

Following this playbook keeps every new resume variant consistent with our ATS-ready template while allowing rapid job-specific tailoring.
