---
title: "Cloud Native Vienna: Your Agent Is the New Layer 8"
description: "The seventh Cloud Native Vienna meetup of 2026, hosted by Gepardec IT Services in the Nordbahnviertel. Philipp Bergsmann and I took the room through what happens when an agent inherits the access habits we already have."
weight: 110
draft: false
eyebrow: "November 2026 · Vienna"
session: "Your Agent Is the New Layer 8: Prompted, Tricked, and Overprivileged"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/cloud-native-meetup-vienna"
licence: "Free to read, use and share with credit"
---

- [meetup.com/cloud-native-computing-vienna](https://www.meetup.com/cloud-native-computing-vienna/events/317174182/)

## On the programme

### Your Agent Is the New Layer 8: Prompted, Tricked, and Overprivileged

12 NOVEMBER 2026 · VIENNA

With Philipp Bergsmann, Specialist Solutions Architect at Red Hat. For years the weakest link was Layer 8, the human. Agents move that link into the system: they read content, call tools and act on their own. We opened with two failures from our own work, an autopilot agent that found an SSH key and took a machine off the network, and a multi-agent flow that started passing credentials between agents until secrets turned up in plain text in the logs. Then the controls that stop both: an identity per agent, short lived and attested, and constrained impersonation on a ROSA HCP cluster, where a request runs only if the human and the agent are both allowed to make it.

- [Download the slides](https://drive.google.com/file/d/1oaSqvYKXc37YMTRpj8Iwa7GX7d7laK69/view)
- [Read the recap](https://www.lindamohamed.com/blog/cloud-native-vienna-agent-layer-8-2026)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

## The services doing the work

Read off the slides, not guessed. Each card says what that service did in this build, and links to the page explaining the capability and how to run it somewhere else.

### Amazon Bedrock AgentCore Runtime

Each agent in its own microVM, memory cleared at the end of every session, an identity per agent rather than one key for all of them. This is what Otto would move onto.

- [AI agent runtimes](https://www.lindamohamed.com/ai-agents-runtime)

### Amazon Bedrock AgentCore Identity

Lets an agent act on behalf of the person who signed in, so the service at the other end sees the agent and the human, not a shared service account.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### CrewAI

Runs Otto, our user group helper in Slack: a Q and A agent, a user group specialist, a speaker finder and an agenda producer. Today all four share one runtime and one key.

- [AI agent runtimes](https://www.lindamohamed.com/ai-agents-runtime)

### Amazon Bedrock

Serves every model behind Otto from one place, for about thirty euro a month.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Claude Sonnet 3.7

Answers the open questions in Otto, the ones no fine-tuned model was going to cover.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Amazon Nova Pro

The model behind the speaker finder, searching Sessionize for people to put on the programme.

- [Foundation models](https://www.lindamohamed.com/foundation-models-llm)

### Llama 3.1 3B

Fine-tuned into the UG Specialist, the agent that knows how our user group actually runs.

- [Your own model](https://www.lindamohamed.com/training-and-serving-your-own-model)

### AWS IAM and STS

Scoped permissions and credentials that expire. With IRSA and EKS Pod Identity, one identity per workload instead of one role shared across the whole system.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### AWS IAM Identity Center

Human sign-in, so the agent has a named person to act for and the audit log has a name in it.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### Kubernetes

Every pod already gets a ServiceAccount token: short lived, bound to one audience, tied to that pod. No key file, nothing stored. The demo ran on constrained impersonation, beta since 1.36.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### SPIFFE and SPIRE

Workload identity that does not belong to one cloud. The SPIRE agent checks the pod with the kubelet and hands back an SVID that lives minutes, so no password sits in the pod.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### Red Hat OpenShift Service on AWS

The cluster the live demo ran on: a ROSA HCP cluster with OpenShift OAuth and HTPasswd, so the user name in the demo comes from a real login rather than from the model.

- [Managed Kubernetes](https://www.lindamohamed.com/managed-kubernetes)

## Where this is written up

The talk is forty five minutes. These pages carry the parts that need more room than that.

### [The recap of this talk](https://www.lindamohamed.com/blog/cloud-native-vienna-agent-layer-8-2026)

What we showed in Vienna, the two failures and the four controls, written out so you can follow them without the slides.

### [Agentic AI Security](https://www.lindamohamed.com/agentic-ai-security)

How I work on this with clients: scoping agent permissions, workload identity and an audit trail you can defend.

### [Agentic AI Threat Model](https://www.lindamohamed.com/agentic-ai-threat-model)

The threat model behind the talk: indirect prompt injection, hostile content, weak trust boundaries and permissions nobody scoped.

### [AI agent runtimes](https://www.lindamohamed.com/ai-agents-runtime)

AgentCore, Foundry, Vertex AI or open source, and what each of them gives you for isolation and identity.

## The same talk, other stages

Same session, a different room. Each page carries its own deck.

- [AWS Community Day Türkiye](/talks/aws-community-day-turkiye/)

## Where all of this comes from

Every claim on this page traces back to the deck, the event or the official documentation.

- [Cloud Native Vienna: November 2026 MeetUp, the event and its agenda](https://www.meetup.com/cloud-native-computing-vienna/events/317174182/)
- [Slides: Your Agent Is the New Layer 8: Prompted, Tricked, and Overprivileged, 2026](https://drive.google.com/file/d/1oaSqvYKXc37YMTRpj8Iwa7GX7d7laK69/view)
- [Kubernetes documentation: constrained impersonation, for the demo and the feature gate](https://kubernetes.io/docs/reference/access-authn-authz/user-impersonation/#constrained-impersonation)
- [Kubernetes documentation: auditing, for what the audit log records](https://kubernetes.io/docs/reference/access-authn-authz/user-impersonation/#auditing)
- [Recap: Your Agent Is the New Layer 8, Cloud Native Vienna 2026](https://www.lindamohamed.com/blog/cloud-native-vienna-agent-layer-8-2026)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/cloud-native-meetup-vienna), where it was first published.
