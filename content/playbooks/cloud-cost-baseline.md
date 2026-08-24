---
title: "Cloud Cost Baseline"
description: "Establish a defensible cost baseline in ten working days, then cut the obvious waste without touching architecture."
weight: 30
draft: false
version: "3.0"
maturity: "stable"
domain: "Cost"
effort: "10 days, 1 engineer part-time"
licence: "CC BY 4.0"
deliverables: ["Tagged cost baseline", "Waste register", "Unit cost metric", "90 day plan"]
---

**Purpose.** For platform owners who cannot answer "what does this service cost us per customer". It is deliberately architecture-neutral so it works before any redesign.

**Contains.**
- Tagging and allocation model, including how to handle shared and untaggable spend
- Unit cost metric selection: choosing a denominator finance and engineering both accept
- Waste register: idle capacity, orphaned storage, over-provisioned instances, forgotten environments
- Commitment strategy decision tree (on demand, savings plans, reserved, spot)
- Reporting cadence and who owns each number
- Anti-patterns: chasing percentage savings without a denominator, cost dashboards nobody opens

**Primary CTA.** Publish the first unit cost metric and defend it in one review.
**Links to.** /architectures/secure-landing-zone/, /checklists/production-readiness/, /method/.
