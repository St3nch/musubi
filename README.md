# VedaOps Musubi

**Reads truth. Writes possibility.**

**Status:** governed project foundation v0.2  
**Repository:** `https://github.com/St3nch/musubi`

Musubi is the LLM-native institutional memory, discovery, and suggestion system for VedaOps.

Individual VedaOps projects remain independently authoritative for their own Product doctrine, accepted decisions, implementation, code, project-local deferrals, runtime state, and project-local history. Musubi reads those sources when current truth matters; it does not synchronize, replace, or override them.

Projects must function correctly without Musubi. Musubi depends on project truth; projects do not depend on Musubi.

## Product constraint

> **Musubi should reduce what CHAZ must remember, not increase what CHAZ must review.**

Musubi succeeds when durable institutional memory helps a fresh capable reasoner recover important context, avoid repeated mistakes, identify useful cross-project connections, preserve worthwhile possibilities, and surface only conclusions that earn attention.

## Authority / read order

1. `AGENTS.md`
2. `VISION.md`
3. `VOCABULARY.md`
4. `decisions/decisions.md`
5. `decisions/deferred.md`
6. `ARCHITECTURE.md`
7. `BOUNDARIES.md`
8. `OPERATING-MODEL.md`
9. `KNOWLEDGE-MODEL.md`
10. accepted ADRs/specifications/tickets when they exist
11. `docs/design/` and `research/` as non-authoritative design/research input

## Current phase

Musubi is being commissioned as a governed VedaOps project. The current job is to establish and test the smallest useful institutional-memory foundation.

No accepted ticket currently authorizes software implementation. In particular, the current foundation does **not** authorize vector search, GraphRAG, federation, automated reconciliation, proactive radar, autonomous semantic writes, project mutation, or the future Idea Workbench.

See `decisions/deferred.md` for preserved future directions and their reassessment conditions.
