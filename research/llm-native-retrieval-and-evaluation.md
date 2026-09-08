# Research Note — LLM-Native Retrieval and Evaluation

**Status:** non-authoritative research input  
**Checked:** 2026-09-07

## Why this matters

“LLM-native” is not satisfied by putting Markdown where an agent can search it. The system must eventually prove that a cold model can recover the right institutional evidence efficiently and reason correctly from it.

## LongMemEval-V2

LongMemEval-V2 (May 2026) evaluates whether memory can help agents become experienced colleagues in customized environments. Its five memory abilities map unusually well to VedaOps:

1. **static state recall** — what exists and what is true about the environment;
2. **dynamic state tracking** — what changed over time;
3. **workflow knowledge** — how work is actually performed;
4. **environment gotchas** — recurring local failure modes;
5. **premise awareness** — recognizing that a seemingly reasonable assumption is wrong in this particular environment.

Its context-gathering formulation also evaluates a memory system that returns compact evidence to a fixed reader model, which fits the desired separation between retrieval and reasoning.

### VedaOps example of premise awareness

Bad inference:

> Strategy is a registered active VedaOps project, therefore Strategy implementation is active.

Correct institutional reasoning:

> Registry/project existence and Product development posture are separate. Strategy implementation is deliberately frozen while preservation-only work may continue.

## LOCOMO-CONV

LOCOMO-CONV (September 3, 2026) argues that ordinary explicit QA can miss memory failures that appear in natural conversation. It evaluates dialog, implicit, counterfactual, and composed query styles and finds important retrieval gaps on implicit/composed questions.

This supports testing Musubi memory with realistic work prompts rather than only trivia-like questions.

Example explicit query:

> What is Strategy's current posture?

More valuable implicit test:

> I want an agent to start implementing the Strategy schema next week. What should it work on first?

A good system must recognize that the premise itself conflicts with current Product posture.

## Retrieval vs answer quality

RAG evaluation work such as Ragas separates useful dimensions:

- **context precision** — relevant material should rank above noise;
- **context recall** — important supporting material should not be missed;
- **faithfulness** — answer claims should be supported by retrieved context.

The project should also measure source/walkback correctness and abstention.

## Proposed future cold-reconnect abilities

A first VedaOps evaluation suite should eventually include:

- static project state;
- dynamic project state/change detection;
- temporal reasoning;
- workflow recovery;
- known local gotchas;
- premise awareness;
- update/correction/supersession reasoning;
- abstention/unknown;
- cross-project composed questions;
- context/token/latency efficiency;
- correct escalation to live authority;
- provenance/walkback correctness.

Do not collapse these into one “brain score.” Different failure dimensions need different remediation.

## Sources

- LongMemEval-V2: https://arxiv.org/abs/2605.12493
- LOCOMO-CONV: https://arxiv.org/abs/2609.03467
- Ragas context precision: https://docs.ragas.io/en/latest/concepts/metrics/available_metrics/context_precision/
- Ragas context recall: https://github.com/vibrantlabsai/ragas/blob/main/docs/concepts/metrics/available_metrics/context_recall.md
- Ragas faithfulness: https://github.com/vibrantlabsai/ragas/blob/main/docs/concepts/metrics/available_metrics/faithfulness.md
