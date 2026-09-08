# Operating Model

## 1. Read mode

Read mode is the default conversational posture.

```text
Musubi corpus:           READ
Project authority:    READ ONLY
Musubi mutation:         OFF
Project mutation:     IMPOSSIBLE FROM Musubi
```

The reasoner may search, compare, infer, challenge, brainstorm, and discuss possibilities without changing durable Musubi state.

This is the preferred mode for ordinary conversation.

## 2. Write mode

Write mode must be explicitly enabled for durable Musubi mutation.

```text
Musubi corpus:           READ + PROPOSE WRITE
Project authority:    READ ONLY
Project mutation:     IMPOSSIBLE FROM Musubi
```

The reasoner may prepare an exact proposed Musubi mutation.

Before writing:

1. show the proposed change or diff to CHAZ;
2. identify what type of Musubi item is being changed;
3. identify important source/basis material where relevant;
4. wait for explicit approve / reject / revise instruction;
5. only then perform the Musubi mutation.

> **No conversational reasoning causes a durable Musubi mutation without CHAZ seeing the proposed mutation first.**

## 3. Project boundary

Musubi never receives project-write authority.

A Musubi suggestion that may deserve project work follows a separate path:

```text
Musubi suggestion
      ↓
CHAZ / Steward evaluation
      ↓
inspect current project authority
      ↓
explicit Product decision
      ↓
separate project ticket / commission
      ↓
project writer works under project governance
```

The Musubi reasoner cannot skip this boundary.

## 4. Project-agent contributions

A source-project agent may produce a candidate institutional contribution when it notices something worth retaining across VedaOps.

Examples:

- reusable lesson;
- new cross-project constraint;
- technology signal;
- potentially relevant idea;
- changed reassessment condition;
- meaningful failure or gotcha.

The contribution remains candidate material until CHAZ / the Steward accepts the proposed Musubi mutation.

## 5. Human responsibility

CHAZ is intentionally part of the Product architecture.

Musubi is not designed to eliminate human Product judgment.

CHAZ's responsibilities include:

- deciding what deserves attention;
- accepting or rejecting durable Musubi mutations;
- distinguishing interesting ideas from distractions;
- deciding whether a suggestion should become project work;
- commissioning that work through the affected project's authority;
- rejecting Musubi reasoning when it is wrong.

## 6. Future autonomy

Future narrowly bounded automatic Musubi maintenance may be reconsidered only after repeated real work proves that a specific mutation is deterministic, low-risk, and burdensome to perform manually.

Semantic institutional writes remain preview-before-write by default unless a later reviewed decision explicitly changes that rule.
