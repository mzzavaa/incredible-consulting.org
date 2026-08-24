---
title: "Retrieval Augmented Knowledge Base"
description: "A retrieval architecture that treats chunking, evaluation, and permissions as first-class design decisions."
weight: 20
draft: false
maturity: "stable"
clouds: ["AWS", "Azure", "GCP", "Cloud-neutral"]
c4_levels: ["Context", "Container", "Component"]
adr_count: 8
licence: "CC BY 4.0"
---

**Purpose.** The most requested pattern and the most often built badly. This entry exists to move the conversation from "which vector database" to "what does correct look like".

**Contains.**
- Ingestion pipeline diagram: source connectors, extraction, chunking, enrichment, indexing
- Permission-aware retrieval: filtering at query time versus index partitioning
- Evaluation design: retrieval metrics separated from generation metrics
- Freshness and reindexing strategy with cost implications
- Hybrid search configuration and when lexical search alone is enough
- When not to use this: small stable corpora, structured data better served by SQL

**Primary CTA.** Run the evaluation section against your existing retrieval setup.
**Links to.** /architectures/multi-agent-orchestration/, /playbooks/data-platform-foundations/, /checklists/ai-governance/.
