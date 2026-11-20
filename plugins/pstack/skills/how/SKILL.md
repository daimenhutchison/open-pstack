---
name: how
description: "Use for \"how does X work\", code walkthroughs before changing something, and placement / ownership / layering questions (\"where should this live\", \"which package owns this\", \"is this the right layer\"). Explains subsystem architecture, runtime flow, onboarding mental models. Use why for motivation."
---

# How

Explain how the subsystem works to a senior engineer who will work on it. State your interpretation if the target is ambiguous.

Route each lane through [provider dispatch](../poteto-mode/references/provider-dispatch.md), using `read-only` access and the configured role or its [default](../poteto-mode/references/model-catalog.md#role-defaults). Start each kickoff with the [worker rules](../poteto-mode/worker.md).

For a narrow question, dispatch one `how explainer` to explore and explain. For a cross-cutting question, dispatch two to four `how explorer` lanes in parallel with distinct scopes, then give their findings to one `how explainer`. Ask for the key concepts, runtime flow, code locations, and gotchas, with source pointers. Present the explanation with only edits for clarity or context.
