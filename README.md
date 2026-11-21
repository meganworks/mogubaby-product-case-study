# Mogubaby | AI-Assisted Product Ownership & Delivery Governance

**English** | [日本語](./README.ja.md)

### From a common parenting challenge to a shipped product — with human-led decisions and complementary AI agents

**Customer insight · Requirements management · Product strategy · Independent review · Release governance**

[View Mogubaby on the App Store](https://apps.apple.com/jp/app/id6823474417)

## The opportunity

Introducing solid foods creates a recurring information-management challenge for caregivers. They need to remember which ingredients a baby has tried, identify what was eaten recently, record ingredients in packaged baby foods, and sometimes prepare food-exposure information requested by childcare providers. These small tasks accumulate during already busy routines.

**What if a food log could support the next practical decision—not just preserve a record?**

Mogubaby is an independently launched Japanese-language baby-food tracking application. It helps caregivers record foods, review ingredient history, check relevant childcare-preparation information, and preserve everyday milestones.

This portfolio describes the **product and delivery decisions**, not the private production source code.

## Product at a glance

| | |
| --- | --- |
| **Product** | Baby-food and ingredient-tracking app |
| **Platform** | iOS; published on the App Store |
| **Example capabilities** | Ingredient logging, packaged-food lookup, food history, last recorded intake and elapsed days, food-list sorting, childcare-preparation tracking, milestones |
| **My role** | Independent product owner: problem framing, requirements, UX and positioning decisions, acceptance and release authorization |
| **Delivery model** | Claude Code for implementation; ChatGPT/Codex for a separate review perspective; GitHub Issues for requirements and decision history |
| **Documented release** | Version 1.0.1, published in October 2026 |

## Four cases demonstrating product ownership

### 01. Customer insight → Prioritized requirements

Early feedback highlighted a common frustration: caregivers could log foods but still struggled to remember **when an ingredient had last been eaten**. I translated that into a focused change: last-recorded intake, elapsed days, and sorting—not a broad meal-planning or clinical advice feature.

[Product discovery and requirements →](./docs/en/product-discovery.md)

### 02. A single source of truth → Delivery alignment

GitHub Issues held current scope, acceptance expectations, constraints, decisions and review follow-ups. As new feedback emerged, the product priorities were explicitly revised rather than silently expanding the feature set.

[Requirements and delivery model →](./docs/en/delivery-governance.md)

### 03. Independent AI review → Corrective action

Separating implementation and review proved useful. A review identified a subtle data-semantic risk: an imported **first-ever consumption date** must not automatically be treated as the **most recent confirmed intake**. The resulting fix and regression checks preserved that distinction.

[Quality management case study →](./docs/en/quality-management.md)

### 04. Product positioning → Coordinated release

Feedback also reshaped the product story for the App Store: **make logging easy → make food history useful for daily decisions → support childcare preparation**. Revised store assets and the food-history enhancement were coordinated into the 1.0.1 release.

[Product positioning and release →](./docs/en/product-and-launch.md)

## Human-led AI delivery

```text
Common caregiver need / initial product hypothesis
                    ↓
Problem framing, scope and priorities [Human product owner]
                    ↓
Requirements and decision history [GitHub Issues]
                    ↓
Implementation and checks [Claude Code]
                    ↓
Separate code / design review [ChatGPT / Codex]
                    ↓
Targeted remediation and regression checks [Claude Code]
                    ↓
UX acceptance and release authorization [Human product owner]
                    ↓
App Store submission and publication
```

This is a description of a documented working pattern—not a claim that AI was fully autonomous or that all testing was independently executed.

## What the project demonstrates

**Customer-to-requirement translation · Scope control · Traceability · Cross-model review · Edge-case analysis · Product positioning · Human-in-the-loop release decisions**

**Evidence boundary:** The detailed development repository is private. This public case study uses only generalized product problems, independently authored summaries, and publicly available app information. It intentionally excludes personal/family details, verbatim private feedback, production source code, credentials, and private development links. The test results discussed in the case studies apply to specific release-candidate workflows, not a blanket guarantee of product quality.

---

[日本語版を読む](./README.ja.md) · [App Store](https://apps.apple.com/jp/app/id6823474417)
