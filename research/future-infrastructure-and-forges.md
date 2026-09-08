# Research Note — Future Retrieval Infrastructure and Git Forges

**Status:** non-authoritative research input  
**Checked:** 2026-09-07

## Retrieval infrastructure

The durable corpus should not be designed around a particular future retrieval engine.

Possible later projections include:

- lexical/BM25 search;
- hybrid dense+sparse/vector retrieval;
- Qdrant, pgvector, OpenSearch, Vespa, or successors;
- GraphRAG or another graph/community extraction pipeline;
- a catalog/federation layer spanning multiple OKF bundles.

The key architectural rule is that indexes and graph projections are rebuilt from durable Musubi knowledge and retain walkback to source concepts/revisions.

## Git scale

Git is not required to remain one monolithic repository forever. The useful invariant is portable, version-controlled knowledge.

GitHub currently recommends repository and directory bounds for healthy operation (including roughly 10 GB on-disk `.git` size and about 3,000 entries per directory). Those figures are nowhere near the current design, but they are evidence that physical layout should remain evolvable.

If scale/access boundaries eventually require multiple bundles, federation becomes a separate concern rather than a reason to abandon the durable Markdown/OKF model.

## Cursor Origin

Cursor Origin is currently early beta. It is a Git forge oriented around agentic development and currently supports standard Git operations, GitHub mirroring, PRs/reviews, code browse/search, cloud agents, automations, apps, checks, and multi-repository environments.

The feature most relevant to future institutional maintenance is the combination of source-control events and native agents. A future reconciliation agent could react to project changes, inspect a revision range, and create a reconciliation candidate without making the forge itself the knowledge authority.

### Adoptable patterns now

- keep VedaOps Project identity separate from forge repository identity;
- use immutable Git SHA as the cross-forge reconciliation primitive;
- design future closeout results so a forge could display them as machine-readable checks;
- design future event handling as idempotent/deduplicatable;
- prefer least-privilege app/install credentials over user-wide tokens;
- allow multi-repository reconciliation in future interfaces;
- treat PR/review metadata as supporting evidence below repository authority.

### Do not adopt now

- Origin-specific frontmatter;
- Origin repository IDs as institutional IDs;
- Cursor Automations as required infrastructure;
- Origin-native hosting as current authority;
- dual-write GitHub/Origin behavior;
- an Origin API dependency inside the durable knowledge model.

### Safe future experiment

When a real workflow requires it, mirror one bounded GitHub repository into Origin while GitHub remains source of truth. Measure whether agent-native PRs, multi-repo workflows, review, closeout, or knowledge reconciliation are materially better before considering migration.

## Sources

- Cursor Origin overview: https://cursor.com/docs/origin
- Origin integrations/automations: https://cursor.com/docs/origin/integrations
- Origin API: https://prod.cursor.com/docs/api/origin
- GitHub mirroring: https://prod.cursor.com/docs/origin/mirror-github
- GitHub repository limits: https://docs.github.com/en/repositories/creating-and-managing-repositories/repository-limits

## Musubi reconciliation note

This research predates the final Musubi actor clarification. Agent-native forges, event normalization, and automated source-change handling remain possibilities only; Musubi does not require project synchronization and no forge-specific future is predetermined. See `decisions/deferred.md`.
