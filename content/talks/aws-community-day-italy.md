---
title: "AWS Community Day Italy"
description: "The Italian community day in Milan, under the theme Learn and be curious, curated by Monica Colangelo. The stage was a 50/50 gender split."
weight: 270
draft: false
eyebrow: "2025 · Milan"
session: "From MacBook to Bedrock: Lessons from Building an AI Assistant"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/aws-community-day-italy"
licence: "Free to read, use and share with credit"
---

- [awscommunityday.it](https://www.awscommunityday.it/)

## On the programme

### From MacBook to Bedrock: Lessons from Building an AI Assistant

*2025 · Milan*

With Philipp Bergsmann. Building OTTO with InstructLab and Amazon Bedrock, the CrewAI agent architecture behind it, the Slack demo and the running cost of about 30 euro a month.

- [Download the slides](https://drive.google.com/file/d/1NAPdZJm1IRSp5q9faf66oAVZbnlmEfeO/view)
- [Read the recap](https://www.lindamohamed.com/blog/aws-community-day-italy-milano-2025)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

### Women of Cloud workshop

*2025 · Milan*

Co-hosted with Suzana Melo and Darya Petrashka. No slides published for this one.

- No slides for this one
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

## On stage in Milan

![Linda Mohamed speaking with both arms open in front of a projected chat log](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/c74143b-f15-12b1-d2e-ead578b41532_milano-2.jpg)

Opening the talk in front of the chat log the agents produced. Photo by Dmytro Hlotenko, AWS Community Day Italy, Milan, 8 April 2025.

![Linda Mohamed gesturing with both hands while explaining a slide](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/cd2686c-86c-060-0f1-fdf3e027e64e_milano-3.jpg)

Walking through what the crew of agents actually does. Photo by Dmytro Hlotenko, AWS Community Day Italy, Milan, 8 April 2025.

![Wide view of the stage with Linda Mohamed and her co-presenter in front of an architecture diagram](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/blogs/2148040642/images/02a5bf0-6b8d-7508-6381-1a8760c1360_milano-4.jpg)

The architecture on screen: from the laptop fine-tune to the model served on Bedrock. Photo by Dmytro Hlotenko, AWS Community Day Italy, Milan, 8 April 2025.

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

From MacBook to Bedrock, with Philipp Bergsmann. The slides that carry the architecture.

![The five steps from a document to a working Slack bot: document knowledge, a Q and A YAML file, synthetic data generation, training, inference. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/a452be3-8ae-3387-7eb0-363f874317a3_italy-030.png)

The five steps from a document to a working Slack bot: document knowledge, a Q and A YAML file, synthetic data generation, training, inference. Slide from the From MacBook to Bedrock deck.

![Synthetic data generation: a taxonomy feeds a teacher model, Mistral Small 24B, which scales the set thirty times into a training and test dataset. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/305688-bec-a00-0c-d37853416e7b_italy-042.png)

Synthetic data generation: a taxonomy feeds a teacher model, Mistral Small 24B, which scales the set thirty times into a training and test dataset. Slide from the From MacBook to Bedrock deck.

![The first agent crew: a Meetup Manager on Amazon Nova Pro delegating to a GitHub Planner, a Speaker Finder and an Agenda Producer, with Chroma as short term memory. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/e5aede4-0db-03f6-d5bb-c16752417332_italy-063.png)

The first agent crew: a Meetup Manager on Amazon Nova Pro delegating to a GitHub Planner, a Speaker Finder and an Agenda Producer, with Chroma as short term memory. Slide from the From MacBook to Bedrock deck.

![The second crew: Slack talks to a Q and A agent on Claude Sonnet 3.7, a User Group Specialist on a custom Llama 3B model and a Speaker Finder on Amazon Nova Pro. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/3e6657b-53b-3cf-264-3efbac3ea42_italy-064.png)

The second crew: Slack talks to a Q and A agent on Claude Sonnet 3.7, a User Group Specialist on a custom Llama 3B model and a Speaker Finder on Amazon Nova Pro. Slide from the From MacBook to Bedrock deck.

![The running cost of the entire setup, about thirty euro a month. Slide from the From MacBook to Bedrock deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/d557c0-e83-72b2-32f1-41c5ff1cd51_italy-069.png)

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
- [AWS Community Day Slovakia](/talks/aws-community-day-slovakia/)
- [AWS Community Day Czech Republic](/talks/aws-community-day-czech-republic/)
- [AWS Community Day Romania](/talks/aws-community-day-romania/)
- [AWS Community Day Poland](/talks/aws-community-day-poland/)
- [CTRL+ESC Malta](/talks/ctrl-esc-malta/)
- [AWS Student Builder Group St. Pölten](/talks/aws-student-builder-group-st-poelten/)
- [Cloud Day FH Burgenland](/talks/cloud-day-fh-burgenland/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [awscommunityday.it, the event's own site](https://www.awscommunityday.it/)
- [Slides: From MacBook to Bedrock: Lessons from Building an AI Assistant, 2025](https://drive.google.com/file/d/1NAPdZJm1IRSp5q9faf66oAVZbnlmEfeO/view)
- [Recap: From MacBook to Bedrock: Lessons from Building an AI Assistant, 2025](https://www.lindamohamed.com/blog/aws-community-day-italy-milano-2025)
- [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)
- [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)
- [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)
- [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-community-day-italy), where it was first published.
