---
title: "Serverless Data Platform"
description: "An event-driven ingestion and analytics platform sized for teams that cannot staff a platform team."
weight: 30
draft: false
maturity: "reviewed"
clouds: ["AWS", "Cloud-neutral"]
c4_levels: ["Context", "Container"]
adr_count: 5
licence: "CC BY 4.0"
---

**Purpose.** For small and mid-sized organisations that need a real data platform without a dedicated operations rota. Optimised for low idle cost and few moving parts.

**Contains.**
- Container diagram: ingestion, raw and curated zones, transformation, serving layer
- Scale-to-zero reasoning and the latency cost it buys
- Schema evolution handling in an append-only landing zone
- Orchestration choice with the failure and retry semantics spelled out
- Cost curve showing where this pattern stops being cheaper than a managed warehouse
- When not to use this: sustained high throughput, sub-second query requirements

**Primary CTA.** Compare your current idle spend against the cost curve.
**Links to.** /playbooks/data-platform-foundations/, /playbooks/cloud-cost-baseline/, /glossary/cloud-and-platform/.
