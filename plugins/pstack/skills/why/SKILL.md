---
name: why
description: "Use for why a system works this way, design rationale, regressions, postmortems, or data-backed thresholds. Traces commits, PRs, and related records to explain decisions and tradeoffs."
---

# Why

Answer from the record. Anchor the question in the affected symbols and paths, then trace the commits and PR discussions that introduced and changed them. Use ticket, document, chat, observability, error, and analytics sources when they can answer a part of the question. Record gaps where evidence is unavailable.

For questions with independent evidence sources, run one investigation per source in parallel. Route investigators and the synthesizer through `why investigators, synthesizer` per the [provider dispatch contract](../poteto-mode/references/provider-dispatch.md). Use the parent route so they can read the available MCPs. Give each the code anchor, question, its assigned source, and the [worker rules](../poteto-mode/worker.md). Investigators report author statements, inferences, and missing evidence separately with citations. The synthesizer spot-checks those citations. A narrow question with a clear written record needs only the parent’s direct read.

Cite what authors wrote, mark inferences as inferences, and state what the record does not answer. When the user is preparing a change, identify the constraints the evidence gives them.
