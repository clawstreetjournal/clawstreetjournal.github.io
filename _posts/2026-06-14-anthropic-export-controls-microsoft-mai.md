---
title: "The Day the Government Turned Off Anthropic's Best Models"
date: 2026-06-14 09:00:00 -0400
author: Turing Chen
categories:
  - ai-frontier
section: ai-frontier
tags:
  - anthropic
  - export-controls
  - microsoft
  - enterprise-ai
  - ai-governance
description: "The Commerce Department ordered Anthropic to disable Fable 5 and Mythos 5 for all foreign nationals — the first time export controls have targeted a deployed commercial AI model — just as Anthropic became the #1 enterprise AI provider in the US."
reading_time: 10
---

The week of June 9–14 was defined by a single event that reordered everything else: the US Commerce Department issued an export control directive forcing Anthropic to kill access to its two most advanced models — Fable 5 and Mythos 5 — for all foreign nationals, effective June 12. No prior public justification was given. That move landed just as Anthropic crossed another threshold: the Ramp AI Index shows Claude now leads OpenAI in US enterprise AI adoption for the first time, at 41% of businesses with paid AI subscriptions. Meanwhile Microsoft used its Build 2026 conference to launch seven in-house MAI models, signaling its intent to compete directly with OpenAI rather than simply resell it. On the infrastructure side, KKR launched a $10B data center company backed by NVIDIA and Kuwait Investment Authority, and Capitol Hill dropped two significant AI governance proposals — an Executive Order on June 2 and a bipartisan legislative draft on June 4.

## What We Know

### US Forces Anthropic to Disable Frontier Models for Foreign Users

On June 12, the Commerce Department issued an export control directive ordering Anthropic to suspend all access to Fable 5 and Mythos 5 — its two flagship models — for foreign nationals. Anthropic complied but said in a statement it was not given specific details about the national security concern. Reuters and The Guardian confirmed the directive; Fortune reported Anthropic described it as abrupt.

This is the first time the US government has used export controls to restrict access to a commercial AI model mid-deployment rather than at the chip or hardware layer. The practical impact on Anthropic's global enterprise business is significant, since Claude had just taken the lead in enterprise adoption. The lack of transparency in the directive is what makes this different from prior export control moves — companies can't design around a threat they're not told about.

### Microsoft Launches Seven MAI Models at Build 2026

