---
name: tilt-ai-course-design
description: Use when developing, revising, or reviewing course materials — syllabi, assignments, activities, rubrics — that should follow the TILT (Transparency in Learning and Teaching) framework, and/or need clear disclosure of the creator's own AI use plus a defined AI Assessment Scale (AIAS) level for what students may use AI for. Trigger on requests like "TILT this assignment," "write an AI use policy for my syllabus," "what AIAS level should this be," "disclose how I used AI to build this," or general course/assignment drafting for this class.
---

# TILT + AI Transparency for Course Design

This skill helps build course materials that are transparent on two axes at once:

1. **TILT** — students can see *why* an assignment exists, *what* to do, and *how*
   it will be judged (Winkelmes, TILT Higher Ed).
2. **AI transparency** — students know exactly what AI use is and isn't allowed on
   a given piece of work (via the AI Assessment Scale, AIAS), and the instructor
   discloses their *own* AI use in creating the material, separately.

These are related but distinct disclosures. Don't merge them into one paragraph —
one is about the instructor's process, the other is a policy for students.

Full framework detail lives in `reference/` and is loaded on demand, not all at
once. Fill-in templates live in `templates/`. A worked real-world example combining
all three pieces is in `examples/science-comm-worked-example.md`. Raw source PDFs
are in `context/` if you need to quote something precisely.

## Workflow

**1. Figure out what's actually being asked for.** Common entry points:
   - "TILT this assignment" → do steps 2–4 below, skip 5–6 unless AI comes up.
   - "What AI level should this be?" / "write an AI use policy" → jump to step 5.
   - "Disclose my AI use in building this" → jump to step 6 only.
   - "Build a full syllabus/assignment" → do all steps.
   Don't run the full pipeline when the instructor asked for one piece — ask if
   genuinely ambiguous, but a single request usually implies its own scope.

**2. Gather the essentials before drafting anything.** At minimum: assignment/
   material name, due date, the specific skill(s) and knowledge it targets, and
   roughly what level of student (intro vs. advanced — this affects how many
   skills Purpose should name at once). If the instructor hasn't given this, ask
   — don't invent learning objectives on their behalf. Read `reference/
   tilt-framework.md` for what "good" looks like in each of these before drafting.

**3. Draft Purpose → Task → Criteria using `templates/tilt-assignment-template.md`
   as the skeleton.** Use Bloom's-Taxonomy verbs consistently between Purpose
   (what skill) and Task (what question cues/actions match that skill level).
   If the instructor mentions deliberately withholding information for productive
   struggle, write that rationale into the Task section explicitly rather than
   leaving the ambiguity unexplained.

**4. Self-audit the draft against the checklist in `reference/
   tilt-framework.md`.** Surface any unchecked item to the instructor as a
   question, not a silent fix — some omissions are intentional (e.g., productive
   ambiguity as criteria).

**5. If AI use by students is in scope, determine the AIAS level(s).** Read
   `reference/aias-levels.md` first — it's short and the level-selection logic
   matters more than the labels. Key moves:
   - Start from the learning outcome the task is actually assessing, not the
     assignment's current format.
   - Ask whether one level covers the whole course/material or whether different
     components need different levels (very common — e.g., reflections at Level 1,
     drafting at Level 3). If multiple components, use `templates/
     component-level-ai-policy-table.md`.
   - Don't just attach a number. Make sure the Task/Criteria sections from step 3
     actually reflect that level structurally (required evidence of process for
     Level 2–3, direction-and-critique framing for Level 4–5, invigilation context
     for Level 1) — a label with no structural change is empty.
   - Flag equity considerations (unequal access to paid AI tools, unequal AI
     literacy) if the instructor's policy doesn't address them.

**6. If instructor self-disclosure is in scope, draft it separately** using
   `templates/instructor-ai-disclosure-template.md` and the patterns in
   `reference/ai-disclosure-patterns.md`. Ask what was actually done — don't
   default to a vague "AI was used." Always ask explicitly whether there's a hard
   boundary (e.g., "AI will never grade or give feedback on student work") and
   write it in even if the answer is "no restrictions."

**7. Assemble and present the final material**, keeping the student-facing AIAS
   policy and the instructor's own disclosure visually separate sections. Point
   out any open questions you flagged in steps 4–5 rather than silently resolving
   them.

## Reference files

- `reference/tilt-framework.md` — TILT Purpose/Task/Criteria guidance + self-audit checklist
- `reference/aias-levels.md` — the 5 AIAS levels, selection logic, equity caveats
- `reference/ai-disclosure-patterns.md` — instructor-disclosure pattern + worked examples

## Templates

- `templates/tilt-assignment-template.md` — TILT assignment skeleton with embedded AI-use section
- `templates/instructor-ai-disclosure-template.md` — creator's own AI-use disclosure
- `templates/component-level-ai-policy-table.md` — per-component AIAS policy table

## Examples

- `examples/science-comm-worked-example.md` — real syllabus combining all three pieces
