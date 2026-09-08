# Musubi Idea Workbench — Deferred Capability

**Status:** Non-authoritative deferred design note  
**Applies to:** Musubi  
**Timing:** Revisit only after the core Musubi system is built, operating, and has demonstrated value  
**Authority:** Non-authoritative elaboration. The canonical Product disposition is `decisions/deferred.md` F20. This note does not authorize implementation.

---

## Purpose

Musubi should eventually provide an **Idea Workbench**: a place where CHAZ can capture, develop, research, pressure-test, defer, revive, reject, or mature ideas that do not yet belong to an existing VedaOps Project.

An idea may be anything from a one-line thought to a nearly complete Product concept.

The goal is not to score ideas.

The goal is to work with them intelligently using the institutional context Musubi already has.

> **An idea does not need to belong to a current Project in order to deserve a place to be explored.**

---

## Product concept

CHAZ should be able to bring an idea to Musubi in whatever state it currently exists:

- a rough thought;
- a possible feature;
- a research direction;
- a business or commercial idea;
- a new Product concept;
- an infrastructure idea;
- an agent workflow;
- a technology opportunity;
- a project-sized proposal;
- an old idea worth reconsidering.

Musubi should preserve the original idea, then allow CHAZ and the Musubi reasoner to work on it over time.

The Musubi reasoner should evaluate the idea in the context of:

- current VedaOps Projects;
- institutional knowledge;
- prior ideas;
- rejected or deferred directions;
- cross-project lessons;
- known constraints;
- existing capabilities;
- technology/vendor signals;
- current market or external research;
- portfolio sequencing;
- relevant historical context.

The workbench should help move an idea from an initial thought toward a useful judgment.

---

## Intended workflow

```text
CHAZ has an idea
      ↓
capture the original idea
      ↓
work on it with the Musubi reasoner
      ↓
clarify the problem / opportunity
      ↓
compare against VedaOps knowledge
      ↓
identify unknowns
      ↓
research only where useful
      ↓
pressure-test assumptions
      ↓
revise the idea
      ↓
reach a reasoned disposition
```

The Idea Workbench should support repeated sessions. An idea should not need to be completed or judged when first captured.

---

## Preserve the original idea

The original idea should remain distinguishable from later interpretation.

Musubi should not silently rewrite CHAZ's initial thought into what the LLM believes the idea ought to be.

A mature workbench may therefore distinguish conceptually between:

### Original idea

CHAZ's original wording or supplied concept.

### Developed understanding

What the idea has become through discussion, research, and refinement.

### Musubi analysis

The reasoner's interpretation, supporting context, criticism, and suggestions.

This preserves the history of how the idea evolved.

---

## What Musubi should help determine

Depending on the maturity of the idea, Musubi may explore questions such as:

- What problem is this actually trying to solve?
- Who would benefit from it?
- Does an existing VedaOps Project already cover part of it?
- Would this be better as a capability of an existing Project?
- Does it deserve to become a separate Project?
- Have we considered or rejected something similar before?
- What previous lessons apply?
- What existing VedaOps capabilities could support it?
- What important dependencies exist?
- What assumptions are weak?
- What is genuinely novel?
- What external research is needed?
- What technology would need to exist?
- What commercial or Product role could it have?
- What would make us regret building it?
- Why might this be the wrong time?
- What would have to change before it becomes attractive?

The workbench should be able to challenge an idea as aggressively as it develops one.

---

## Research

Research should be available when an idea earns it.

```text
idea
  ↓
important unknowns
  ↓
research questions
  ↓
external / technical / market research
  ↓
findings
  ↓
reassessment
```

Research may strengthen, weaken, reshape, defer, or kill an idea.

Research should not be performed merely to make every captured thought look substantial.

---

## Reasoned dispositions, not scores

The Idea Workbench must not reduce ideas to numerical scores.

A useful conclusion is a reasoned judgment.

Examples may include:

- strong enough to consider commissioning;
- promising, but more research is needed;
- interesting but premature;
- blocked by a specific dependency;
- revisit when a stated condition changes;
- keep dormant;
- probably not viable;
- not possible under current constraints;
- superseded by another direction;
- better suited to an existing Project;
- candidate for a future new Project.

