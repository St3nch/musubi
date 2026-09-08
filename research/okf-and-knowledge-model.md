# Research Note — OKF and the Musubi Knowledge Model

**Status:** non-authoritative research input  
**Checked:** 2026-09-07

## Why OKF remains a useful floor

Open Knowledge Format v0.2's Markdown + YAML frontmatter, Git-native portability, provenance/freshness fields, links, and implementation-neutral posture align well with Musubi's durable-layer goals.

Musubi should use OKF semantics where they help without forcing all institutional meaning into an OKF schema. Markdown must remain directly useful even if no OKF-specific serving system exists.

## Path-based identity

OKF concept identity is path-based. That is adequate for the first corpus. Musubi should distinguish a file/concept path from stable VedaOps subject identity where such identity already exists (for example a project id).

Do not introduce universal concept UUIDs until real moves, renames, external references, or federation make path identity insufficient.

## Source revision observations

A source-dependent Musubi note may optionally record the Git revision observed while developing or reviewing that note.

The revision is a source-reading clue, not a universal verification cursor, semantic certificate, or obligation to synchronize Musubi after every project commit. When current project truth matters, read native authority.

## Relationships

Use normal Markdown links and explicit prose first. Typed relationship vocabulary should be earned by failed real retrieval/reasoning cases rather than invented as an ontology up front.

## Federation

Do not solve multi-bundle discovery now. Revisit it only when scale, access, ownership, or repository boundaries require independent bundles.

## Canonical source

- Open Knowledge Format repository: `https://github.com/GoogleCloudPlatform/open-knowledge-format`
