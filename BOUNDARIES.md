# Boundaries

This document defines what Musubi should and should not retain.

The default question is:

> **Does retaining this in Musubi add institutional meaning that would otherwise be expensive to recover?**

If not, leave it in its native source.

## A. Belongs in Musubi

Examples:

- cross-project relationships whose meaning is not owned by one project;
- transferable lessons with evidence and limitations;
- institutional rationale;
- portfolio-level context;
- meaningful technology/vendor signals tied to real questions;
- ideas and hypotheses worth retaining;
- suggestions for CHAZ to consider;
- recurring rejected ideas and why they remain rejected;
- reassessment conditions;
- VedaOps-level institutional decisions actually made by CHAZ;
- unresolved cross-project questions and tensions;
- important historical institutional context;
- minimal authority/navigation pointers.

## B. Belongs only in native project authority

Examples:

- Product doctrine for that project;
- accepted project decisions;
- code and implementation detail;
- project-local tickets and work plans;
- project-local deferrals;
- detailed capability inventories;
- project-local history;
- runtime/operational state;
- current project queue or priority state;
- acceptance records for project changes.

Musubi may discuss institutional implications without copying the native body of truth.

## C. Reference but do not copy wholesale

Examples:

- ADR collections;
- full project documentation;
- runtime records;
- Evidence stores and raw captures;
- customer datasets;
- research archives;
- vendor documentation and release-note collections;
- long transcripts;
- large historical registers.

Use pointers and bounded attributed excerpts only when they support a specific institutional insight.

## D. Should not enter the ordinary Musubi corpus

Examples:

- credentials, tokens, passwords, secrets;
- raw customer data;
- customer PII;
- protected Evidence payloads owned by another system;
- full confidential contracts;
- raw operational databases;
- material inappropriate for every model/provider environment authorized to use ordinary Musubi;
- routine chat narration and raw reasoning traces;
- generic brainstorming with no identifiable institutional value;
- duplicate suggestions that add no evidence or meaningful variation;
- stale signals whose retention costs more than rediscovery.

## Sensitivity seam

The first prototype does not need a full ACL platform.

It does need one coarse rule:

> The ordinary Musubi corpus contains private internal VedaOps institutional knowledge suitable for every model/provider environment explicitly authorized to consume that corpus.

If a future knowledge class cannot safely satisfy that rule, it must stay outside the ordinary corpus until a real restricted-knowledge boundary is designed and reviewed.
