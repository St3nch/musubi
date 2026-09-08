# Musubi Deferred / Future Direction

These are durable **Accepted Direction** or **Research Required** items, not backlog. A Review trigger or Revisit point creates a fresh Product review obligation only. It never authorizes implementation.

When an item is revisited, current technology, providers, assumptions, and Product needs must be reconsidered rather than treating old implementation guesses as architecture.

## F1 — Universal stable concept identifiers

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** HORIZON

**Direction / question:** Determine whether Musubi eventually needs stable concept identity independent of file paths.

**Why it matters:** Moves, renames, federation, or external references may eventually make path identity costly.

**Why not now:** Stable VedaOps subject identities plus ordinary paths are sufficient at prototype scale.

**Review trigger:** Repeated concept moves/renames break durable references, or multiple bundles require cross-bundle identity.

**Revisit point:** Major architecture review after the first real corpus has accumulated.

**Evidence basis:** OKF/path-identity design review.

**Cost of forgetting:** Later refactors could accumulate brittle links or ad-hoc identifiers.

**Not authorized:** UUID layer, global ID service, migration machinery, or schema work now.

## F2 — Typed relationship vocabulary / knowledge graph schema

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** TRIGGERED

**Direction / question:** Determine whether explicit relationship semantics are needed beyond links and prose.

**Why it matters:** Typed relationships may improve later cross-project reasoning and graph retrieval.

**Why not now:** Links and prose are sufficient; ontology work would be speculative.

**Review trigger:** A repeated important cross-project query fails because relationship meaning cannot be recovered reliably from normal links and text.

**Revisit point:** First retrieval review that documents such a failure.

**Evidence basis:** Adversarial review of the pre-project knowledge model.

**Cost of forgetting:** We could either overbuild an ontology early or rediscover the need after concrete failures without preserving why it was deferred.

**Not authorized:** Knowledge-graph schema, mandatory edge types, graph database, or GraphRAG.

## F3 — Vector / hybrid retrieval

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** TRIGGERED

**Direction / question:** Determine whether semantic/vector or hybrid retrieval adds measured value over text search and link traversal.

**Why it matters:** Semantic retrieval may improve recall for implicit, paraphrased, or composed questions.

**Why not now:** The corpus is small and simpler retrieval is cheaper and inspectable.

**Review trigger:** Measured reconnect tests show important recall, noise, or latency failures that simpler retrieval cannot solve acceptably.

**Revisit point:** After a minimum-prototype evaluation exposes retrieval failures.

**Evidence basis:** LLM-native retrieval research and reviewer subtraction.

**Cost of forgetting:** We could mistake a future retrieval failure for a model problem or prematurely lock into today's vector tooling.

**Not authorized:** Qdrant, pgvector, embeddings pipeline, vector schema, or provider selection now.

## F4 — GraphRAG / graph projection

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** TRIGGERED

**Direction / question:** Determine whether machine-assisted graph/community projection improves concrete cross-project reasoning tasks.

**Why it matters:** Some future relationship-composition tasks may benefit from graph-derived retrieval.

**Why not now:** No measured query requires it, and inferred edges create provenance and confirmation-loop risk.

**Review trigger:** Repeated relationship-composition failures survive good text/link retrieval.

**Revisit point:** The evaluation cycle that demonstrates the failure.

**Evidence basis:** Future-infrastructure research and adversarial review.

**Cost of forgetting:** A useful future projection could be missed, or an attractive graph stack could be adopted without evidence.

**Not authorized:** GraphRAG implementation, graph database, inferred-edge promotion, or ontology work.

## F5 — Multi-bundle federation / catalog

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** TRIGGERED

**Direction / question:** Determine how independent Musubi knowledge bundles should be discovered if one repository stops being appropriate.

**Why it matters:** Scale, access boundaries, or ownership may eventually require independent bundles.

**Why not now:** One small corpus is easier to inspect and govern.

**Review trigger:** A real access, ownership, scale, or repository-performance boundary requires a second independent bundle.

**Revisit point:** The Product/architecture review that proposes the second bundle.

**Evidence basis:** OKF/federation research.

**Cost of forgetting:** Partitioning could happen ad hoc and make discovery or identity inconsistent.

**Not authorized:** Catalog service, federation protocol, cross-bundle index, or global namespace now.

## F6 — Fine-grained sensitivity / ACL platform

**Disposition:** Accepted Direction  
**Pillar:** Agent Interaction & Governance  
**Clock:** TRIGGERED

