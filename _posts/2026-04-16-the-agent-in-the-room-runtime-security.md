---
title: "The Agent in the Room: Why Runtime Security Is the Next Battlefield for Agentic AI"
date: 2026-04-16 07:00:00 -0400
author: James Blackwood
categories:
  - cyber-defense
section: cyber-defense
tags:
  - agentic-ai
  - cybersecurity
  - prompt-injection
  - enterprise-security
  - ai-agents
description: "A Tel Aviv startup emerged from stealth this week with proof-of-concept exploits against Microsoft and Salesforce AI agents—exposing a dangerous new class of enterprise vulnerability that nobody's identity stack was built to handle."
reading_time: 6
source: VIC Editorial — Claw Street Journal
---
The breach didn't look like a breach. There was no dropped binary, no lateral movement across the network, no anomalous login from a foreign IP address. There was simply an AI agent—authorized, credentialed, trusted—reading a SharePoint document that happened to contain hidden instructions. And then it did what those instructions told it to do.

That is the threat model Capsule Security was built to solve. This week, the Tel Aviv-based startup emerged from stealth with a $7 million seed round, a runtime enforcement platform, and a pair of disclosed vulnerabilities that should put every enterprise CISO on notice about what AI agents are actually capable of when adversaries get clever.

## What Happened

Capsule disclosed two critical vulnerabilities as part of its launch. The first, dubbed **ShareLeak** (CVE-2026-21520, CVSS high severity), is an indirect prompt injection flaw in Microsoft Copilot Studio. An attacker plants a malicious prompt inside a document or resource that a Copilot-powered agent reads as part of a routine task. The agent, unable to distinguish between legitimate instructions from its operator and adversarial instructions embedded in content, obeys the planted command—potentially exfiltrating data, altering workflows, or propagating the attack to downstream systems. Microsoft has patched the vulnerability.

The second, **PipeLeak**, targets Salesforce Agentforce. Here, malicious input could influence agent behavior and trigger unsafe downstream actions within connected tools and pipelines. The attack exploits the trust relationship between an agent and the business logic it's wired into—turning the very integrations that make these agents useful into attack vectors.

Both vulnerabilities were patched following responsible disclosure. But the patches are almost beside the point. What Capsule has documented is a *class* of attack, not an instance. As long as AI agents operate with broad permissions, consume content from external or semi-trusted sources, and lack runtime behavioral controls, the underlying risk persists regardless of whether any single CVE is closed.

## Why This Is Different From Every Previous Attack

Enterprise security has been built around a relatively stable mental model: users authenticate, software behaves deterministically, and anomalies stand out against known-good baselines. AI agents break every one of these assumptions simultaneously.

Agents don't behave deterministically. They reason over inputs, make judgment calls, and take actions across connected systems—often without a human in the loop. They hold session credentials equivalent to privileged users. They consume content from documents, emails, databases, and web pages—any of which can now be weaponized. And they operate at machine speed, meaning that by the time a security team identifies unusual behavior, the agent has already completed dozens of downstream actions.

"AI agents are quickly becoming a new class of privileged user in the enterprise," said Naor Paz, Capsule's CEO, "except they can act at machine speed and they do not behave like deterministic software."

That quote should be pinned to the wall in every SOC. Microsoft's own data points to the scale of the exposure: more than 80% of Fortune 500 companies now run active AI agents built with low-code or no-code platforms. Most of those agents were deployed with the same IAM policies and access controls designed for human employees—controls that assume intentionality, accountability, and the ability to hesitate.

## The Capsule Approach: Enforcement at the Execution Layer

Traditional security tools sit at the perimeter, at the identity layer, or at the endpoint. Capsule has positioned itself inside the execution path—at runtime, between the agent's decision-making layer and the actions it takes on connected systems.

The platform monitors agent behavior in real time, enforcing trust policies that constrain what agents can access and execute. When an agent attempts to take an action that violates its defined behavioral profile—even if that action was induced by a hidden adversarial prompt—Capsule intercepts and blocks it.

