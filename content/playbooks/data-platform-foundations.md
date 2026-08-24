---
title: "Data Platform Foundations"
description: "The minimum viable data platform: ingestion, contracts, quality gates, and access control that survive the first three teams."
weight: 40
draft: false
version: "1.2"
maturity: "reviewed"
domain: "Data"
effort: "6 to 12 weeks"
licence: "CC BY 4.0"
deliverables: ["Data contract spec", "Quality gate set", "Access model", "Domain onboarding guide"]
---

**Purpose.** For organisations building their second data platform because the first one became a swamp. It focuses on the contracts and guardrails, not on tool selection.

**Contains.**
- Scope boundary: what belongs in the platform and what belongs to the domain team
- Data contract specification with schema, freshness, ownership, and breaking-change policy
- Quality gate set: the five checks that catch most incidents
- Access model mapping business roles to storage and compute permissions
- Domain onboarding guide, the self-service path from request to first table
- Tool-agnostic reference mapping so the playbook survives a vendor change

**Primary CTA.** Write one data contract for your busiest table and enforce it.
**Links to.** /architectures/serverless-data-platform/, /glossary/cloud-and-platform/, /playbooks/ai-readiness-assessment/.