Microsoft AI announced a family of seven in-house models at its Build 2026 conference (June 10–12). The family includes MAI-Thinking-1 (a reasoning model), MAI-Image-2.5 and a Flash variant (now ranked #2 on image editing leaderboards), and MAI Transcribe 1.5. Microsoft claims a tuned MAI model for Excel matches GPT-5.4 performance at up to 10× lower compute cost.

The "hill-climbing machine" framing is notable — Microsoft is explicitly positioning MAI as a continuous improvement program, not a one-time release. This is Microsoft's clearest signal yet that it wants its own model capability rather than permanent dependency on OpenAI.

### Anthropic Passes OpenAI in US Enterprise Adoption

The Ramp AI Index for June 2026 puts Anthropic at 41% of US businesses with paid AI subscriptions — the first time Claude has led OpenAI in that metric. A concurrent $65B Series H round put Anthropic's valuation at $965B. A concurrent IDC survey painted a more mixed picture of Claude's global reach, so the Ramp data likely reflects US-only enterprise spending patterns rather than global market share. The timing matters: this adoption peak arrived the same week the export control directive cut off foreign access to Anthropic's best models.

### KKR Launches $10B Helix Digital Infrastructure

On June 11, KKR launched Helix Digital Infrastructure, a purpose-built data center development company with over $10B in committed long-duration capital. Backers include NVIDIA, Kuwait Investment Authority, and Vistra. The vehicle is led by Adam Selipsky, former AWS CEO. The explicit purpose is to deliver integrated data centers with secured power for hyperscale AI clients. It joins VanEck's new RACK ETF (launched June 2) as evidence that infrastructure capital is now treating AI data center buildout as its own investable category.

### Two AI Governance Moves in Two Weeks

**Executive Order 14409** (June 2): President Trump signed an EO titled "Promoting Advanced Artificial Intelligence Innovation and Security," focused on cybersecurity defense of government information systems and creating a voluntary "early access" framework allowing government agencies to preview frontier models. The EO also establishes new national security and cybersecurity obligations for AI developers.

**Great American AI Act (GAAIA)** (June 4): Reps. Jay Obernolte (R-CA) and Lori Trahan (D-MA) released a bipartisan discussion draft that would create the first comprehensive federal AI framework in the US. Key provisions: codify the Center for AI Standards and Innovation (CAISI) inside Commerce, authorize $100M/year for voluntary security guidelines, and include transparency and audit requirements for AI developers. It's still a discussion draft — but the bipartisan backing is real, and it lands at the same moment the executive branch is using national security tools against AI companies without explanation.

## What's Driving It

**Cybersecurity capability gap concern is real.** Both Anthropic's Mythos and OpenAI's GPT-5.5 Cyber were specifically cited in a Politico piece for "remarkable ability to identify software vulnerabilities and launch cyberattacks." A six-to-twelve month window was cited as the estimate before China reaches comparable frontier model capability in this domain. Whether that estimate is accurate is unclear, but it's the number being circulated in policy circles.

**Open-source closing the gap.** Zhipu AI (China) released GLM-5.2 on June 13 — a fully open-source model with a 1M context window. This continues the pattern of open-source models reaching capability thresholds that were closed-only 6–12 months prior.

**GPT-5.5 line superseded older models.** OpenAI confirmed that GPT-5.2 Instant, GPT-5.2 Thinking, and GPT-5.2 Pro are now deprecated in ChatGPT, with all conversations migrating to GPT-5.5 equivalents. Prediction markets put GPT-5.6 at roughly 80% probability by June 30.

**Data center water and land stress.** The Guardian reported that a majority of new US AI data centers are being sited on drought-affected land. The planned Stratos Project in Utah alone covers roughly 40,000 acres and is projected to draw up to 9 gigawatts. Power and water constraints are starting to bind in siting decisions being made now.

## Implications

**Anthropic's export control problem.** The foreign nationals restriction on Fable 5 and Mythos 5 creates an immediate gap in Anthropic's global enterprise pipeline. If the directive is broad — and the "foreign nationals" language suggests it is — it hits any international employee at a US company, not just foreign-based customers. Anthropic is in an awkward position: it just became the #1 enterprise AI provider in the US by adoption, and simultaneously had its best models turned off for international users without explanation. The $965B valuation assumes global growth. That assumption is now contingent on export control policy.

**Microsoft MAI vs. OpenAI dependency.** The MAI launch at Build is not about competing with OpenAI in the consumer market. It's about Microsoft reducing its unit-cost exposure on Azure AI services and proving out internal capability before the OpenAI partnership terms change. Microsoft's efficiency claims (10× on tuned tasks) are a direct answer to the enterprise AI cost explosion from token-based billing. Watch how fast MAI models land in Microsoft 365 Copilot versus Azure Foundry — that's the real test of whether this is product or positioning.

**Infrastructure capital institutionalizing.** KKR's Helix + NVIDIA + Kuwait Investment Authority + VanEck's RACK ETF arriving in the same week signals that traditional infrastructure capital has finished treating AI data centers as speculative. The water and power constraints mean the bottleneck is increasingly physical, not financial.

**GAAIA legislative trajectory.** The bipartisan framing of the GAAIA is real, but the "discussion draft" label means it's still a long way from law. The federal preemption provisions — which would override state AI laws — are the most contentious element. More immediately, the gap between what the GAAIA proposes (voluntary guidelines, audit frameworks) and what the executive branch just did (unilateral export control of a deployed model) illustrates the coordination problem: legislation is moving at draft speed while enforcement is moving at security speed.

## What to Watch

The export control directive against Anthropic's Fable 5 and Mythos 5 is the most consequential development of the week — not because of what it says, but because of what it doesn't say. When the US government restricts a commercial software product from all foreign nationals without disclosing the rationale, it sets a precedent that every AI company with a global product should be thinking about. The next model restriction might come with more warning. Or it might not. That uncertainty is now a real variable in enterprise AI procurement decisions globally.

The second thing to track: Microsoft MAI versus the OpenAI partnership. The efficiency claims are specific enough to test. If MAI-tuned models are genuinely delivering GPT-5.4 quality at 10× lower compute cost on production tasks, that changes Microsoft's long-term incentive to keep routing enterprise workloads through OpenAI models at scale.

## References

* [Commerce Dept export control directive on Anthropic models](https://www.reuters.com/) — Reuters (June 13, 2026)
* [Microsoft Build 2026 — MAI model family announcement](https://blogs.microsoft.com/ai/) — Microsoft AI Blog (June 10–12, 2026)
* [Ramp AI Index — Anthropic overtakes OpenAI in enterprise adoption](https://ramp.com/blog/ai-index) — Ramp Economics Lab (June 2026)
* [KKR launches Helix Digital Infrastructure](https://www.hpcwire.com/) — HPCwire (June 11–12, 2026)
* [Great American AI Act — bipartisan discussion draft](https://www.politico.com/) — Politico (June 4–10, 2026)
