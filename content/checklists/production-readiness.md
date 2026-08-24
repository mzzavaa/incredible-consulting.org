---
title: "Production Readiness"
description: "Forty-two checks across reliability, observability, security, and cost that a service should pass before it carries real traffic."
weight: 10
draft: false
item_count: 42
review_stage: "Pre go-live"
formats: ["Markdown", "PDF", "YAML"]
licence: "CC BY 4.0"
---

**Purpose.** A gate for engineering leads and on-call teams. It is deliberately opinionated so that an exception has to be argued rather than assumed.

**Contains.**
- Six sections: reliability, observability, security, data, cost, and operability
- Each item written as a testable statement with a pass condition
- Severity marking so a team can agree a minimum bar for lower environments
- Exception register template with expiry dates
- Machine-readable YAML variant for pipeline enforcement
- Notes on adapting the list for AI and agentic services

**Primary CTA.** Run the checklist and record every exception with an owner and an expiry.
**Links to.** /playbooks/agentic-systems-in-production/, /checklists/cloud-security-baseline/, /architectures/.
