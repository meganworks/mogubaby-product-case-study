# Product Discovery & Requirements Translation

[Portfolio](../../README.md) · [日本語](../ja/product-discovery.md)

## The customer problem: ingredient checklists vs. meal reflection

Ingredient-introduction checklists are useful, but their information architecture and interaction patterns may not suit caregivers who need to revisit individual meals in detail. The opportunity concerns a particular set of user needs, not dissatisfaction across the entire market.

| Everyday task | Information or experience needed |
| --- | --- |
| Recreate a meal a baby enjoyed | Recall the meal and preparation method |
| Understand what was easier to eat | Note texture, consistency and feeding reactions |
| Review a day when symptoms appeared | Retrieve meal content and the baby's condition |
| Consider the next ingredient | Consult last recorded intake and elapsed days |

The design priorities are intuitive interaction, low recording friction, and retrieval by date and meal. These scenarios describe user needs, not a claim that every detail has a dedicated implemented field. Mogubaby combines ingredient logging, a diary and calendar, and ingredient history.

## From feedback to a focused feature

Early feedback suggested that showing when an ingredient was last consumed could make a food log more useful for everyday choices.

| Problem / insight | Product requirement |
| --- | --- |
| Hard to recall when an ingredient was last eaten | Show last recorded intake and elapsed calendar days |
| Difficult to identify foods not used recently | Sort by older/newer last recorded intake |
| Tracking spans different food groups | Preserve category-specific browsing while allowing sorting |
| Data may be edited, deleted or imported | Define what constitutes reliable intake history |
| Caregivers need quick answers | Favor a small, understandable enhancement over a new meal-planning engine |

The scope of this last-intake enhancement was **date visibility and sorting**, not automated meal plans, clinical nutritional guidance, allergy prevention, or food inventory tracking.

## Product judgment

A key distinction is between **a user's desired outcome** and **the smallest reliable capability** that supports it. A request to reduce meal-planning friction does not justify claiming to optimize nutrition or prescribe eating frequency.

The initial user input was qualitative and limited in sample size; this case does not claim measured improvements in diet, retention, or download conversion.

**Capabilities:** customer discovery, JTBD framing, prioritization, bounded requirements, responsible product claims.
