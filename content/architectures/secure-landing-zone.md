---
title: "Secure Landing Zone"
description: "A multi-account baseline covering identity, network segmentation, logging, and guardrails before the first workload lands."
weight: 40
draft: false
maturity: "stable"
clouds: ["AWS", "Azure"]
c4_levels: ["Context", "Container"]
adr_count: 9
licence: "CC BY 4.0"
---

**Purpose.** For platform teams standing up a new cloud estate, and for auditors who need to see the control mapping. It is the foundation the other architectures assume.

**Contains.**
- Account and subscription topology with the reasoning for each boundary
- Identity model: workforce access, workload identity, and break-glass procedure
- Network segmentation baseline and egress control options
- Central logging, retention tiers, and the queries that make logs useful
- Preventive versus detective guardrails, with a sample policy set
- Control mapping table aligned to common audit frameworks
- When not to use this: single-team estates where the overhead exceeds the risk

**Primary CTA.** Run the control mapping against your existing estate and record the gaps.
**Links to.** /checklists/cloud-security-baseline/, /playbooks/legacy-to-cloud-migration/, /programmes/public-sector/.