**Direction / question:** Preserve the ability to introduce restricted knowledge classes if ordinary Musubi visibility becomes too broad.

**Why it matters:** Commercial, customer-derived, contractual, or otherwise restricted knowledge may eventually need different visibility boundaries.

**Why not now:** The ordinary corpus can begin under one coarse private/internal visibility rule and exclude sensitive material entirely.

**Review trigger:** A legitimate knowledge class cannot safely be exposed to every model/provider environment authorized for ordinary Musubi.

**Revisit point:** Before admitting the first such restricted class.

**Evidence basis:** Independent adversarial reviews of the first design.

**Cost of forgetting:** Sensitive material could become difficult to remove from Git history, model contexts, or future derived indexes.

**Not authorized:** ACL service, per-note permissions, encryption architecture, or sensitive-data ingestion.

## F7 — Automated evidence/source ingestion

**Disposition:** Research Required  
**Pillar:** Institutional Memory  
**Clock:** TRIGGERED

**Direction / question:** Determine whether a bounded source class should be ingested automatically.

**Why it matters:** Repeated manual discovery/capture may eventually become expensive.

**Why not now:** Automation can create noise, prompt-injection exposure, deduplication burden, and false institutional weight.

**Review trigger:** Repeated manual capture of a bounded source class is measurably expensive and has clear provenance, retention, deduplication, and review behavior.

**Revisit point:** The first review documenting that repeated bottleneck.

**Evidence basis:** Security/promotion-boundary review.

**Cost of forgetting:** Manual work could remain unnecessarily expensive, or ingestion could be automated without a trustworthy boundary.

**Not authorized:** Crawlers, feeds, monitoring daemons, automated admission, or external-provider spend.

## F8 — Automatic semantic Musubi rewriting

**Disposition:** Research Required  
**Pillar:** Agent Interaction & Governance  
**Clock:** HORIZON

**Direction / question:** Determine whether any semantic Musubi mutation can safely occur without ordinary human preview.

**Why it matters:** Very repetitive deterministic maintenance might eventually justify automation.

**Why not now:** Semantic mutation is where LLM error can compound across future sessions and become false institutional memory.

**Review trigger:** A narrow write class is deterministic, reversible, repeatedly approved, and contains no institutional judgment.

**Revisit point:** Major governance review after substantial real write history exists.

**Evidence basis:** Clarified actor/authority review.

**Cost of forgetting:** Either needless human ceremony persists forever or unsafe automation is introduced casually.

**Not authorized:** Autonomous semantic writes, auto-promotion, or removal of preview-before-write as the default.

## F9 — Project-closeout knowledge integration

**Disposition:** Research Required  
**Pillar:** Institutional Memory  
**Clock:** TRIGGERED

**Direction / question:** Determine whether source-project closeout should ever emit a bounded institutional-knowledge review signal.

**Why it matters:** Some project changes may create cross-project lessons or reassessment conditions worth noticing.

**Why not now:** Musubi does not need continuous project synchronization, and mandatory closeout coupling would violate the clarified lightweight model.

**Review trigger:** Repeated real project work loses important institutional consequences because nobody notices them after closeout.

**Revisit point:** The first post-project review showing repeated loss.

**Evidence basis:** First design/review reconciliation.

**Cost of forgetting:** Useful lessons may remain trapped in projects, while premature integration would create project→Musubi dependency.

**Not authorized:** Mandatory closeout gate, synchronous dual-write, project dependency on Musubi, or automatic knowledge admission.

## F10 — Knowledge-impact receipts

**Disposition:** Research Required  
**Pillar:** Institutional Memory  
**Clock:** TRIGGERED

**Direction / question:** Determine whether a tiny durable breadcrumb is useful when project work may have institutional consequences.

**Why it matters:** A lightweight pointer could help later review without synchronizing project state.

**Why not now:** No live workflow has demonstrated that ordinary project review and Musubi research miss this information.

**Review trigger:** F9's trigger fires and a bounded breadcrumb is shown to solve the loss with less coupling than other approaches.

**Revisit point:** During the corresponding project-closeout integration review.

**Evidence basis:** First design pack; later reviewer subtraction.

**Cost of forgetting:** We could either lose useful review cues or resurrect receipt machinery as if it were already justified.

**Not authorized:** Receipt schema, mandatory MCP closeout behavior, or automatic Musubi updates.

## F11 — Session capsules

**Disposition:** Research Required  
**Pillar:** Institutional Memory  
**Clock:** TRIGGERED

**Direction / question:** Determine whether bounded session summaries preserve material context that repository authority and normal Musubi notes fail to retain.

