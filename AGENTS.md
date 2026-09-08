# Musubi Agent Instructions

## Roles and authority

- **CHAZ** is Product Owner and final human Product authority.
- **ChatGPT** is the VedaOps Project Steward.
- Other models may perform bounded Writer, reviewer, research, or operator tasks; they are not Project Steward.
- One Writer per implementation ticket when implementation work exists.
- Repository/live authority outranks chat memory, model confidence, reviewer consensus, and derived summaries.

## Canonical authority order

1. `AGENTS.md`
2. `VISION.md`
3. `VOCABULARY.md`
4. `decisions/decisions.md`
5. `decisions/deferred.md`
6. accepted ADRs
7. accepted specifications
8. accepted tickets
9. non-authoritative `docs/design/` and `research/` material

When authority conflicts, stop and surface the conflict. Do not manufacture reconciliation from chat memory.

## Core boundary

> **Musubi reads truth and writes possibility.**

- Each VedaOps project remains authoritative for itself.
- Musubi project access is read-only.
- Projects must remain able to function correctly without Musubi.
- Musubi suggestions do not authorize project work.
- Any consequence for another project must be separately considered and commissioned through that project's own authority and governance.
- Musubi must never become a synchronized second representation of project implementation/runtime truth.

## Musubi write boundary

Ordinary Musubi conversation is read-only.

For durable semantic Musubi changes:

1. prepare the exact proposed mutation or diff;
2. show it to CHAZ before writing;
3. identify the knowledge type and important basis/provenance;
4. obtain explicit approve/reject/revise direction;
5. only then mutate durable Musubi state.

> **No conversational reasoning causes a durable Musubi mutation without CHAZ seeing the proposed mutation first.**

Repository commissioning/governance changes explicitly requested by CHAZ may be executed through the governed VedaOps MCP boundary and reviewed by diff before commit.

## External-effect gates

No push, publication, spend, provider/network action carrying credentials or cost, production mutation, destructive operation, or new external integration without explicit CHAZ authorization.

A local commit is not a push. A trigger is not authorization. A recommendation is not authorization.

## Current work boundary

Current work is **Musubi foundation commissioning and minimum-prototype preparation**.

Allowed now:

- establish authoritative Product/governance docs;
- preserve research/design history as non-authoritative input;
- install/adapt bounded project-local working-method skills;
- design and evaluate the minimum Musubi prototype;
- define future directions without implementing them.

Not authorized now:

- software implementation without an accepted ticket;
- vector/hybrid infrastructure;
- GraphRAG or graph storage;
- federation/catalog services;
- automated external ingestion;
- automatic semantic reconciliation;
- proactive institutional radar;
- automatic project closeout integration;
- the Idea Workbench;
- automatic Musubi-to-project handoff or project mutation.

## Future-direction doctrine

Musubi adopts the VedaOps Idea and Capability Lifecycle Doctrine.

- Future capability is not backlog.
- Brainstorming, LLM/reviewer suggestions, and Writer discoveries are inputs, not authority.
- Material future direction receives a durable disposition when forgetting it would be costly.
- `CURRENT`, `NEXT`, `TRIGGERED`, and `HORIZON` describe review timing, not implementation schedules.
- Review triggers and Revisit points create review obligations only.
- Only fresh CHAZ Product judgment may promote future direction into current work.
- Canonical future-direction register: `decisions/deferred.md`.

Musubi Product Pillars:

- **Institutional Memory**
- **Discovery & Ideas**
- **Agent Interaction & Governance**
- **Retrieval & Evolution**

## Project-local skills

Canonical reviewed working-method skills live under `.agents/skills/`. Thin client pointers may live under `.claude/skills/` and `.grok/skills/`.

Current earned skill surface:

- `research` — bounded source-based investigation and technical/Product research;
- `grilling` — stress-test a plan or idea through explicit decision branches;
- `domain-modeling` — sharpen Musubi terminology and durable concept boundaries;
- `writing-for-agents` — write authority/context documents for capable agents;
- `future-capability-reconciliation` — preserve future direction without manufacturing backlog.

Skills are working method, not Product authority. They cannot widen permissions or promote their own output. Add engineering skills such as implementation, TDD, debugging, ticketing, or code review only when real implementation work earns them.

## Durable knowledge discipline

- Retained does not mean believed.
- Believed does not mean decided.
- Suggested does not mean authorized.
- A project fact should normally be live-read from that project's authority when currentness matters.
- Consequential suggestions preserve basis, inference, assumptions/limits, and counterevidence.
- Do not allow one Musubi inference to return later as fake independent corroboration. Preserve source ancestry sufficiently to recognize repetitions.
- Unknown is a valid result.
- Preserve conclusions, evidence, and decisions—not private chain-of-thought.

## Repository discipline

- Keep authoritative files small enough for useful progressive disclosure.
- Do not create empty directory forests or speculative schemas.
- `docs/design/` and `research/` are non-authoritative unless a higher authority explicitly adopts a conclusion.
- Future retrieval/indexing layers must remain rebuildable derivatives of durable knowledge.
- Do not place credentials, raw customer PII, protected project Evidence, raw operational databases, or material unsuitable for every authorized Musubi model/provider into the ordinary corpus.
