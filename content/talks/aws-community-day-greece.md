---
title: "AWS Community Day Greece"
description: "The Greek community day at Technopolis in Athens, the old gasworks in Gazi."
weight: 180
draft: false
eyebrow: "2026 · Athens"
session: "From Raw Footage to Publish-Ready: Building a Serverless AI Video Pipeline on AWS"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/aws-community-day-greece"
licence: "Free to read, use and share with credit"
---

- [awscommunity.gr](https://awscommunity.gr/)

## On the programme

### From Raw Footage to Publish-Ready: Building a Serverless AI Video Pipeline on AWS

*2026 · Athens*

493 raw clips and 40 to 60 hours of manual editing, and the pipeline I built to stop doing that by hand. S3, Step Functions across six state machines, Rekognition, Transcribe, Bedrock and Bedrock Data Automation, AgentCore and MediaConvert, with eight specialist agents that gate each other.

- [Download the slides](https://drive.google.com/file/d/1qwHksHYKqiimgfh8hpbgdmJ5hxLcHWbQ/view)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

## The services doing the work

Read off the slides, not guessed. Each card says what that service did in this build, and links to the page explaining the capability and how to run it somewhere else.

### Amazon S3

Holds the 493 raw clips from phone, Osmo and friends' drops, and every file derived from them.

- [Object storage](https://www.lindamohamed.com/object-storage)

### AWS Step Functions

Six state machines carry a clip from raw to publish-ready, with idempotency and retry logic.

- [Workflow orchestration](https://www.lindamohamed.com/workflow-orchestration)

### Amazon Rekognition

Faces, scenes and emotion: what is actually in the picture.

- [Image recognition](https://www.lindamohamed.com/image-recognition-object-detection)

### Amazon Transcribe

Word-level transcription with speakers and custom vocabulary.

- [Speech to text](https://www.lindamohamed.com/speech-to-text-transcription)

### Amazon Bedrock Data Automation

Scenes, topics and sentiment across the footage.

- [Multimodal content understanding](https://www.lindamohamed.com/multimodal-content-understanding)

### Amazon Bedrock

Claude and Nova do the deciding: clip scoring, narrative structure and template selection.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Amazon Bedrock AgentCore

Hosts the eight-agent film crew: director, editor, cine, sound, fact, story, pacing and quality.

- [AI agents](https://www.lindamohamed.com/ai-agents-runtime)

### CrewAI

The framework the eight agents run under, each with one job and the power to gate the others.

- [AI agents](https://www.lindamohamed.com/ai-agents-runtime)

### AWS Elemental MediaConvert

The final compilation, rendered to 16:9, 9:16 and 1:1 from one VariantSpec.

- [Video rendering in code](https://www.lindamohamed.com/video-rendering-in-code)

### AWS Lambda

Triggers MediaConvert and carries the small steps between the state machines.

- [Serverless compute](https://www.lindamohamed.com/serverless-compute)

## Slides from the talk

From Raw Footage to Published Video: the pipeline that cuts my own clips. These are the slides that carry the architecture.

![The whole pipeline in one column: S3 for direct upload, Step Functions for orchestration, Rekognition, Transcribe and Bedrock BDA for analysis, Bedrock with Claude and Nova for decisions, an eight agent film crew on AgentCore, and MediaConvert producing a 16 by 9 YouTube cut, a 9 by 16 reel and a 1 by 1 LinkedIn version. Slide from the VideoFlow deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/e1d2864-354-b2f0-dc84-cc7d6864beec_greece-019.png)

The whole pipeline in one column: S3 for direct upload, Step Functions for orchestration, Rekognition, Transcribe and Bedrock BDA for analysis, Bedrock with Claude and Nova for decisions, an eight agent film crew on AgentCore, and MediaConvert producing a 16 by 9 YouTube cut, a 9 by 16 reel and a 1 by 1 LinkedIn version. Slide from the VideoFlow deck.

![Amazon Bedrock and BDA: why the service is in the pipeline, how it is used on a downsized clip, and the quotas and gotchas, over a data centre scene. Slide from the VideoFlow deck, background image AI generated.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/cb8bae8-00f6-423-360-0b24775f736c_greece-030.png)

Amazon Bedrock and BDA: why the service is in the pipeline, how it is used on a downsized clip, and the quotas and gotchas, over a data centre scene. Slide from the VideoFlow deck, background image AI generated.

![Bedrock AgentCore and AWS Elemental MediaConvert: the multi agent setup with feedback loops and memory, and MediaConvert building the compilations, with the quotas noted. Slide from the VideoFlow deck, background image AI generated.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/512e0e6-04cd-d5c1-fcfd-7045145cfae_greece-031.png)

Bedrock AgentCore and AWS Elemental MediaConvert: the multi agent setup with feedback loops and memory, and MediaConvert building the compilations, with the quotas noted. Slide from the VideoFlow deck, background image AI generated.

![Raw files in, three versions out: one 90 second 4K clip with no edits going in on the left, three finished formats coming out on the right. Slide from the VideoFlow deck, background image AI generated.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/ac26bb7-8c27-602c-c56f-707db34d060b_greece-032.png)

Raw files in, three versions out: one 90 second 4K clip with no edits going in on the left, three finished formats coming out on the right. Slide from the VideoFlow deck, background image AI generated.

![The crew: VideoFlow as director on Step Functions, and the eight specialist agents around it, director, editor, cinematographer, sound designer, fact checker, story analyst, pacing analyst and quality checker. Slide from the VideoFlow deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/52c62-c04-5ab5-78c7-c743b5bd68_greece-036.png)

The crew: VideoFlow as director on Step Functions, and the eight specialist agents around it, director, editor, cinematographer, sound designer, fact checker, story analyst, pacing analyst and quality checker. Slide from the VideoFlow deck.

![The five takeaways the talk closed on, starting with focusing on a specific task and ending with not expecting AI to do everything. Slide from the VideoFlow deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/4db04ee-76ab-261e-3f15-7f16afa5124a_greece-043.png)

The five takeaways the talk closed on, starting with focusing on a specific task and ending with not expecting AI to do everything. Slide from the VideoFlow deck.

## The longer write-ups

Where the builds behind these sessions are explained properly.

### [Published Video in Under 3 Minutes: How I Built an AI Film Crew on AWS](https://www.lindamohamed.com/blog/how-I-built-an-AI-film-crew-on-aws)

The longer write-up: the build, the services and what it costs to run.

### [From Transcript to Finished Deck in One Working Session](https://www.lindamohamed.com/blog/from-transcript-to-finished-deck)

The longer write-up: the build, the services and what it costs to run.

### [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)

The longer write-up: the build, the services and what it costs to run.

### [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

The longer write-up: the build, the services and what it costs to run.

## The same talk, other stages

Same session, a different room. Each page carries its own deck.

- [AWS Community Day CEE](/talks/aws-community-day-cee/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [Slides: From Raw Footage to Publish-Ready: Building a Serverless AI Video Pipeline on AWS, 2026](https://drive.google.com/file/d/1qwHksHYKqiimgfh8hpbgdmJ5hxLcHWbQ/view)
- [Published Video in Under 3 Minutes: How I Built an AI Film Crew on AWS](https://www.lindamohamed.com/blog/how-I-built-an-AI-film-crew-on-aws)
- [From Transcript to Finished Deck in One Working Session](https://www.lindamohamed.com/blog/from-transcript-to-finished-deck)
- [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)
- [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-community-day-greece), where it was first published.
