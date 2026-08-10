# class-dev-skill

A Claude Code skill that helps build course materials — syllabi, assignments,
activities, rubrics — using the **TILT** (Transparency in Learning and Teaching)
framework, with clear, separate disclosures for (1) the instructor's own AI use in
creating the material and (2) which AI Assessment Scale (AIAS) level students are
permitted to use on it.

## What it does

The skill (`SKILL.md`) walks a drafting workflow rather than just handing back a
blank template:

- **TILT drafting** — builds Purpose / Task / Criteria sections using Bloom's
  Taxonomy language (or plain language for affective/psychomotor skills like
  confidence or delivery), then self-audits the draft against TILT's own
  transparent-assignment checklist and flags gaps back to the instructor instead
  of silently filling them in. Supports both a single assignment prompt
  (header-per-section) and a syllabus-level numbered list of learning objectives
  (inline-labeled Purpose/Task/Criteria per objective).
- **AIAS level selection** — starts from the learning outcome being assessed, not
  the assignment's current format, to pick (or help the instructor pick) a level
  1–5 on the AI Assessment Scale (Perkins, Roe & Furze, 2025). Supports a single
  course-wide level or a differentiated policy per component (e.g., reflections at
  Level 1, drafting at Level 3) — most real syllabi need the latter.
  Levels are not a quality hierarchy — no level is "more rigorous" than another.
- **Instructor AI-disclosure** — drafts a statement naming the actual tool(s) used
  to build the material, what they were used for, what was and wasn't delegated,
  and an explicit accountability/boundary statement (e.g., "AI will never be used
  to grade student work"). Kept visually separate from the student-facing AIAS
  policy so the two audiences don't get conflated.

Supporting content lives alongside `SKILL.md`, loaded on demand rather than all at
once:

- `reference/` — condensed TILT and AIAS framework guidance, and instructor-
  disclosure patterns with worked examples, all traceable back to source PDFs.
- `templates/` — fill-in skeletons: a TILT assignment with an embedded AI-use
  section, a numbered syllabus-level learning-objectives list, a standalone
  instructor-disclosure statement, and a per-component AIAS policy table.
- `examples/` — a real syllabus that already combines all three pieces, used as a
  model for tone and structure.
- `context/` — the original source material (TILT Higher Ed templates and
  checklist, the AIAS papers, a worked syllabus) the rest of the skill is
  distilled from.

It's structure and framework knowledge, not a generic writing assistant — it
doesn't know the specifics of any one course. See `SKILL.md` for the exact
step-by-step workflow.

## Install

Download and extract this repo directly into a skills directory — no Node/npm
required. Choose one:

**Per-project** (only available in this repo):

```sh
mkdir -p <your-project>/.claude/skills/tilt-ai-course-design
curl -fsSL https://github.com/bu-bioinfo/class-dev-skill/archive/refs/heads/main.tar.gz \
  | tar -xz -C <your-project>/.claude/skills/tilt-ai-course-design --strip-components=1
```

**Global** (available in every project):

```sh
mkdir -p ~/.claude/skills/tilt-ai-course-design
curl -fsSL https://github.com/bu-bioinfo/class-dev-skill/archive/refs/heads/main.tar.gz \
  | tar -xz -C ~/.claude/skills/tilt-ai-course-design --strip-components=1
```

To update to the latest version later, just re-run the same command — it
overwrites the existing install.

(Note: this skill's `SKILL.md` references files under `reference/`, `templates/`,
`examples/`, and `context/` in the same directory, so installers that fetch only
`SKILL.md` — such as `npx skills add` — will not work here.)

## Use

In Claude Code, ask it to work on course material and let the description in
`SKILL.md` match naturally — e.g. "TILT this assignment," "what AIAS level should
this lab be," "write an AI use policy for my syllabus," or "disclose how I used AI
to build this slide deck."
