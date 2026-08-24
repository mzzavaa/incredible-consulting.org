---
title: "Multi-Agent Orchestration"
description: "A reference pattern for routing work across specialised agents with bounded autonomy and traceable decisions."
weight: 10
draft: false
maturity: "reviewed"
clouds: ["AWS", "Azure", "Cloud-neutral"]
c4_levels: ["Context", "Container"]
adr_count: 6
licence: "CC BY 4.0"
---

**Purpose.** For teams moving past a single prompt-and-response service into orchestrated agents, and needing to explain the blast radius to a risk function.

**Contains.**
- Context and container diagrams showing orchestrator, specialist agents, tool layer, and memory
- Routing strategies compared: static, model-selected, and rules-plus-model
- Bounded autonomy: budget caps, tool allowlists, and escalation triggers
- State and memory options with their consistency and privacy trade-offs
- Six architecture decision records covering model choice, retry policy, and trace format
- When not to use this: single-step tasks, hard latency ceilings, unclear ownership of tool side effects

**Primary CTA.** Copy the ADR set and adapt the six decisions to your context.
**Links to.** /playbooks/agentic-systems-in-production/, /architectures/retrieval-augmented-knowledge-base/, /glossary/ai-and-agents/.
