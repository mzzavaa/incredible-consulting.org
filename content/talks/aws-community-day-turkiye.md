---
title: "AWS Community Day Türkiye"
description: "The Turkish community day in Istanbul, run by the Cloud Türkiye community."
weight: 170
draft: false
eyebrow: "2026 · Istanbul"
session: "Your Agent Is the New Layer 8: Prompted, Tricked, and Overprivileged"
status_label: "Slides free to download"
source_url: "https://www.lindamohamed.com/aws-community-day-turkiye"
licence: "Free to read, use and share with credit"
---

- [the event on Kommunity](https://kommunity.com/cloud-turkiye/events/aws-community-day-turkiye-2026-7ed168b3)

## On the programme

### Your Agent Is the New Layer 8: Prompted, Tricked, and Overprivileged

*2026 · Istanbul*

With Philipp Bergsmann. Two agent failures from our own machines, then the controls that fix them: per-agent isolation, workload identity, SPIFFE and SPIRE, OAuth and OIDC, and scoping at runtime with RFC 8693 token exchange.

- [Download the slides](https://drive.google.com/file/d/1cKRqo4UCX9LBur00SkMRboRyS4HqnJ19/view)
- [Have me give this talk](https://bookings.cloud.microsoft/book/Letstalk@lindamohamed.com/s/F_Jis4LDA0mHQmuslLXijA2/)

## The services doing the work

Read off the slides, not guessed. Each card says what that service did in this build, and links to the page explaining the capability and how to run it somewhere else.

### Amazon Bedrock AgentCore Runtime

Per-agent isolation by default: a dedicated microVM per agent, memory sanitised at the end of every session, and an identity per agent instead of one shared between them.

- [AI agents](https://www.lindamohamed.com/ai-agents-runtime)

### Amazon Bedrock AgentCore Identity

On-behalf-of token exchange, so the downstream service sees both the agent and the user it is acting for.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### AWS IAM

Scoped permissions the agent assumes as a role, instead of one shared key passed around.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### AWS STS and IRSA

One identity per workload, issued at runtime and short-lived.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### IAM Identity Center

Human SSO into AWS: the first hop, before the agent assumes anything.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### SPIFFE

An open identity standard for workloads, Active Directory but for software. A SPIFFE ID names the trust domain and the workload itself, as in spiffe://otto.io/agent/researcher. Use it when you straddle several clouds and on-prem and IAM cannot be the only source of truth.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### SPIRE

The implementation that issues and attests those identities: it proves what a workload is at runtime from its node, namespace and image. Also used by Istio, Linkerd and Vault.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### OAuth 2.1

Authorization. Access tokens, refresh tokens and scopes, answering whether this thing may do that.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

### OpenID Connect

Authentication. ID tokens on top of OAuth, answering who the user is. With RFC 8693 token exchange the broker mints a token that says: this agent, acting for this user, scoped to X.

- [Identity and access](https://www.lindamohamed.com/identity-access-management)

## Slides from the talk

Your Agent Is the New Layer 8, with Philipp Bergsmann. The slides that carry the argument.

![The seven OSI layers with the AWS services that take each one over, and a dashed band above them labelled Layer 8: humans, agents and managed service teams. Slide from the Your Agent Is the New Layer 8 deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/0e842fd-7440-3546-100-fdea42b43a4_turkiye-021.png)

The seven OSI layers with the AWS services that take each one over, and a dashed band above them labelled Layer 8: humans, agents and managed service teams. Slide from the Your Agent Is the New Layer 8 deck.

![Three cards comparing a single agent, a multi-agent setup and sub-agents, rated low, medium and high risk, with sub-agents marked as a workflow pattern rather than a security boundary. Slide from the Your Agent Is the New Layer 8 deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/51ac15a-83c7-f833-33e-cfb842eac7d_turkiye-027.png)

Three cards comparing a single agent, a multi-agent setup and sub-agents, rated low, medium and high risk, with sub-agents marked as a workflow pattern rather than a security boundary. Slide from the Your Agent Is the New Layer 8 deck.

![The same four practices side by side: a red column of what would be a fireable offence with people, a green column of what teams ship with agents on a Tuesday. Slide from the Your Agent Is the New Layer 8 deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/0cb7c4-63bc-ae23-8025-6b40ca6ccf2_turkiye-029.png)

The same four practices side by side: a red column of what would be a fireable offence with people, a green column of what teams ship with agents on a Tuesday. Slide from the Your Agent Is the New Layer 8 deck.

![Workload identity in four numbered points: provisioned, attestable, short lived, auditable, with a code line keeping agent, runtime and user identity separate. Slide from the Your Agent Is the New Layer 8 deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/2cdbfae-6b10-1a61-efae-c8eb7006fa6_turkiye-031.png)

Workload identity in four numbered points: provisioned, attestable, short lived, auditable, with a code line keeping agent, runtime and user identity separate. Slide from the Your Agent Is the New Layer 8 deck.

![Four AWS pieces that already cover most of this: IAM roles, STS and IRSA, Identity Center, and AgentCore Identity for on-behalf-of token exchange, with the end to end story written underneath. Slide from the Your Agent Is the New Layer 8 deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/ca6e2b7-0f2c-6b61-4e33-15db83144eae_turkiye-032.png)

Four AWS pieces that already cover most of this: IAM roles, STS and IRSA, Identity Center, and AgentCore Identity for on-behalf-of token exchange, with the end to end story written underneath. Slide from the Your Agent Is the New Layer 8 deck.

![Token exchange drawn as four boxes: a human user with full scope, an OIDC broker that downscopes, the agent with a subset of the user, and the resource, with the rule that agent scope stays inside human scope. Slide from the Your Agent Is the New Layer 8 deck.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/f476a-d43a-35de-264b-850178dfe67_turkiye-035.png)

Token exchange drawn as four boxes: a human user with full scope, an OIDC broker that downscopes, the agent with a subset of the user, and the resource, with the rule that agent scope stays inside human scope. Slide from the Your Agent Is the New Layer 8 deck.

![The closing line of the talk over a lab scene, the same controls and the same standards. Slide from the Your Agent Is the New Layer 8 deck, background image AI generated.](https://kajabi-storefronts-production.s3.amazonaws.com/file-uploads/sites/2148741032/images/303c480-d342-02d6-0b4d-5c80eba836_turkiye-039.png)

The closing line of the talk over a lab scene, the same controls and the same standards. Slide from the Your Agent Is the New Layer 8 deck, background image AI generated.

## The longer write-ups

Where the builds behind these sessions are explained properly.

### [OpenClaw: The Local AI Agent That Executes Tasks](https://www.lindamohamed.com/blog/what-is-openclaw)

The longer write-up: the build, the services and what it costs to run.

### [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)

The longer write-up: the build, the services and what it costs to run.

### [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

The longer write-up: the build, the services and what it costs to run.

## The same talk, other stages

Same session, a different room. Each page carries its own deck.

- [Cloud Native Meetup Vienna](/talks/cloud-native-meetup-vienna/)

## Where all of this comes from

Every claim on this page traces back to the deck, the recap or the event's own site.

- [Slides: Your Agent Is the New Layer 8: Prompted, Tricked, and Overprivileged, 2026](https://drive.google.com/file/d/1cKRqo4UCX9LBur00SkMRboRyS4HqnJ19/view)
- [OpenClaw: The Local AI Agent That Executes Tasks](https://www.lindamohamed.com/blog/what-is-openclaw)
- [What is an AWS Community Day?](https://www.lindamohamed.com/blog/what-is-an-aws-community-day)
- [10 Years of AWS User Group Vienna](https://www.lindamohamed.com/blog/10-years-of-aws-user-group-vienna)

Everything here is free to read, use and share. No email needed for the slides. If you reuse something, please credit the source.

This page mirrors [the talk page on lindamohamed.com](https://www.lindamohamed.com/aws-community-day-turkiye), where it was first published.
