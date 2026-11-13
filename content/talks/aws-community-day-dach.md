---
title: "AWS Community Day DACH"
description: "The German-speaking community day in Munich, twice. I also co-organise this one."
weight: 220
draft: false
eyebrow: "2025 · Munich"
session: "From MacBook to Bedrock"
source_url: "https://www.lindamohamed.com/aws-community-day-dach"
licence: "Free to read, use and share with credit"
---

- [aws-community-day.de](https://www.aws-community-day.de/)

## On the programme

### From MacBook to Bedrock

*2025 · Munich*

The OTTO build and what it taught us about fine-tuning, retrieval and cost.

- Slides coming soon
- [Read the recap](https://www.lindamohamed.com/blog/aws-community-day-dach-munich-2025)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

### Workshop: Women in Cloud

*2024 · Munich*

A hands-on Women in Cloud workshop, run together with Meyyar Palaniappan from the AWS user group in Munich and Sana Shah from the AWS Women's user group in Berlin.

- No slides for this one
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

## The women of the DACH community

[Open the original post on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7304111265197494272)

From the Förderverein AWS Community DACH e.V., celebrating the women of the AWS community in DACH. Shown here as the original LinkedIn post, not a copy.

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

### [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)

The longer write-up: the build, the services and what it costs to run.

### [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

The longer write-up: the build, the services and what it costs to run.

## The same talk, other stages

Same session, a different room. Each page carries its own deck.

- [AWS re:Invent](/talks/aws-reinvent/)
- [AWS Community Day Slovakia](/talks/aws-community-day-slovakia/)
- [AWS Community Day Czech Republic](/talks/aws-community-day-czech-republic/)
- [AWS Community Day Romania](/talks/aws-community-day-romania/)
- [AWS Community Day Italy](/talks/aws-community-day-italy/)
- [AWS Community Day Poland](/talks/aws-community-day-poland/)
- [CTRL+ESC Malta](/talks/ctrl-esc-malta/)
- [AWS Student Builder Group St. Pölten](/talks/aws-student-builder-group-st-poelten/)
- [Cloud Day FH Burgenland](/talks/cloud-day-fh-burgenland/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [Recap: From MacBook to Bedrock, 2025](https://www.lindamohamed.com/blog/aws-community-day-dach-munich-2025)
- [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)
- [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)
- [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)
- [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-community-day-dach), where it was first published.
