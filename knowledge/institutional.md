# Institutional Knowledge

This file contains a deliberately small initial set of VedaOps-level knowledge and reusable
cross-project lessons.

Retention here does not make a hypothesis true, turn a lesson into universal law, or authorize
project work.

## I1 — Future capability is not backlog

**Type:** Institutional knowledge

**Knowledge:** VedaOps preserves meaningful future Product direction without treating it as
current work. A review trigger creates an obligation to reconsider an idea, not authority to
implement it. Promotion requires fresh Product judgment from CHAZ.

**Source:** Linux VedaOps MCP,
`docs/idea-capability-lifecycle-doctrine.md`.

**Observed source revision:**
`dd812db21abd45381b4d4e1f0f9a725be35570d0`

**Why retain institutionally:** This is explicitly VedaOps-wide doctrine rather than a
project-local implementation choice. Forgetting it would repeatedly turn useful brainstorming,
reviewer findings, and future capability into accidental backlog.

**Limit:** Preserving a future direction does not settle its eventual architecture, provider,
schema, priority, or implementation. Some irreversible evidence-acquisition decisions may have
a different clock from software implementation.

## L1 — Preserve authority; derive convenience

**Type:** Lesson

**Lesson:** When a system has an irreplaceable or semantically authoritative form and a more
convenient derived representation, preserve the authority boundary and allow the derived form
to be rebuilt, revised, or replaced without rewriting the underlying authority.

**Supporting examples:**

- Observatory preserves filesystem Evidence while PostgreSQL Outcomes and Observations are
  rebuildable derivations.
- Discrepancy Desk preserves captured Artifact/Vault authority relative to OCR, transcripts,
  extracted or normalized Surfaces, while separately treating PostgreSQL as authoritative for
  structured investigative Record.

**Observed source revisions:**

- Observatory:
  `d44fa7589a539bd1b29fd460ff1b85509811d662`
- Discrepancy Desk:
  `73941507f2511aca3af8abcf47799bd016c687bf`

**Why it appears transferable:** Both projects independently encountered the danger of a
useful representation becoming mistaken for the thing it represents.

**Conditions:** Apply when the authoritative form and convenient representation genuinely
have different recoverability, provenance, or semantic roles.

**Limits / counterexample:** This does not mean databases are generally disposable.
Discrepancy Desk explicitly makes PostgreSQL 18 authoritative for structured Record state.
The transferable lesson is to identify the actual authority boundary, not to prefer one
storage technology.

**Potential relevance:** Musubi retrieval indexes, future semantic search, derived summaries,
and any project that introduces model-generated or normalized representations of preserved
source material.

## L2 — Keep source presentation, interpretation, and human authority distinct

**Type:** Lesson

**Lesson:** In systems where external sources or models inform consequential reasoning,
represent what the source presented separately from what the system infers and separately
again from what the human decides.

**Supporting examples:**

- Observatory treats provider output as source-attributed testimony rather than universal
  truth and leaves strategy downstream.
- Strategy distinguishes Observatory testimony, Strategy interpretation/recommendation,
  consumer-project authority, and human decision.
- Discrepancy Desk separates Observation, Claim, and human Decision.

**Observed source revisions:**

- Observatory:
  `d44fa7589a539bd1b29fd460ff1b85509811d662`
- Discrepancy Desk:
  `73941507f2511aca3af8abcf47799bd016c687bf`

Strategy Layer was also inspected live while this lesson was developed. Its Git HEAD was
`8b782749c8398e56901c58a586a892605419ca11`, but relevant authority files had uncommitted
working-tree changes, so that commit is not presented as a complete snapshot of the live
Strategy authority observed.

**Why it appears transferable:** The three projects have different domains but independently
need to prevent evidence, interpretation, model output, and human authority from collapsing
into one convenient truth field.

**Conditions:** Most valuable when inputs are contested, provider-attributed, incomplete,
model-interpreted, or consequential enough that provenance and authority matter.

**Limits:** The projects need not share one universal noun model. `Observation`, `Testimony`,
`Claim`, `Interpretation`, `Recommendation`, and `Decision` retain their native project
meanings. Transfer the separation principle, not the schemas.
