# Review Reconciliation Note

**Status:** non-authoritative design history

The first pre-project design pack was independently reviewed by two capable external reasoners.

Both initially returned a reconciliation-level verdict and converged on several useful criticisms:

- Project concept documents risked becoming stale shadow summaries;
- a Git revision was being asked to carry too much semantic meaning;
- lifecycle/posture enums were premature;
- knowledge-impact receipts and closeout machinery were unearned;
- sensitivity boundaries and candidate/curated separation deserved earlier attention;
- vectors, GraphRAG, federation, automatic reconciliation, and similar infrastructure should remain deferred.

A later Product clarification materially changed the architecture under review:

> **Musubi reads truth and writes possibility.**

The clarified model established that Musubi is not synchronized project knowledge, project repos are read-only to the Musubi reasoner, projects do not depend on Musubi, and CHAZ remains the boundary between institutional suggestion and commissioned project work.

One reviewer explicitly revised its verdict from `RECONCILE` to `SOUND WITH MATERIAL CORRECTIONS` under that clarified model and withdrew much of the synchronization/reconciliation criticism.

The resulting v0.2 design therefore keeps the useful subtraction from both reviews while centering Musubi on institutional memory, discovery, lessons, signals, ideas, suggestions, and portfolio reasoning rather than project-state mirroring.

This note is design history, not project authority.