These are examples, not a required fixed enum.

The explanation matters more than the label.

---

## Idea → Project boundary

An Idea is not a Project.

A favorable Musubi assessment does not create or authorize a Project.

```text
IDEA WORKBENCH
      ↓
idea matures
      ↓
Musubi may recommend Project consideration
      ↓
CHAZ decides
      ↓
if approved:
normal VedaOps Project commissioning / onboarding
```

Only CHAZ can decide that an idea should cross into actual Project work.

The Musubi reasoner must not automatically:

- create a new Project;
- authorize implementation;
- commission a writer;
- modify an existing Project;
- convert an idea into Project authority.

---

## Relationship to existing Projects

A major value of the Idea Workbench is that it should reason inside the actual VedaOps landscape rather than provide generic startup or Product advice.

For example, a new idea may overlap with:

- an existing Observatory capability;
- a Search Clarity commercial direction;
- a Discrepancy Desk research lesson;
- a previously deferred Neon Ronin hypothesis;
- a technology signal preserved elsewhere in Musubi.

Musubi should be able to surface those relationships without assuming they authorize integration or implementation.

---

## Long-lived ideas

Some ideas may remain in the workbench for years.

That is acceptable.

Musubi should be able to preserve:

- why the idea mattered;
- why it was not pursued;
- what assumptions blocked it;
- what conditions would justify reassessment;
- what later evidence changed the picture.

This allows a future reasoner to notice that an old obstacle has disappeared.

Example:

```text
old idea
   +
new technology
   +
changed project capability
   +
changed market condition
   ↓
"this may deserve reassessment"
```

A reassessment suggestion still does not authorize Project work.

---

## Attention discipline

The Idea Workbench should not become an idea-spam system.

Generating possibilities is cheap. CHAZ's attention is not.

The system should therefore prefer a small number of meaningful conclusions over large volumes of speculative suggestions.

It should be able to say:

> **Nothing here currently deserves further attention.**

A useful future question for every surfaced idea is:

> **Why does this deserve CHAZ's attention now?**

---

## Musubi write and authority boundaries still apply

The Idea Workbench does not change Musubi's core authority model.

- Project repositories remain authoritative for their own truth.
- Musubi access to Projects remains read-only.
- Musubi suggestions do not modify Project authority.
- Normal Musubi conversational mode may remain read-only.
- Durable Musubi changes should follow the Musubi preview-and-approval model.
- CHAZ remains the human decision boundary between institutional reasoning and commissioned Project work.

---

## Why this capability is deferred

The core Musubi system must first demonstrate that institutional memory and cross-project reasoning provide real value.

Building an Idea Workbench before Musubi has a useful institutional corpus would mostly produce a generic LLM brainstorming interface.

The capability becomes more valuable only after Musubi has accumulated enough real knowledge to reason about new ideas in the context of actual VedaOps history, Projects, lessons, constraints, and decisions.

---

## Reassessment trigger

Revisit the Idea Workbench when:

> **The core Musubi system is operating successfully and CHAZ begins regularly using Musubi to preserve or develop ideas that do not yet belong to a current Project.**

The trigger permits a fresh Product/design review.

It does **not** authorize implementation.

When triggered, review real examples of how CHAZ has been developing ideas and design the smallest workbench that supports those actual workflows.

---

## Explicitly not authorized by this note

This deferred direction does not authorize:

- numerical idea scoring;
- automated project creation;
- autonomous Project commissioning;
- automatic idea-to-ticket conversion;
- automatic implementation;
- automated portfolio prioritization;
- autonomous spending or external action;
- a large idea-management workflow engine;
- speculative database/schema machinery;
- automatic promotion of an LLM suggestion into institutional or Project authority.

---

## Long-term Product possibility

If Musubi proves itself, the Idea Workbench could become one of its most valuable interfaces.

Instead of asking a fresh generic LLM:

> “Is this a good idea?”

CHAZ could ask an institutional reasoner:

> **“Here is my idea. Given everything VedaOps has learned, what should change how I think about it?”**

That is the capability this note preserves.