**Why it matters:** Important rationale can disappear into chat if it has no durable Product home.

**Why not now:** Automatic session summaries can create noise and duplicate lower-quality versions of authority.

**Review trigger:** Multiple meaningful sessions repeatedly lose rationale, findings, or candidate knowledge despite normal repository discipline.

**Revisit point:** The first review demonstrating repeated loss across sessions.

**Evidence basis:** LLM continuity research.

**Cost of forgetting:** Reconnect burden may stay high; premature capsules could flood the corpus.

**Not authorized:** Automatic chat export, session ingestion, model-memory sync, or capsule schema.

## F12 — Formal correction ledger / contradiction graph

**Disposition:** Research Required  
**Pillar:** Institutional Memory  
**Clock:** TRIGGERED

**Direction / question:** Determine whether ordinary Git history and prose are insufficient to represent material corrections or unresolved contradictions.

**Why it matters:** Future models must not silently flatten correction, supersession, or tension.

**Why not now:** The doctrine can preserve those distinctions without an event model.

**Review trigger:** A material knowledge error or cross-source contradiction cannot be represented cleanly through normal files, links, and Git history.

**Revisit point:** The review of that concrete correction/contradiction.

**Evidence basis:** Original temporal/history design pressure.

**Cost of forgetting:** Important causal history could become opaque, while a premature ledger would create ceremony.

**Not authorized:** Correction database, contradiction graph, universal event sourcing, or migration machinery.

## F13 — Formal cold-reconnect evaluation harness

**Disposition:** Accepted Direction  
**Pillar:** Retrieval & Evolution  
**Clock:** NEXT

**Direction / question:** Build a repeatable evaluation only after the first usable Musubi retrieval path exists.

**Why it matters:** Musubi must prove value over the baseline rather than rely on intuition.

**Why not now:** There is not yet a working corpus/retrieval path worth automating around.

**Review trigger:** The minimum prototype can answer real Musubi-vs-baseline tasks.

**Revisit point:** First minimum-prototype evaluation.

**Evidence basis:** Long-memory/RAG evaluation research and both adversarial reviews.

**Cost of forgetting:** Musubi could expand based on anecdotes and sunk cost rather than measured value.

**Not authorized:** Benchmark framework, synthetic score, CI gate, or infrastructure before the minimum prototype exists.

## F14 — Physical repository partitioning / large-scale Git optimization

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** HORIZON

**Direction / question:** Determine whether repository size/performance or access boundaries require physical partitioning.

**Why it matters:** Durable knowledge need not live in one monolithic repository forever.

**Why not now:** No measured scale problem exists.

**Review trigger:** Repository size, directory width, clone/fetch latency, maintenance cost, or access boundaries become materially painful.

**Revisit point:** Major scale/operations review when those symptoms appear.

**Evidence basis:** Git-scale research.

**Cost of forgetting:** Scaling could be treated as an emergency or, conversely, optimized prematurely.

**Not authorized:** Multi-repo split, sharding, large-file strategy, or federation implementation.

## F15 — Agent-native forge / Cursor Origin adoption

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** HORIZON

**Direction / question:** Reassess agent-native forge capabilities if a real Musubi workflow would materially benefit from them.

**Why it matters:** Future forge-native agents, checks, events, or multi-repository workflows may reduce operational friction.

**Why not now:** Current forge behavior is not a Musubi Product requirement and future products may differ materially from today's options.

**Review trigger:** A real VedaOps workflow requires forge-native agent execution, multi-repository agents, native automation, or institutional-review events that current GitHub workflows cannot satisfy well.

**Revisit point:** The architecture review for that concrete workflow.

**Evidence basis:** 2026-09-07 agent-native forge research.

**Cost of forgetting:** We may miss a useful future workflow or accidentally treat today's vendor as predetermined architecture.

**Not authorized:** Origin migration, Origin-specific schema, dual-write, or forge dependency.

## F16 — Forge-event normalization / source-change monitoring

**Disposition:** Research Required  
**Pillar:** Retrieval & Evolution  
**Clock:** HORIZON

**Direction / question:** Determine whether external project/forge events should ever create bounded Musubi review signals.

**Why it matters:** At larger scale, manual awareness of meaningful changes may become expensive.

**Why not now:** Musubi does not require synchronized project state, and no event-driven problem has been measured.

**Review trigger:** Manual discovery of relevant source changes repeatedly misses time-sensitive institutional review obligations.

**Revisit point:** The first review documenting that repeated failure.

**Evidence basis:** Future forge/reconciliation research.

