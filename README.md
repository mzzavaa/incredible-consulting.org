# incredible-consulting.org: Open Methodology & Public Good

**Domain:** incredible-consulting.org
**Role:** Open methodology · Public-good arm of the consulting practice
**Priority:** Phase 2
**Strategy doc:** internal, not linked from here

## Purpose
The non-commercial counterpart to incredible-consulting.com. It publishes the frameworks, playbooks,
checklists, reference architectures, and research that the commercial arm actually uses, openly and for
free. No gated downloads, no sales pitch on the page. Authority is built by giving the method away, and
inbound demand for the commercial arm follows from that rather than from a call to action.

## Key Features / Sections
- Open playbook library, versioned and licensed for reuse including commercial reuse
- Reference architectures with decision records and a mandatory "when not to use this" section
- The three-workshop method, documented end to end so others can run it without us
- Printable and machine-readable checklists for go-live, governance, and security reviews
- Research programme with published methods, raw data, and disclosed funding
- Glossary for mixed business and engineering audiences
- Licensing and attribution terms in plain language
- Contribution process, writing style, and named maintainers
- Pro bono, non-profit, and public sector programmes with published selection criteria

## Monetization
Indirect. Authority and inbound demand feeding incredible-consulting.com. Optional sponsorship or grant
funding for the research programme only, under published independence rules that keep funders away from
questions, analysis, and findings. Nothing on this site is a teaser for a paid version.

## Content map

```
content/
  _index.md                                 Homepage
  playbooks/                                Open playbook library (data/playbooks.yaml)
    _index.md
    ai-readiness-assessment.md
    agentic-systems-in-production.md
    cloud-cost-baseline.md
    data-platform-foundations.md
    legacy-to-cloud-migration.md
  architectures/                            Reference architectures (data/architectures.yaml)
    _index.md
    multi-agent-orchestration.md
    retrieval-augmented-knowledge-base.md
    serverless-data-platform.md
    secure-landing-zone.md
  method/                                   The three-workshop method
    _index.md
    three-workshop-method.md
    workshop-one-discovery.md
    workshop-two-architecture.md
    workshop-three-decision.md
    facilitation-kit.md
  checklists/                               Gates and review lists (data/checklists.yaml)
    _index.md
    production-readiness.md
    ai-governance.md
    cloud-security-baseline.md
  research/                                 Research programme (data/research.yaml)
    _index.md
    reports.md
    open-datasets.md
    take-part.md
    funding-and-sponsorship.md
  glossary/                                 Shared vocabulary
    _index.md
    ai-and-agents.md
    cloud-and-platform.md
  licensing/                                Reuse terms
    _index.md
    reuse-terms.md
    attribution-and-trademark.md
  contribute/                               How to contribute
    _index.md
    contribution-guide.md
    writing-style.md
    review-process.md
    maintainers.md
  programmes/                               Pro bono and public good
    _index.md
    pro-bono.md
    non-profit-and-ngo.md
    public-sector.md
    apply.md
  about/                                    Who, why, and how it is funded
    _index.md
    why-open.md
    how-this-is-funded.md
    changelog.md

data/
  playbooks.yaml                            Playbook collection schema, 3 seeded entries
  architectures.yaml                        Reference architecture schema, 3 seeded entries
  checklists.yaml                           Checklist schema, 3 seeded entries
  research.yaml                             Research programme schema, 3 seeded entries
```

10 top level sections · 47 markdown files · 4 data collections.

## Relationship to other Incredible domains

| Domain | Relationship |
| --- | --- |
| incredible-company.com | Parent umbrella brand. Linked from the footer and the about section as the group entity. |
| incredible-consulting.com | The commercial arm and the canonical consulting domain. This site never sells, it hands off. Paid delivery, rates, and engagement enquiries all live there. |
| incredibleconsulting.org | Defensive typo-catch domain. It keeps a four-page signpost, 301s every deep path to incredible-consulting.com as the canonical consulting domain, and offers a route card to this site for visitors who meant the open methodology. Nothing here links to it. |
| incredible.builders | Practitioner and open source community. Contribution discussion, code, and hands-on building live there. This site links out for the conversation and keeps the finished artefacts. |
| incredible.community | People, events, and membership. Clinics, meetups, and the human layer around the programmes are hosted there rather than duplicated here. |
| incredible.training | Commercial learning and enablement. This site publishes the facilitation kit for free, the training domain sells certified delivery and instructor-led courses on top of it. |

**Lane discipline.** This domain publishes method and evidence. It does not price work, run events,
host community discussion, or sell courses. Where a visitor needs one of those, the page links out.

## Local development

```
make dev      # hugo server on the first free port from 1313
make build    # hugo --gc --minify
make clean    # remove public, resources/_gen, .hugo_build.lock
```

## House style
No em-dashes. No emojis. Middle dots are fine as separators. Direct, concrete, practitioner-level voice.
Brand palette: green #3D8F37 · dark #0a1a08 · white #fff · background #f8f9f6. Typeface: Inter.
Theming is a later pass, `layouts/` and `static/` are intentionally empty.
