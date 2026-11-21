# Requirements Management & AI-Assisted Delivery

[Portfolio](../../README.md) · [日本語](../ja/delivery-governance.md)

## Requirements as the working source of truth

The implementation workflow treated GitHub Issues as the latest reference for **scope, decisions, acceptance conditions, and review requests**. When feedback changed product positioning, the current issue specification was revised explicitly and superseded earlier proposals while preserving decision history.

The point was not to build an elaborate governance layer around a small app. It was to reduce ambiguity when multiple AI assistants worked on related tasks.

## Responsibility split

| Participant | Documented responsibility |
| --- | --- |
| Human product owner | Define outcomes, choose scope, judge UX and claims, authorize release |
| Claude Code | Implement changes, create assets, propose fixes, report test outcomes |
| ChatGPT/Codex | Review independently from a different model/provider perspective, identify gaps and boundary cases |
| GitHub Issues | Preserve current requirements, review history, decisions, and follow-ups |
| CI / test tools | Execute release-candidate checks; distinguish passed runs from reports or assumptions |

## Example: coordinated changes

A food-history feature and revised App Store presentation were intentionally coupled: promotional screenshots had to depict real functionality available in the same version. This reduced the risk of advertising functionality before users could obtain it.

AI did not independently choose the product strategy or receive blanket authority to publish. Final user-facing decisions and release authorization remained with the human owner.

## Honest limits

This project did **not** implement a formal enterprise SDLC, exhaustive accessibility coverage, or universal test automation. Some checks relied on reported results and hands-on device inspection. The value demonstrated is pragmatic ownership, traceability, and risk-aware review.

**Capabilities:** requirements governance, delivery coordination, AI orchestration, scope control, accountable sign-off.
