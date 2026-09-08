# Knowledge Model

This is a content model, not a database schema or ontology.

The goal is to preserve enough context that future LLMs can distinguish source fact, institutional interpretation, and possibility.

## 1. Serious suggestions

A consequential suggestion should be able to answer:

### What is the suggestion?

Plain statement of the possibility being proposed for consideration.

### Why now?

What changed, accumulated, or became newly relevant?

### Basis

Which project facts, institutional lessons, signals, research, or prior decisions contributed?

### Musubi inference

What part is the reasoner's synthesis rather than something directly stated by a source?

### Assumptions / limits

Under what conditions does this reasoning hold?

### Counterevidence

What evidence, constraints, or prior lessons push against it?

### Requested consideration

What is Musubi actually asking CHAZ to consider?

The suggestion should not imply authorization.

## 2. Lessons

A reusable lesson should preserve:

- the lesson;
- supporting source/example;
- why the lesson appears transferable;
- conditions where it applies;
- known limits or counterexamples;
- related projects or contexts where it may be relevant.

Example failure to avoid:

> Project A's database is rebuildable, therefore databases are disposable.

The source example and transfer conditions must survive the abstraction.

## 3. Signals

A signal should normally preserve:

- what was observed;
- when it was observed;
- source;
- why it might matter;
- what would need verification before it becomes actionable.

Technology/vendor signals should not be treated as current capability claims without fresh verification when currentness matters.

## 4. Ideas

An idea may be lightweight.

Retention should still answer at least:

- what is the idea;
- why it is worth remembering;
- whether it is new, rejected-before, deferred, or speculative;
- what condition would make it worth reconsidering if not now.

## 5. Institutional decisions

A VedaOps-level institutional decision should record:

- the decision actually made by CHAZ;
- effective scope;
- rationale where useful;
- date;
- affected projects or questions;
- whether any project-local authority must be updated separately.

The LLM may draft the record. It cannot create the decision by drafting it.

## 6. Provenance ancestry

Musubi must avoid treating its own previous output as independent corroboration.

If:

```text
Musubi idea A
   ↓
inspires project proposal B
   ↓
Musubi later reads B
```

B is not independent evidence for A merely because it appears in a different repository.

Initially, ordinary source links and explicit provenance notes are sufficient to preserve this ancestry.

No graph database is required.

## 7. Attention quality

More ideas are not better institutional memory.

A suggestion worth surfacing should normally be able to answer:

> **Why does this deserve CHAZ's attention now?**

The reasoner may successfully return:

> Nothing worth surfacing right now.
