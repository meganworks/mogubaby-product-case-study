# Mogubaby | From Parenting Needs to a Shipped Product

**English** | [日本語](./README.ja.md)

### Start with the problem. Build only what helps solve it.

**Customer discovery · Product strategy · Requirements · AI-assisted delivery · Quality management**

[View Mogubaby on the App Store](https://apps.apple.com/jp/app/id6823474417)

## The opportunity: make everyday feeding decisions easier

Starting solid foods creates more work than preparing meals. Caregivers need to keep track of ingredients a baby has tried, recall when each food was last offered, and sometimes check food-exposure records for childcare enrollment. With notes, photos, product labels and daily routines scattered across different places, even answering **“When did we last have this?”** can take effort.

**What if recording a meal also made the next meal easier to plan?**

That question became **Mogubaby**, a baby-food tracking app for caregivers. It brings ingredient logging, packaged baby-food lookup, food history and childcare-preparation checks into a practical everyday experience.

**The objective was not to develop an app for its own sake. It was to reduce a recurring burden for caregivers—and use software and AI as the means to deliver that value.**

## Product at a glance

| | |
| --- | --- |
| **Product** | Baby-food and ingredient-tracking app for caregivers |
| **Platform** | iOS, available on the App Store |
| **Core experience** | Record foods and ingredients, review food history, see last recorded intake and elapsed days, sort ingredients, and check childcare-preparation records |
| **Additional experience** | Capture feeding milestones and memories |
| **My contribution** | Problem framing, product direction, requirements, UX and scope decisions, quality acceptance, release approval |
| **Delivery approach** | Claude Code for implementation, ChatGPT/Codex for separate review, GitHub Issues for requirement and decision tracking |

## What this project demonstrates

### 01. Customer discovery → Product direction

A recurring challenge is not simply recording food, but **making that record useful afterward**. Early feedback reinforced the need to see when an ingredient was last eaten. I translated that need into a focused set of features: last recorded intake, elapsed days and sorting—rather than adding a complex meal planner.

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

**My approach:** *Understand the problem first. Define the value. Use technology—including AI—to deliver the simplest useful solution.*

This repository contains a public account of product decisions and delivery practices, not the private application source code or private user information.
