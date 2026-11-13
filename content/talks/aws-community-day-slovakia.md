---
title: "AWS Community Day Slovakia"
description: "The first edition of AWS Community Day Slovakia, in Košice."
weight: 280
draft: false
eyebrow: "2025 · Košice"
session: "From MacBook to Bedrock: Lessons from Building an AI Assistant"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/aws-community-day-slovakia"
licence: "Free to read, use and share with credit"
---

- [awscommunityday.sk](https://www.awscommunityday.sk/)

## On the programme

### From MacBook to Bedrock: Lessons from Building an AI Assistant

*2025 · Košice*

With Philipp Bergsmann. Training an AI-powered Slackbot with InstructLab and deploying it on Amazon Bedrock, and the real bottlenecks: slow training on laptops, inconsistent retrieval, and debugging.

- [Download the slides](https://drive.google.com/file/d/1tap3GgiOqxxp5nO-w7wEzGQQoj3UUBvD/view)
- [Read the recap](https://www.lindamohamed.com/blog/aws-community-day-slovakia-kosice-2025)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

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

## Slides from the talk

Philipp Bergsmann and I built OTTO, a Slack bot that helps run the Vienna user group. These are the slides that carry the architecture.

![The five steps from a document to a working Slack bot: document knowledge, a Q and A YAML file, synthetic data generation, training, inference. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/8431cea-7126-48ff-3f81-7fcf8c18f8e_slovakia-020.png)

The five steps from a document to a working Slack bot: document knowledge, a Q and A YAML file, synthetic data generation, training, inference. Slide from the From MacBook to Bedrock deck.

![Three columns comparing open source, open weights and proprietary models, with Granite on one side and Claude, GPT and Nova on the other. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/f3d5eca-13cc-8b50-e217-6c315cb5db8_slovakia-022.png)

Three columns comparing open source, open weights and proprietary models, with Granite on one side and Claude, GPT and Nova on the other. Slide from the From MacBook to Bedrock deck.

![Synthetic data generation: a taxonomy feeds a teacher model, Mistral Small 24B, which scales the set thirty times into a training and test dataset. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/eb6b62d-def7-a378-7ac8-340d14e4ab_slovakia-027.png)

Synthetic data generation: a taxonomy feeds a teacher model, Mistral Small 24B, which scales the set thirty times into a training and test dataset. Slide from the From MacBook to Bedrock deck.

![Low rank adaptation: a large base model carrying general knowledge, plus a small LoRA adapter carrying the domain knowledge. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/a3703f2-dd2b-d1f-3531-ef61d445115_slovakia-032.png)

Low rank adaptation: a large base model carrying general knowledge, plus a small LoRA adapter carrying the domain knowledge. Slide from the From MacBook to Bedrock deck.

![The first agent crew: a Meetup Manager on Amazon Nova Pro delegating to a GitHub Planner, a Speaker Finder and an Agenda Producer, with Chroma as short term memory. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/b06088-dbd0-66d-800-85f405a2512_slovakia-039.png)

The first agent crew: a Meetup Manager on Amazon Nova Pro delegating to a GitHub Planner, a Speaker Finder and an Agenda Producer, with Chroma as short term memory. Slide from the From MacBook to Bedrock deck.

![The second crew: Slack talks to a Q and A agent on Claude Sonnet 3.7, a User Group Specialist on a custom Llama 3B model and a Speaker Finder on Amazon Nova Pro. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/6aecd-5ab5-ef68-de5-7c83c4d0774b_slovakia-040.png)

The second crew: Slack talks to a Q and A agent on Claude Sonnet 3.7, a User Group Specialist on a custom Llama 3B model and a Speaker Finder on Amazon Nova Pro. Slide from the From MacBook to Bedrock deck.

![The whole architecture on one slide: a user reaches App Runner running CrewAI, which calls Bedrock for Claude Sonnet 3.7, Amazon Nova Pro and the custom model, with ECR and S3 beside it. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/b548f44-4f6-300a-3518-7a370656f138_slovakia-043.png)

The whole architecture on one slide: a user reaches App Runner running CrewAI, which calls Bedrock for Claude Sonnet 3.7, Amazon Nova Pro and the custom model, with ECR and S3 beside it. Slide from the From MacBook to Bedrock deck.

![The running cost of the entire setup, about thirty euro a month. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/865d76f-1270-0faf-d3a0-07503c56203_slovakia-045.png)

The running cost of the entire setup, about thirty euro a month. Slide from the From MacBook to Bedrock deck.

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
- [AWS Community Day DACH](/talks/aws-community-day-dach/)
- [AWS Community Day Czech Republic](/talks/aws-community-day-czech-republic/)
- [AWS Community Day Romania](/talks/aws-community-day-romania/)
- [AWS Community Day Italy](/talks/aws-community-day-italy/)
- [AWS Community Day Poland](/talks/aws-community-day-poland/)
- [CTRL+ESC Malta](/talks/ctrl-esc-malta/)
- [AWS Student Builder Group St. Pölten](/talks/aws-student-builder-group-st-poelten/)
- [Cloud Day FH Burgenland](/talks/cloud-day-fh-burgenland/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [awscommunityday.sk, the event's own site](https://www.awscommunityday.sk/)
- [Slides: From MacBook to Bedrock: Lessons from Building an AI Assistant, 2025](https://drive.google.com/file/d/1tap3GgiOqxxp5nO-w7wEzGQQoj3UUBvD/view)
- [Recap: From MacBook to Bedrock: Lessons from Building an AI Assistant, 2025](https://www.lindamohamed.com/blog/aws-community-day-slovakia-kosice-2025)
- [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)
- [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)
- [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)
- [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-community-day-slovakia), where it was first published.
