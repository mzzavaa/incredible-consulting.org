---
title: "AWS re:Invent"
description: "AWS re:Invent in Las Vegas, twice. Two different formats, two different decks, both free here."
weight: 210
draft: false
eyebrow: "2025 · Las Vegas"
session: "OTTO at the Open Source Learning Corner"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/aws-reinvent"
licence: "Free to read, use and share with credit"
---

- [reinvent.awsevents.com](https://reinvent.awsevents.com/)

## On the programme

### OTTO at the Open Source Learning Corner

*2025 · Las Vegas*

A lightweight multi-agent system that automates recurring tasks in communities and teams, presented at the Open Source Learning Corner. Cloud-native, cost-efficient and scale-to-zero, with the emphasis on simplicity and real operational use.

- [Download the slides](https://drive.google.com/file/d/106heBUSxPbRtwYu47-9724KjLA0SABQl/view)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

### Build Amazon Q apps to scale and drive community engagement

*2024 · Las Vegas*

How AI services including Amazon Q Business can scale community engagement, streamline event planning and handle an organiser's everyday tasks, with a live demo using Amazon S3 and AWS Lambda alongside Q Business.

- [Download the slides](https://drive.google.com/file/d/1CmbarDbWLRlFD83HymxPt30XKGDoGNta/view)
- [Read the recap](https://www.lindamohamed.com/blog/aws-reinvent-2024)
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

### Amazon Q Business

Answers against the community's own documents, with permissions carried through from the identity provider into every filtered response.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### AWS Lambda

The integration glue between the assistant and everything else.

- [Serverless compute](https://www.lindamohamed.com/serverless-compute)

### Amazon Rekognition

Image and video analysis, as the immediate way into AI without a model of your own.

- [Image recognition](https://www.lindamohamed.com/image-recognition-object-detection)

### Amazon Textract

Pulls printed text, handwriting and form data out of almost any document.

- [Reading documents](https://www.lindamohamed.com/document-ocr-text-extraction)

### Amazon Transcribe

Speech to text.

- [Speech to text](https://www.lindamohamed.com/speech-to-text-transcription)

### Amazon Comprehend

Insight and relationships in text.

- [Text analysis](https://www.lindamohamed.com/text-analysis-nlp)

### Amazon Polly

Text into lifelike speech.

- [Text to speech](https://www.lindamohamed.com/text-to-speech)

### Amazon Translate

Machine translation between languages.

- [Machine translation](https://www.lindamohamed.com/machine-translation)

### Amazon SageMaker AI

Rapid model deployment when a ready-made service is not enough.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

## Slides from the session

DEV201 at re:Invent 2024: four Amazon Q Business applications that take work off a user group organiser. These are the architecture slides.

![Identify Locations: a Lambda scrapes AWS user group and partner pages into CSV and TXT on S3, EventBridge and Step Functions drive it, and Amazon Q connectors read it into the business app. Slide from the DEV201 deck, re:Invent 2024.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/5d671-0100-1012-1804-dbb0d82aa37_reinvent2024-017.png)

Identify Locations: a Lambda scrapes AWS user group and partner pages into CSV and TXT on S3, EventBridge and Step Functions drive it, and Amazon Q connectors read it into the business app. Slide from the DEV201 deck, re:Invent 2024.

![Find Speakers: Lambdas pull the Sessionize speakers directory and the AWS Heroes and Community Builders lists into CSV on S3, with three custom layers for requests, BS4 and pandas. Slide from the DEV201 deck, re:Invent 2024.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/a8c5248-f06f-5683-e055-31edef2e47f8_reinvent2024-022.png)

Find Speakers: Lambdas pull the Sessionize speakers directory and the AWS Heroes and Community Builders lists into CSV on S3, with three custom layers for requests, BS4 and pandas. Slide from the DEV201 deck, re:Invent 2024.

![Identify Dates: a web crawler reaches Meetup events through Secrets Manager, and a Lambda writes AWS events data to S3 for the Amazon Q connectors. Slide from the DEV201 deck, re:Invent 2024.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/614265a-f4-2e24-85bf-215c7fa62fe3_reinvent2024-034.png)

Identify Dates: a web crawler reaches Meetup events through Secrets Manager, and a Lambda writes AWS events data to S3 for the Amazon Q connectors. Slide from the DEV201 deck, re:Invent 2024.

![Content: a Lambda collects AWS Events videos from YouTube into CSV on S3, alongside the community blogs crawled directly. Slide from the DEV201 deck, re:Invent 2024.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/f013f83-440d-86c2-aef2-c1f1bf20bb44_reinvent2024-041.png)

Content: a Lambda collects AWS Events videos from YouTube into CSV on S3, alongside the community blogs crawled directly. Slide from the DEV201 deck, re:Invent 2024.

![The whole thing on one page: authenticated users reach the Amazon Q web application and business index, fed by five scraping Lambdas and a set of web crawlers covering Meetup, community blogs, the Vienna meetup planner and the slides. Slide from the DEV201 deck, re:Invent 2024.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/5ed7655-f21b-73b-b5b-c05cdca2aaf_reinvent2024-047.png)

The whole thing on one page: authenticated users reach the Amazon Q web application and business index, fed by five scraping Lambdas and a set of web crawlers covering Meetup, community blogs, the Vienna meetup planner and the slides. Slide from the DEV201 deck, re:Invent 2024.

![The four takeaways the session closed on: align Amazon Q Business with specific use cases, develop a data strategy, optimize for cost, keep the implementation compliant. Slide from the DEV201 deck, re:Invent 2024.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/e0351a3-28-fa8e-63ec-2048b6002215_reinvent2024-048.png)

The four takeaways the session closed on: align Amazon Q Business with specific use cases, develop a data strategy, optimize for cost, keep the implementation compliant. Slide from the DEV201 deck, re:Invent 2024.

## The longer write-ups

Where the builds behind these sessions are explained properly.

### [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)

The longer write-up: the build, the services and what it costs to run.

### [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)

The longer write-up: the build, the services and what it costs to run.

### [How I Planned AWS re:Invent in Notion](https://www.lindamohamed.com/blog/aws-reinvent-2025-notion-planner)

The longer write-up: the build, the services and what it costs to run.

### [AI Use Cases](https://www.lindamohamed.com/ai-use-cases)

The longer write-up: the build, the services and what it costs to run.

## The same talk, other stages

Same session, a different room. Each page carries its own deck.

- [AWS Community Day DACH](/talks/aws-community-day-dach/)
- [AWS Community Day Slovakia](/talks/aws-community-day-slovakia/)
- [AWS Community Day Czech Republic](/talks/aws-community-day-czech-republic/)
- [AWS Community Day Romania](/talks/aws-community-day-romania/)
- [AWS Community Day Italy](/talks/aws-community-day-italy/)
- [AWS Community Day Poland](/talks/aws-community-day-poland/)
- [CTRL+ESC Malta](/talks/ctrl-esc-malta/)
- [AWS Student Builder Group St. Pölten](/talks/aws-student-builder-group-st-poelten/)
- [Cloud Day FH Burgenland](/talks/cloud-day-fh-burgenland/)
- [AWS Community Day Switzerland](/talks/aws-community-day-switzerland/)
- [AWS User Group Košice](/talks/aws-user-group-kosice/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [reinvent.awsevents.com, the event's own site](https://reinvent.awsevents.com/)
- [Slides: OTTO at the Open Source Learning Corner, 2025](https://drive.google.com/file/d/106heBUSxPbRtwYu47-9724KjLA0SABQl/view)
- [Slides: Build Amazon Q apps to scale and drive community engagement, 2024](https://drive.google.com/file/d/1CmbarDbWLRlFD83HymxPt30XKGDoGNta/view)
- [Recap: Build Amazon Q apps to scale and drive community engagement, 2024](https://www.lindamohamed.com/blog/aws-reinvent-2024)
- [From AI Demo to Enterprise Solutions](https://www.lindamohamed.com/blog/from-ai-prototype-to-enterprise-solution)
- [Enterprise AI Consultant vs. AI Consultant](https://www.lindamohamed.com/blog/enterprise-ai-consultant-vs-ai-consultant)
- [How I Planned AWS re:Invent in Notion](https://www.lindamohamed.com/blog/aws-reinvent-2025-notion-planner)
- [AI Use Cases](https://www.lindamohamed.com/ai-use-cases)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-reinvent), where it was first published.