**Cost of forgetting:** Event integration may be rediscovered without remembering why it was intentionally omitted.

**Not authorized:** Webhooks, polling service, event schema, or automatic semantic reconciliation.

## F17 — Stable machine-readable Project schema/enums

**Disposition:** Research Required  
**Pillar:** Institutional Memory  
**Clock:** TRIGGERED

**Direction / question:** Determine whether repeated machine queries justify structured Project attributes beyond minimal identity/orientation/authority pointers.

**Why it matters:** Some future retrieval or policy tasks may need machine-readable attributes.

**Why not now:** Prose and authority pointers are more honest; lifecycle/posture/capability mirrors risk shadow authority.

**Review trigger:** A repeated important retrieval or policy task fails specifically because the needed Project attribute is not machine-readable.

**Revisit point:** The evaluation/retrieval review documenting that failure.

**Evidence basis:** Both adversarial reviews and Product clarification.

**Cost of forgetting:** We could either rebuild a shadow project model or miss a small earned structured field when it becomes useful.

**Not authorized:** Lifecycle enum, development-posture enum, capability mirror, project-state schema, or synchronization machinery.

## F18 — Autonomous or proactive institutional radar

**Disposition:** Research Required  
**Pillar:** Discovery & Ideas  
**Clock:** HORIZON

**Direction / question:** Determine whether bounded proactive review can surface high-value opportunities without becoming an attention tax.

**Why it matters:** Musubi may eventually notice reassessment candidates or useful cross-project opportunities before CHAZ asks the exact question.

**Why not now:** Idea generation is cheap; CHAZ's attention is not. Proactivity can create confirmation loops and noise.

**Review trigger:** On-demand Musubi repeatedly produces high-value institutional discoveries and there is evidence that bounded proactive review would save attention.

**Revisit point:** Major Product review after sustained useful on-demand operation.

**Evidence basis:** Clarification follow-up review and Product attention constraint.

**Cost of forgetting:** Valuable proactive potential could be lost, or an institutional Clippy could be built without evidence.

**Not authorized:** Scheduled idea generation, automatic notifications, opportunity quotas, or autonomous project proposals.

## F19 — Automatic Musubi writes without per-change preview

**Disposition:** Research Required  
**Pillar:** Agent Interaction & Governance  
**Clock:** HORIZON

**Direction / question:** Determine whether any non-semantic housekeeping class can safely bypass per-change preview.

**Why it matters:** Some deterministic maintenance may eventually be unnecessarily burdensome to review manually.

**Why not now:** Preview-before-write is the primary defense against self-contaminating institutional memory.

**Review trigger:** A narrow write class is deterministic, reversible, repeatedly approved, and contains no institutional judgment.

**Revisit point:** Major governance review after substantial real Musubi mutation history.

**Evidence basis:** Product clarification and reviewer findings.

**Cost of forgetting:** Review burden could remain unnecessarily high, or the safety boundary could erode informally.

**Not authorized:** Semantic auto-writes, model self-approval, bulk admission, or removal of preview from ordinary knowledge changes.

## F20 — Idea Workbench

**Disposition:** Accepted Direction  
**Pillar:** Discovery & Ideas  
**Clock:** TRIGGERED

**Direction / question:** Allow CHAZ eventually to capture, develop, research, pressure-test, defer, revive, reject, or mature ideas that do not yet belong to an existing VedaOps Project. Ideas may range from one-line sparks to nearly complete Product concepts.

**Why it matters:** The workbench could let a Musubi reasoner evaluate new ideas against current projects, institutional knowledge, prior ideas, lessons, constraints, technology, market research, and portfolio sequencing instead of giving generic fresh-chat advice.

**Why not now:** Core Musubi must first prove that its institutional memory and cross-project reasoning provide real value. Before that, an Idea Workbench would mostly be a generic LLM brainstorming interface.

**Review trigger:** Core Musubi is operating successfully and CHAZ begins regularly using Musubi to preserve or develop ideas that do not yet belong to current Projects.

**Revisit point:** First major Product review after the core Musubi prototype is in real use.

**Evidence basis:** CHAZ Product direction during Musubi pre-project design; see `docs/design/idea-workbench-deferred.md`.

**Cost of forgetting:** Ideas and their rationale continue disappearing into temporary chats or get reconsidered later without the accumulated institutional context that could change the judgment.

**Not authorized:** Numerical idea scoring, automatic project creation, automatic ticket conversion, autonomous commissioning, automated portfolio prioritization, or implementation of the workbench before fresh Product review.
