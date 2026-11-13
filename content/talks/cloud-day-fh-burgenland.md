---
title: "Cloud Day FH Burgenland"
description: "A free one-day public tech event at Hochschule Burgenland in Eisenstadt, where I also lecture."
weight: 200
draft: false
eyebrow: "2026 · Eisenstadt"
session: "Multi-Agent Systems on AWS: From Prototype to Production"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/cloud-day-fh-burgenland"
licence: "Free to read, use and share with credit"
---

- [cloud-day.hochschule-burgenland.at](https://cloud-day.hochschule-burgenland.at/2026/)

## On the programme

### Multi-Agent Systems on AWS: From Prototype to Production

*2026 · Eisenstadt*

Using OTTO to show how teams move a multi-agent system from a working demo to something they can actually operate.

- [Download the slides](https://drive.google.com/file/d/17CYmFtwZ8zB_2JmwJ25xgHJFie74s8zo/view)
- [Read the recap](https://www.lindamohamed.com/blog/cloud-day-fh-burgenland-2026)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

## The day itself, in their words

[Open the original post on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7424443059746144257)

The official recap from Igor Ivkic, who runs the Cloud Computing Engineering master at Hochschule Burgenland. His post carries the photos from the day. Shown here as the original LinkedIn post, not a copy.

## The services doing the work

Read off the slides, not guessed. Each card says what that service did in this build, and links to the page explaining the capability and how to run it somewhere else.

### InstructLab

The open-source pipeline behind the fine-tune: documents become Q&A pairs in YAML, synthetic data is generated from them, then the adapter is trained with LoRA. Model-agnostic, and it ran on a laptop.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### Amazon Bedrock

The workstation. Claude Sonnet 3.7, Amazon Nova Pro and the custom model are all served from one place.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Amazon Bedrock Custom Model Import

Serves the fine-tuned Llama 3.1 3B as the UG Specialist, so the trained model needs no cluster of its own.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### CrewAI

Runs the crew: Q&A agent, agenda producer, header generator, speaker finder, GitHub planner and the UG Specialist.

- [AI agents](https://www.lindamohamed.com/ai-agents-runtime)

### AWS App Runner

Runs the agent container. The whole system came to about 30 euros a month.

- [Serverless compute](https://www.lindamohamed.com/serverless-compute)

### Amazon ECR

Holds the container image App Runner pulls.

- [Object storage](https://www.lindamohamed.com/object-storage)

### Amazon S3

Stores the trained model before Bedrock imports it.

- [Object storage](https://www.lindamohamed.com/object-storage)

### Llama 3.1 3B

The open-weights base model that became the UG Specialist, adapted with LoRA rather than retrained.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### Amazon Nova Pro

The agent model, and the teacher that generated the synthetic training data.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Claude Sonnet 3.7

Answers the open questions in the Q&A agent.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Red Hat OpenShift AI

The alternative to training on a Mac: the same run as a Jupyter environment or an OpenShift pipeline.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

## The longer write-ups

Where the builds behind these sessions are explained properly.

### [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)

The longer write-up: the build, the services and what it costs to run.

### [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)

The longer write-up: the build, the services and what it costs to run.

### [Cloud Day | FH Burgenland](https://www.lindamohamed.com/blog/cloud-day-fh-burgenland-2026)

The longer write-up: the build, the services and what it costs to run.

### [Open-Source AI Wiki: Why I Built AI Solutions Wiki](https://www.lindamohamed.com/blog/free-open-source-ai-wiki)

The longer write-up: the build, the services and what it costs to run.

## The same talk, other stages

Same session, a different room. Each page carries its own deck.

- [AWS re:Invent](/talks/aws-reinvent/)
- [AWS Community Day DACH](/talks/aws-community-day-dach/)
- [AWS Community Day Slovakia](/talks/aws-community-day-slovakia/)
- [AWS Community Day Czech Republic](/talks/aws-community-day-czech-republic/)
- [AWS Community Day Romania](/talks/aws-community-day-romania/)
- [AWS Community Day Italy](/talks/aws-community-day-italy/)
- [AWS Community Day Poland](/talks/aws-community-day-poland/)
- [CTRL+ESC Malta](/talks/ctrl-esc-malta/)
- [AWS Student Builder Group St. Pölten](/talks/aws-student-builder-group-st-poelten/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [cloud-day.hochschule-burgenland.at, the event's own site](https://cloud-day.hochschule-burgenland.at/2026/)
- [Slides: Multi-Agent Systems on AWS: From Prototype to Production, 2026](https://drive.google.com/file/d/17CYmFtwZ8zB_2JmwJ25xgHJFie74s8zo/view)
- [Recap: Multi-Agent Systems on AWS: From Prototype to Production, 2026](https://www.lindamohamed.com/blog/cloud-day-fh-burgenland-2026)
- [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)
- [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)
- [Cloud Day | FH Burgenland](https://www.lindamohamed.com/blog/cloud-day-fh-burgenland-2026)
- [Open-Source AI Wiki: Why I Built AI Solutions Wiki](https://www.lindamohamed.com/blog/free-open-source-ai-wiki)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/cloud-day-fh-burgenland), where it was first published.
