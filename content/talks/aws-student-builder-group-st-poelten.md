---
title: "AWS Student Builder Group St. Pölten"
description: "Austria's only AWS Student Builder Group, run by students out of the University of Applied Sciences St. Pölten."
weight: 150
draft: false
eyebrow: "2026 · St. Pölten"
session: "Hybrid AI Architecture"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/aws-student-builder-group-st-poelten"
licence: "Free to read, use and share with credit"
---

- [the group on Meetup](https://www.meetup.com/aws-sbg-at-university-of-applied-sciences-st-polten/)

## On the programme

### Hybrid AI Architecture

*2026 · St. Pölten*

What actually happens when you wire local servers to the cloud: where the data has to stay, what each answer costs, and which of those two decides the architecture. Four ways to draw the same system, then three real projects on the layer their constraints forced.

- [Download the slides](https://drive.google.com/file/d/11DFmGg-6DV9Zw_YkIPhSRBejTj79gpQp/view)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

### OTTO: demo and presentation

*2026 · St. Pölten*

The multi-agent assistant, demonstrated and taken apart for the Cloud Club earlier in the year.

- [Download the slides](https://drive.google.com/file/d/1GsmZFeeHxM1WE7x5zLk66nRyZ62ESbs0/view)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

From the deck

## Five slides, straight from the talks

![Four ways to run one task](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/dfb6da2-3f84-520-7335-ac60b2bbc8_stpoelten-hybrid-1.jpg)

Hybrid AI architecture: the same invoice job, four architectures. Slide from the deck.

![Two grounds under one operating model](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/4c6b221-8f3c-7a51-7c27-db7e314e06d_stpoelten-hybrid-2.jpg)

What hybrid actually means: Bedrock in the Region, vLLM on OpenShift AI inside the building. Slide from the deck.

![Three real systems](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/72ae84-f663-fdcb-d8c6-4bd33b31b70_stpoelten-hybrid-3.jpg)

The video pipeline, the event assistant and the geospatial platform, side by side. Slide from the deck.

![The OTTO agent crew](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/bf3d0cc-5dc3-e511-babe-dc6b577126b_stpoelten-otto-1.jpg)

From MacBook to Bedrock: the agents and the models behind them. Slide from the deck.

![Inference on Bedrock and App Runner](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/4ccebfb-c303-757-c441-77e3ed4452ab_stpoelten-otto-2.jpg)

Where the fine-tuned model runs, and what it costs. Slide from the deck.

## The services doing the work

Read off the slides, not guessed. Each card says what that service did in this build, and links to the page explaining the capability and how to run it somewhere else.

### Amazon Textract

The ready-made column in the invoice example: it returns the fields and you write the glue code, nothing else.

- [Reading documents](https://www.lindamohamed.com/document-ocr-text-extraction)

### Amazon Bedrock

The ask-a-model column, and the regional half of the hybrid picture: one endpoint, one log, paid per token.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Amazon SageMaker AI

The train-your-own column: the same invoices, your model, behind your own endpoint.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### Red Hat OpenShift AI

The run-the-platform-yourself column, and the ground inside the building in the hybrid split.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### vLLM

Serves the model inside the building, for the data that may not leave it.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### Amazon Bedrock AgentCore

Lets the agent reach on-premises data and tools while the inference stays in the Region. Only the agent crosses the line.

- [AI agents](https://www.lindamohamed.com/ai-agents-runtime)

### Amazon Bedrock Custom Model Import

System two: a 3B model tuned once on a rented GPU, then served managed. About 30 a month, almost all of it idle.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### Amazon Rekognition

In the video pipeline: faces, shots and what is on screen.

- [Image recognition](https://www.lindamohamed.com/image-recognition-object-detection)

### Amazon Transcribe

The words, and when each one was said.

- [Speech to text](https://www.lindamohamed.com/speech-to-text-transcription)

### AWS Step Functions

Remembers where a long job got to, so a three-hour render survives a failure.

- [Workflow orchestration](https://www.lindamohamed.com/workflow-orchestration)

### AWS Elemental MediaConvert

Renders the versions each platform wants.

- [Video rendering in code](https://www.lindamohamed.com/video-rendering-in-code)

### Amazon API Gateway

In the geospatial platform: one front door, one audit trail, a key per tenant.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### Amazon RDS

PostGIS on RDS holds the open spatial data in the cloud half. The survey and CAD files stay in an internal PostGIS.

### AWS CloudTrail

Who called what, agents included, across two organisations operating two halves.

### AWS IAM

A role per tenant, one identity each, nothing shared between customers.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### InstructLab

The open-source pipeline behind the fine-tune: documents become Q&A pairs in YAML, synthetic data is generated from them, then the adapter is trained with LoRA. Model-agnostic, and it ran on a laptop.

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

## The longer write-ups

Where the builds behind these sessions are explained properly.

### [AI Architecture Layers: where a workload actually belongs](https://www.lindamohamed.com/ai-architecture-layers)

The longer write-up: the build, the services and what it costs to run.

### [Open-Source AI Wiki: Why I Built AI Solutions Wiki](https://www.lindamohamed.com/blog/free-open-source-ai-wiki)

The longer write-up: the build, the services and what it costs to run.

### [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)

The longer write-up: the build, the services and what it costs to run.

### [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)

The longer write-up: the build, the services and what it costs to run.

### [Cloud Day | FH Burgenland](https://www.lindamohamed.com/blog/cloud-day-fh-burgenland-2026)

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
- [Cloud Day FH Burgenland](/talks/cloud-day-fh-burgenland/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [the group on Meetup, the event's own site](https://www.meetup.com/aws-sbg-at-university-of-applied-sciences-st-polten/)
- [Slides: Hybrid AI Architecture, 2026](https://drive.google.com/file/d/11DFmGg-6DV9Zw_YkIPhSRBejTj79gpQp/view)
- [Slides: OTTO: demo and presentation, 2026](https://drive.google.com/file/d/1GsmZFeeHxM1WE7x5zLk66nRyZ62ESbs0/view)
- [AI Architecture Layers: where a workload actually belongs](https://www.lindamohamed.com/ai-architecture-layers)
- [Open-Source AI Wiki: Why I Built AI Solutions Wiki](https://www.lindamohamed.com/blog/free-open-source-ai-wiki)
- [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)
- [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)
- [Cloud Day | FH Burgenland](https://www.lindamohamed.com/blog/cloud-day-fh-burgenland-2026)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-student-builder-group-st-poelten), where it was first published.
