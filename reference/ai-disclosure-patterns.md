# Instructor AI-Disclosure Patterns — Reference

This is about the creator's own AI use in *building* the course material — separate from, but often placed near, the AIAS policy that governs *students'* AI use in *completing* it. Don't conflate the two in a draft; a syllabus typically needs both, clearly distinguished.

## The reusable pattern

A credible instructor disclosure statement has four components, in this order:

1. **Which tools, specifically.** Name the actual model/product (e.g., "Claude Sonnet 5," "ChatGPT o3-mini-high") — not a vague "AI was used." Precision here is itself the transparency being modeled.
2. **For what purpose.** Brainstorming/ideation, outlining, drafting text, editing/copyediting, formatting — name the actual activity, not a blanket claim.
3. **Degree of reliance / what was NOT delegated.** State what was created manually first and what AI touched after the fact, or vice versa. If there's a boundary that was never crossed (e.g., "AI was never used to grade or give feedback on student work"), state it explicitly — boundary statements are often more informative to students than the positive disclosure.
4. **Human accountability.** A closing statement that the instructor reviewed, edited, and takes responsibility for all resulting content. This is not boilerplate — it's the load-bearing claim that AI assistance didn't outsource judgment.

## Worked examples found in source material

**Academic paper acknowledgement (Furze, Perkins, Roe & MacVaugh, 2024):**
> "This study used GenAI tools for revision and editorial purposes... Models used were ChatGPT (GPT-4) and Claude 3 (Opus). The authors reviewed, edited and take responsibility for all outputs."

**Academic paper acknowledgement (Perkins, Roe & Furze, 2025 — more granular):**
> "...used GenAI tools for ideation and in some passages of draft text creation which was then heavily revised, along with editing and revision... selected and used supportively and not to replace core author responsibilities... reviewed, edited, and take responsibility for all outputs."

**Syllabus disclosure (Science Communication Syllabus, instructor's own material-creation disclosure — note this is framed *in AIAS terms*, reusing the same scale for self-disclosure that the syllabus also uses for students):**
> "This syllabus was developed with AI assistance at Levels 2 and 3 of the AI Assessment Scale (Perkins, Furze, Roe & MacVaugh, 2024). AI tools were used for brainstorming, outlining, and suggestions; all content was generated manually first before AI suggested edits and revisions approved by the instructor. AI will never be used to evaluate or provide feedback on any student assessment in this course. All feedback is conducted solely by the instructor."

That last example is the strongest model to imitate: it (a) cites the framework and version, (b) reuses the AIAS's own vocabulary to describe the *instructor's* process — which only works if the instructor's workflow actually maps onto specific levels — (c) narrates the actual workflow (manual-first, then AI-assisted revision), and (d) draws an explicit, separate boundary line for what AI will never touch (student grading/feedback), which matters more to students than the creation-process disclosure itself.

## Multi-artifact disclosures

A single lab/activity folder often bundles several artifacts with genuinely
different AI-authorship provenance — a narrative README, a companion worksheet
that's a mechanical, fill-in-the-blank derivative of the README's own Task/
Criteria text, and generated analysis or data-processing code. Collapsing these
into one blanket statement ("AI was used to help build this lab") hides exactly
the distinction that makes the disclosure credible. Disclose each artifact
separately:

- **Narrative content** (README prose, case write-ups, learning objectives):
  state the actual editorial role — e.g., "used to edit existing text for
  clarity and organization and to suggest draft learning objectives," critically
  reviewed and edited by the instructor before inclusion.
- **Structural/mechanical derivatives** (a worksheet template whose fields are
  algorithmically derived from another document's own headings/prompts): name
  it as "fully AI-generated" *and* explain why that's low-risk — it's a fixed
  structural derivation of already-instructor-authored content, not original
  narrative or graded content.
- **Generated code** (analysis pipelines, data-processing scripts): name the
  actual workflow if one was used — e.g., a behavior-driven design (BDD)
  workflow where test/behavior specifications were written first and AI
  generated implementation code to satisfy them — and state that the instructor
  manually reviewed and tested it before use.
- **What was authored manually, with no AI involvement at all** (e.g., case data,
  grading criteria): say so explicitly and by name. This is as load-bearing as
  disclosing what *was* AI-assisted — students and reviewers need to know which
  artifacts are fully human-authored ground truth.

Close with one explicit **Boundary** line that covers the whole bundle (e.g.,
"AI was not used to generate case data or grading criteria, and is not used to
evaluate or grade student submissions") — don't let the boundary get diluted by
being restated per-artifact.

## Guidance for drafting one with an instructor

- Ask what was actually used, don't assume — ideation only? Drafting? Editing? Formatting/slide generation? Literature search? Code/data-pipeline help? Each implies different disclosure language.
- If the instructor's own creation workflow doesn't map cleanly onto AIAS levels (levels are designed for *student assessment tasks*, not necessarily authorship), don't force the mapping — plain-language process description is fine and often clearer. The Science Comm syllabus example maps its own creation onto AIAS levels because that syllabus already teaches AIAS to students; that reuse is a nice touch but not a requirement.
- Always ask explicitly: "Is there anything AI should never be used for in this course (e.g., grading, personalized feedback, accommodations decisions)?" and write that boundary into the disclosure even if the answer is "no restrictions" — silence reads as unconsidered, not as permissive.
- Keep the disclosure near the syllabus's AI-use policy for students but visually/structurally distinct — one is "how I made this," the other is "what you may do." A single combined paragraph tends to confuse the two audiences (institution/accreditation readers vs. students).
