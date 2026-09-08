---
name: writing-for-agents
description: Write or edit Musubi documents intended to guide capable agents, especially AGENTS.md, authority/context docs, skills, and retrieval-facing knowledge.
---

# Writing for Agents — Musubi mode

Write for progressive disclosure and reliable agent behavior.

- Put high-cost authority mistakes near the top of the document that prevents them.
- Use one canonical home for each rule; point rather than duplicate when possible.
- Prefer explicit boundaries, source pointers, and examples over motivational prose.
- Separate Product authority from non-authoritative design/research.
- Preserve qualifications that change action. Retrieval of correct-but-incomplete text is a failure mode.
- Do not encode model-specific quirks as Product doctrine unless they are durable environmental facts.
- Keep context documents bounded enough that a fresh model can orient without reading the whole repository.

When writing a skill, make clear that the skill is working method rather than Product authority and cannot widen permissions or self-promote its output.
