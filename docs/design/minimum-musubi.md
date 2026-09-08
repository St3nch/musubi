# Minimum Musubi Prototype

## Goal

Test whether durable institutional memory improves cross-project reasoning and continuity beyond a strong baseline of portfolio index + project-native documentation + live read-only source access.

The prototype should be deliberately small enough that failure cannot be blamed on missing infrastructure.

## Minimum durable corpus

### Portfolio / authority map

For each VedaOps subject:

- stable subject identity;
- current/useful former names;
- one-sentence purpose;
- how to inspect native authority;
- only exceptional institutional warnings or relationships worth preserving.

### Institutional knowledge

A small set of genuinely cross-project or VedaOps-level notes.

### Lessons

Only lessons with real reuse value, supporting examples, and applicability limits.

### Signals

Only signals tied to real institutional questions.

### Ideas / suggestions

Only possibilities worth retaining or bringing to CHAZ's attention.

### Institutional decisions

Only VedaOps-level decisions actually made by CHAZ whose natural durable home is not one project.

### Historical / rejected material

Only where forgetting would cause repeated work, recurring bad ideas, or loss of important rationale.

## Explicitly absent

The prototype does not include:

- vector search;
- graph storage;
- GraphRAG;
- federation;
- project-state mirroring;
- lifecycle/posture enums;
- mandatory reconciliation cursors;
- knowledge-impact receipts;
- project-closeout gates;
- automatic ingestion;
- proactive monitoring;
- automatic semantic writes;
- a UI beyond what is needed to interact with the reasoner and preview changes.

## Access model

```text
Musubi reasoner → Musubi                  read
Musubi reasoner → project authority    read-only
Musubi reasoner → project mutation     impossible
normal conversation → Musubi mutation  off
write mode → Musubi mutation           proposal + preview + CHAZ approval
```

## Success shape

The prototype earns expansion only if it repeatedly helps a fresh reasoner do at least some of the following better than the baseline:

- recover institutional rationale that project-local search misses;
- transfer a useful lesson safely across projects;
- suppress a previously rejected/deferred idea whose conditions have not changed;
- notice that a genuine reassessment condition has changed;
- identify a valuable cross-project opportunity;
- distinguish current fact, historical context, and Musubi inference;
- reduce the amount of context CHAZ must reconstruct manually;
- improve a real Product decision after maintenance cost is counted.

## Failure shape

If Musubi mostly restates project documentation, creates more material for CHAZ to review, or produces suggestions a fresh reasoner with the baseline would find just as well, shrink it.

If the smallest useful form is only a portfolio index plus native repo access, that is an acceptable outcome.
