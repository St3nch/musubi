# Vision

## North star

Build a durable, LLM-native institutional memory and discovery system for VedaOps that lets a fresh capable reasoner recover the institutional context needed to continue useful work without relying on prior chat memory.

> **Musubi reads truth and writes possibility.**

Musubi should help VedaOps remember what matters across projects, discover meaningful relationships, preserve lessons and reasons, notice changed conditions, and surface worthwhile possibilities without becoming a second authority over the projects it observes.

## LLM-native, not model-dependent

The durable system must survive replacement of ChatGPT, Claude, Grok, Cursor, or any other model/provider.

Markdown and Git are the initial durable substrate because they remain readable, inspectable, portable, and easy to rebuild indexes from later.

The primary interaction model is LLM-first, but the durable knowledge must remain usable by humans and future tools without a specific model.

## Authority boundary

Each VedaOps project remains the sole authority for its own:

- Product doctrine;
- accepted project decisions;
- implementation;
- code;
- project-local deferrals;
- runtime and operational state where applicable;
- project-local history.

Musubi may point to, summarize narrowly, or reason from those sources. It does not become a shadow copy of them.

When current project truth matters, the Musubi reasoner reads native authority.

## Musubi's institutional job

Musubi exists primarily for knowledge whose useful scope is broader than one project or whose value lies in durable institutional reuse.

Examples include:

- cross-project relationships;
- transferable lessons and their limits;
- institutional rationale;
- recurring mistakes and known traps;
- technology or vendor signals tied to real questions;
- ideas and hypotheses worth retaining;
- suggestions for CHAZ to consider;
- reasons an idea was rejected or deferred;
- conditions that could justify reassessment;
- unresolved cross-project tensions;
- portfolio-level sequencing or other accepted VedaOps-level judgments;
- historical context that would otherwise be expensive to reconstruct.

Musubi is allowed to retain possibility without pretending possibility is fact or authorization.

## Separate reasoner

The Musubi reasoner is an institutional analyst, not a project executive.

It may:

- read Musubi;
- search Musubi;
- compare knowledge across projects;
- inspect native project authority read-only;
- form hypotheses;
- identify opportunities or tensions;
- suggest reassessment;
- prepare proposed Musubi changes when write mode is explicitly enabled.

It may not:

- mutate project repositories;
- authorize project implementation;
- convert its own suggestion into a project decision;
- treat a trigger as authorization;
- silently turn its own inference into durable trusted institutional knowledge.

## Human decision boundary

CHAZ remains the Product Owner and the decision boundary between institutional reasoning and commissioned project work.

A Musubi suggestion can become project work only through a separate decision and the affected project's normal governed process.

Musubi may be the durable home for a VedaOps-level institutional decision after CHAZ makes it, but Musubi does not create that decision's authority merely by storing it.

## Useful uncertainty

A good Musubi reasoner must be able to say:

- unknown;
- source unavailable;
- current truth requires a live read;
- evidence is conflicting;
- this is an inference rather than a source fact;
- this idea was retained but not adopted;
- this trigger has fired but no work is authorized.

Uncertainty is preferable to plausible invention.

## Attention economy

Musubi should not become an institutional idea spammer.

A successful reasoner may conclude:

> Nothing worth surfacing right now.

Suggestions should earn attention by explaining why they matter now, what changed, what evidence supports them, and what assumptions limit them.

## Future retrieval invariant

Future lexical indexes, vector stores, graph projections, summaries, caches, catalogs, and other retrieval systems may be added when demonstrated pressure requires them.

They remain rebuildable derivatives of durable Musubi knowledge and must preserve enough source identity and provenance for walkback.

They are retrieval infrastructure, not institutional authority.
