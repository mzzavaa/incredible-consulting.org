---
title: "Agentic Systems in Production"
description: "How to take a multi-agent prototype from a laptop demo to a system that can be operated, observed, and paid for."
weight: 20
draft: false
version: "1.4"
maturity: "reviewed"
domain: "AI"
effort: "4 to 8 weeks, small team"
licence: "CC BY 4.0"
deliverables: ["Operating model", "Evaluation harness", "Cost model", "Runbook"]
---

**Purpose.** Most agent projects die between the demo and the on-call rota. This playbook covers only that gap, for engineering teams who already have something that works once.

**Contains.**
- Definition of done for an agentic system, stated as operational criteria not demo criteria
- Evaluation harness: golden set construction, regression gates, and human review sampling
- Failure taxonomy: tool errors, loop escapes, silent degradation, prompt drift
- Cost model per request, with token, tool call, and retry accounting
- Observability requirements: trace shape, span naming, and what to alert on
- Human-in-the-loop patterns and when to remove the human
- Runbook template covering rollback, model pinning, and incident triage

**Primary CTA.** Build the evaluation harness before the next feature.
**Links to.** /architectures/multi-agent-orchestration/, /checklists/production-readiness/, /glossary/ai-and-agents/.
