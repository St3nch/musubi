# Architecture

## 1. Architectural center

Musubi is not a synchronized representation of VedaOps projects.

It is a separate institutional memory, discovery, and suggestion system that reads project truth without owning it.

```text
Project repositories / native authority
              │
              │ READ ONLY
              ▼
         Musubi reasoner
              │
              ├── institutional memory
              ├── lessons
              ├── signals
              ├── ideas
              ├── relationships
              ├── hypotheses
              └── suggestions
                       │
                       ▼
                 CHAZ / Steward
                       │
              explicit project decision
                       │
                       ▼
             normal project workflow
```

There is no automatic Musubi-to-project-authority path.

## 2. Actor model

### Project repositories

Own their own truth.

They must continue to function correctly if Musubi disappears.

### Source-project agents

Agents working inside a project may notice institutional lessons, useful signals, constraints, or ideas that could matter elsewhere.

They may propose candidate Musubi knowledge.

They do not gain institutional authority by proposing it and cannot change another project through Musubi.

### Musubi reasoner

Reads curated Musubi knowledge and authorized project sources.

It can reason across institutional context and surface possibilities.

It cannot mutate project authority.

### CHAZ / Steward

Provides the human decision boundary.

CHAZ decides whether a Musubi suggestion deserves institutional retention, further investigation, or separately commissioned project work.

## 3. Durable substrate

Initial durable representation:

- Markdown;
- Git;
- small machine-readable metadata only where it earns its maintenance cost;
- normal links and source references;
- Open Knowledge Format semantics where useful and non-distorting.

Musubi is not designed around a vector database, graph database, forge, or specific model/provider.

## 4. Project representation

Musubi should retain the minimum information needed to orient the reasoner and route it toward native authority.

A project entry may contain:

- stable VedaOps subject identity;
- current and useful former names;
- one-sentence purpose;
- authority pointer / how to inspect current truth;
- exceptional institutional warnings or relationships when they add real value.

Musubi should not maintain detailed capability inventories, implementation state, runtime state, current queues, or project-local deferral registers.

## 5. Source observations

An exact Git revision may be recorded selectively when a Musubi note materially depends on repository content.

Its meaning is intentionally narrow:

> The source project was observed at this revision when this Musubi understanding was developed or reviewed.

It is not a semantic truth certificate and creates no universal obligation to keep a cursor synchronized.

Current project claims require native inspection when currentness matters.

## 6. Candidate and curated knowledge

The initial promotion model is deliberately boring:

```text
candidate proposal
      ↓
visible review
      ↓
CHAZ / Steward approval
      ↓
durable Musubi mutation
```

No workflow database, receipt service, approval engine, or candidate-state platform is required.

A curated speculative item remains speculative. Human approval to retain an idea does not transform it into a Product decision.

## 7. Future retrieval

Future retrieval may derive:

- lexical/BM25 indexes;
- hybrid/vector indexes;
- graph projections;
- GraphRAG-style structures;
- catalogs/federation layers;
- summaries and caches.

All remain derived and rebuildable from durable Musubi knowledge.

Derived structures must not turn machine inference into institutional authority merely because retrieval ranks it highly.