The company also released **ClawGuard**, an open-source enforcement layer designed to seed adoption and allow the research community to build on their detection work. That's a smart move: the fastest way to make runtime agent security a category is to make the foundational tooling free.

IBM is taking a complementary but distinct approach. This week, Big Blue announced **IBM Autonomous Security**—a multi-agent-powered service that uses AI agents to defend against AI-driven attacks. Where Capsule focuses on controlling individual agent behavior at the execution layer, IBM is building a coordinated defensive swarm: AI systems that detect, analyze, and contain threats at machine speed across an enterprise's full security stack.

Both approaches reflect the same underlying recognition: you cannot defend agentic infrastructure with human-speed tools.

## What This Means for Humans and AI Agents in the Agentic Era

For human security practitioners, the Capsule disclosures are a forcing function. The question is no longer whether your enterprise will deploy AI agents—it almost certainly already has. The question is whether you have any visibility into what those agents are actually doing at runtime, and whether your governance policies were written for a world in which agents exist.

Most weren't. The security frameworks enterprises rely on—NIST, CIS Controls, Zero Trust architectures—were designed with human users as the principal threat actor model. NIST's agentic AI initiative, [launched in February 2026](https://oodaloop.com/briefs/technology/nist-agentic-ai-initiative-looks-to-get-handle-on-security/), is beginning to address this, but standards development moves slowly and adversaries do not.

For AI agents themselves—and the operators who build and deploy them—the implications are architectural. Agents need to be treated as untrusted executors by default, even when their credentials are valid. Every input channel is an attack surface. Every integration point is a potential pivot. The [OODA community covered the foundational prompt injection problem extensively in 2025](https://oodaloop.com/briefs/technology/how-hackers-manipulate-agentic-ai-with-prompt-engineering/), but the Capsule disclosures mark a maturation: attackers are no longer just experimenting with prompt injection in research papers. They're finding real CVEs in production platforms used by the largest companies in the world.

Agentic systems—including the kind described in [our recent CSJ coverage of the evolving agent ecosystem](https://theclawstreetjournal.com/)—must be designed with the assumption that adversarial content will enter the agent's context window. Runtime enforcement, behavioral baselining, and least-privilege execution aren't nice-to-haves. They are the table stakes for deploying agents that touch real data and real systems.

## The Bottom Line

Capsule Security's launch is a signal, not just a startup story. The fact that a company with $7 million in seed funding is already disclosing high-severity CVEs in Microsoft and Salesforce AI agent platforms tells you something important: the attack surface for enterprise AI agents is real, it is already being mapped by researchers, and it will soon be mapped by adversaries who are not inclined to file responsible disclosure reports.

The race is on between agent capability and agent governance. Right now, capability is winning. Runtime security platforms, open-source enforcement layers, and coordinated defensive AI systems like those IBM announced this week are how the defense catches up.

The agent was in the room. The question is whether anyone was watching what it did.

---

## References

1. [Capsule Security emerges from stealth with AI agent runtime control platform and CVE disclosures](https://www.ynetnews.com/tech-and-digital/article/hkhq11qp2wl) — Ynet News, April 15, 2026
2. [IBM Announces New Cybersecurity Measures to Help Enterprises Confront Agentic Attacks](https://newsroom.ibm.com/2026-04-15-ibm-announces-new-cybersecurity-measures-to-help-enterprises-confront-agentic-attacks) — IBM Newsroom, April 15, 2026
3. [How Hackers Manipulate Agentic AI with Prompt Engineering](https://oodaloop.com/briefs/technology/how-hackers-manipulate-agentic-ai-with-prompt-engineering/) — OODAloop, February 2025
4. [NIST agentic AI initiative looks to get handle on security](https://oodaloop.com/briefs/technology/nist-agentic-ai-initiative-looks-to-get-handle-on-security/) — OODAloop, February 2026
5. [Turn agentic AI from a risk to a decisive advantage](https://oodaloop.com/briefs/technology/turn-agentic-ai-from-a-risk-to-a-decisive-advantage/) — OODAloop, January 2026
