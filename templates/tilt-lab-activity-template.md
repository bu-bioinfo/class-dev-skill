<!--
Fill-in template for a multi-part lab/activity handout — e.g., a discussion segment
plus a hands-on case-analysis segment in one session. Structure: title/timing header,
then one `## Part N` section per activity segment, each containing `### Instructions`
followed by `### Learning Objectives` — objectives come AFTER instructions, not
before, since students need to know what they're doing before being told why it
matters. Each objective is a `#### {skill-named title}` heading (no "Objective N:"
numbering — the part already scopes it) with Purpose/Task/Criteria blockquoted
underneath, one level more compact than the inline-labeled but unquoted prose in
tilt-learning-objectives-template.md.

Use this template for a single lab/activity session with one or more discrete parts;
use tilt-learning-objectives-template.md for a syllabus-level objectives list, and
tilt-assignment-template.md for one graded assignment prompt. See
reference/tilt-framework.md ("Presentation formats") for when each shape applies,
and reference/ai-disclosure-patterns.md ("Multi-artifact disclosures") if this
activity bundles a README, a companion worksheet, and/or generated analysis code
with different AI-authorship provenance.

Each part should make clear what AIAS level applies to it and why — parts
commonly warrant different levels (e.g., a group discussion/ranking part may be
fine at Level 3 AI Collaboration, while a part whose point is students forming
their own read of raw output before comparing notes may call for Level 1 No AI).
What matters is that the level and a short rationale are present *somewhere* for
each part — not the exact placement or format. Put it in the part heading, a line
under it, a shared section after all parts if levels repeat, or wherever else
fits the document naturally. See reference/aias-levels.md and
templates/component-level-ai-policy-table.md.
-->

# {Lab/Activity number} - {Title}

**Estimated time:** {~X minutes total (Part 1: ~Y minutes {short description};
Part 2: {short description})}

## Part 1 {optionally note its AIAS level here, e.g. "(AIAS Level 1 - No AI)"}

<!-- State this part's AIAS level and a short rationale for it somewhere in this
part — in the heading above, a line here, or a shared section if it's the same
across parts. Format is up to you; just make sure it's actually there. -->

### Instructions

{What students actually do in this part — discussion prompts, a ranking task, a
dataset to inspect, etc. Name any companion file(s) they should use to record
answers, e.g.: Use [`worksheet_template.md`](worksheet_template.md) to record
your group's answers.}

### Learning Objectives

#### {Skill-named title, e.g., "Interpret sequencing QC metrics by their impact on downstream analysis"}

> **Purpose — Why this matters:** {1–2 sentences on why this skill matters
> beyond this one activity — what it lets students correctly judge or do
> afterward.}
>
> **Task — What you will do:** {The concrete activity in this part that builds
> the skill — what students reason about, rank, or decide.}
>
> **Criteria — How you'll know you're succeeding:** {Observable signs of
> success specific enough for students to self-assess against — what
> distinction they should be able to draw by the end.}

<!-- Repeat the #### objective block above for each additional objective this
part builds. -->

## Part 2 {optionally note its AIAS level here}

<!-- Same reminder as Part 1 — level + rationale should be findable somewhere,
even if it's just a pointer to a shared statement covering both parts. -->

### Instructions

{What students do in this part. If it builds on Part 1's output (e.g., "in your
same groups..."), say so explicitly. State any assumptions students should take
as given for the activity (what's real vs. constructed, what hint they're given,
etc.) so the ambiguity that remains is intentional, not confusing.}

### Learning Objectives

#### {Skill-named title}

> **Purpose — Why this matters:** {...}
>
> **Task — What you will do:** {...}
>
> **Criteria — How you'll know you're succeeding:** {...}

<!-- Repeat the ## Part N section above for each additional part of the activity
(with its AIAS level + rationale noted somewhere), and the #### objective block
for each objective within it. -->

## AI Use Disclosure (Course Materials)

{Draft using templates/instructor-ai-disclosure-template.md and the patterns in
reference/ai-disclosure-patterns.md. If this activity bundles multiple artifacts
with different AI-authorship provenance — e.g., a narrative README, a
mechanically-derived worksheet template, generated analysis/data code — disclose
each artifact's provenance separately rather than one blanket statement, and
state the boundary (what AI was never used for, e.g., generating case data or
grading criteria) explicitly. See "Multi-artifact disclosures" in
reference/ai-disclosure-patterns.md.}

<!--
Self-check before distributing: run this draft against the checklist in
reference/tilt-framework.md (per objective) and confirm the AI Use Disclosure
covers every distinct artifact in this activity's directory, not just the README.
-->
