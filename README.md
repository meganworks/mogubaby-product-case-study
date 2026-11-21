# Mogubaby | From Food Logs to Everyday Feeding Decisions

**English** | [日本語](./README.ja.md)

### Remember what was served, learn from past meals, and make the next feeding decision easier

**Customer discovery · Product strategy · Requirements · AI-assisted delivery · Quality management**

[View Mogubaby on the App Store](https://apps.apple.com/jp/app/id6823474417)

## The opportunity: from ingredient tracking to meal management

Existing baby-food apps are useful for tracking ingredient introductions and feeding progression. However, an interface centered on ingredient checklists can be a poor fit for caregivers who need to record and revisit everyday feeding experiences in more detail.

- Recreate a meal that a baby particularly enjoyed.
- Recall which texture or consistency was easier to eat.
- Review food consumed and how the baby was feeling on a day when symptoms appeared.
- Find ingredients that have not been eaten recently when considering the next meal.

These tasks call for more than an ingredient checklist. Caregivers need an intuitive way to record and retrieve information by date and meal, including context that may matter for future decisions.

**From ingredient tracking to meal management.**

Mogubaby was conceived around that need, with an emphasis on ease of recording and retrieval. It combines ingredient logging, packaged baby-food lookup, a diary and calendar, and ingredient history to support both meal reflection and food tracking.

## Product at a glance

| | |
| --- | --- |
| **Product** | Baby-food and ingredient-tracking app for caregivers |
| **Platform** | iOS, available on the App Store |
| **Core experience** | Record foods and ingredients, review food history, see last recorded intake and elapsed days, sort ingredients, and check childcare-preparation records |
| **Additional experience** | Diary and calendar, feeding milestones and memories |
| **My contribution** | Problem framing, product direction, requirements, UX and scope decisions, quality acceptance, release approval |
| **Delivery approach** | Claude Code for implementation, ChatGPT/Codex for separate review, GitHub Issues for requirement and decision tracking |

## What this project demonstrates

### 01. Customer discovery → Product direction

I focused on the gap between ingredient-centered tracking and meal-centered reflection, treating ease of recording and information retrieval as design priorities. Early feedback then reinforced the need for last-recorded intake dates, elapsed days and sorting, which became a focused feature enhancement.

[Explore product discovery →](./docs/en/product-discovery.md)

### 02. Product leadership → Clearer everyday value

The initial App Store story emphasized childcare preparation. Feedback revealed a broader, more frequent use case: everyday food choices. I reorganized the product message around **easy logging → useful food history → childcare preparation**, while preserving the value of milestone sharing.

[Explore product positioning →](./docs/en/product-and-launch.md)

### 03. AI orchestration → Accountable execution

I led scope and product decisions while Claude Code supported implementation and ChatGPT/Codex provided a separate review perspective. GitHub Issues connected the current requirements, decisions, review findings and changes.

[Explore the delivery model →](./docs/en/delivery-governance.md)

### 04. Quality management → A more trustworthy product

Independent review caught an important distinction: an imported **first-ever consumption date** is not necessarily the **latest confirmed intake date**. That finding prompted a targeted implementation correction and additional regression coverage before release.

[Explore the quality case study →](./docs/en/quality-management.md)

## From insight to release

```text
Everyday caregiver problem
            ↓
Define the outcome that matters [Human]
            ↓
Prioritize a focused product response [Human]
            ↓
Document requirements and decisions [GitHub Issues]
            ↓
Implement and validate changes [Claude Code]
            ↓
Review independently and correct issues [ChatGPT/Codex + Claude Code]
            ↓
Accept the experience and authorize release [Human]
            ↓
App Store publication
```

Version **1.0.1**, including improvements to food-history visibility and App Store presentation, was published in October 2026. This is a product-and-delivery case study, not a claim of measured nutrition, conversion or retention improvements.

## Tools and methods

**Product:** Customer insight, requirements translation, prioritization, UX decisions, product positioning  
**Delivery:** GitHub Issues, AI-assisted implementation, independent review, regression checks, release approval  
**AI:** Claude Code, ChatGPT/Codex

## Case studies

| Detailed case | Focus |
| --- | --- |
| [Product discovery & requirements](./docs/en/product-discovery.md) | Turn a caregiver problem into a focused capability |
| [Product positioning & launch](./docs/en/product-and-launch.md) | Communicate the value and coordinate release |
| [AI-assisted delivery governance](./docs/en/delivery-governance.md) | Human accountability and requirements traceability |
| [Quality management](./docs/en/quality-management.md) | Independent review, edge cases and correction |

---

This repository contains a public account of product decisions and delivery practices, not the private application source code or private user information.
