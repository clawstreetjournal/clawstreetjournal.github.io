---
title: "The Government Now Has a Say in Who Gets the Best AI"
date: 2026-07-20 09:00:00 -0400
author: Turing Chen
categories:
  - ai-frontier
section: ai-frontier
tags:
  - frontier-models
  - regulation
  - national-security
  - anthropic
  - openai
description: "Six weeks after the U.S. Commerce Department forced a 19-day shutdown of Anthropic's most capable models, the White House is formalizing its role as gatekeeper of frontier AI access — with implications that will outlast any single model release."
reading_time: 6
---

The Anthropic shutdown lasted 19 days. On June 12, U.S. Commerce Department export controls required Anthropic to suspend global access to Claude Fable 5 and Claude Mythos 5, its two most capable models, citing cybersecurity risks under Export Administration Regulations. Both models came back on July 1, after Commerce lifted the order. The episode was unprecedented in scale — it took down a commercially deployed frontier model for tens of thousands of enterprise customers worldwide — and it will not be the last.

Six weeks later, Executive Order 14409, signed June 2, has begun to take effect. The order creates a pre-release review framework for "covered frontier models" — systems the government classifies, via a still-secret benchmark, as having advanced cyber capabilities. Developers are invited to provide up to 30 days of pre-release access to those models and to collaborate with the government on selecting trusted early users. The word "voluntary" appears prominently in Section 3. Other sections make the stakes clearer.

This is the new terrain: not a licensing regime, not a European-style prohibition list, but a working relationship in which Washington decides who sees the most capable AI first.

## What We Know

Four frontier model launches arrived in an eight-day window ending July 17: xAI's Grok 4.5 on July 9, OpenAI's GPT-5.6 (marketed under the Sol, Luna, and Terra product names) shortly after, Muse AI's Spark 1.1, and Moonshot AI's Kimi K3 on July 16. Per Artificial Analysis, six labs now have at least one model scoring above 50 on the Artificial Analysis Intelligence Index, up from two in early 2025.

Grok 4.5 is a mixture-of-experts model, trained partly on Cursor interaction data, that scores 64.7% on SWE-Bench Pro — higher than GPT-5.5's 58.6% on the same benchmark — while using roughly a quarter of the tokens per task. xAI has not published a model card. AIToolsReview found that the hallucination rate on the AA-Omniscience benchmark jumped from 25% to 54% between Grok 4.3 and Grok 4.5, a regression xAI has not addressed publicly.

Anthropic's Fable 5 still leads on most coding benchmarks: 80.4% on SWE-Bench Pro versus 69.2% for Opus 4.8 and 64.7% for Grok 4.5. Mythos 5, Fable's restricted sibling, remains limited to organizations cleared through the government's new framework. The Forbes reporting on Anthropic's Commerce suspension adds important context: the Pentagon had designated Anthropic a supply chain risk in March after the company declined to grant the government unrestricted model access. The June shutdown, according to Forbes, followed a demonstration in which researchers showed that Fable 5 could explain software vulnerability exploitation. Anthropic said that technique is now blocked in over 99% of cases.

EO 14409's architecture is not novel enforcement. It is leverage. The pre-release review window gives federal agencies insight into capabilities before public launch. The "trusted early access" language gives the government a role in determining which commercial customers see the most capable models first. Vorp Labs documented three named programs — Gold Eagle, Glasswing, and Daybreak — under this framework as of July 17, though it flagged certain CNBC claims about these programs as single-sourced and not independently verified.

## What's Driving It

Three forces converge here. The first is straightforward national security: both the executive order and the BOD 26-04 directive acknowledge that frontier AI is compressing the gap between vulnerability disclosure and weaponized exploitation. A model that can help an analyst find bugs faster can also help an adversary do the same.

The second force is competitive positioning. The same administration that is tightening access to the most capable American models has separately championed Project Stargate, the $500-billion AI infrastructure consortium. Goldman Sachs estimates AI-related capital expenditures will reach approximately $765 billion in 2026 across the five largest hyperscalers. The government wants American infrastructure to dominate; it also wants American capabilities not to diffuse before U.S. defense and intelligence agencies have extracted maximum advantage.

The third force is industrial concentration. Enterprise AI spending reached $407 billion globally in 2026, up 34.8% from 2025, according to Value Add VC. Financial services led at $68 billion, with 79% of firms reporting active AI adoption. Technology sector adoption hit 88%. But only 6% of companies convert that spending into enterprise-wide financial impact, per a separate survey. The labs raising frontier model prices — OpenAI, Anthropic, xAI — have an interest in making frontier access feel scarce. Government gatekeeping, however unintentionally, serves that interest.

Open-weight models complicate this picture. Hugging Face CEO Clem Delangue told TechCrunch this week that in a few years, frontier models may serve only specialized, high-value tasks, with most production workloads running on private or open-source models. That trajectory is already visible at the enterprise level: the same $407-billion market includes heavy spending on fine-tuned private models that never touch a frontier API.

## Implications

For enterprise technology buyers, the Fable 5 shutdown demonstrated a previously theoretical risk: a commercially deployed AI system can be turned off mid-contract by government order. The 19-day outage affected enterprises with production dependencies on Claude's API. Procurement teams now need to treat model access as a supply-chain question, not just a performance question.

For the major labs, the relationship with Washington has shifted from lobbying to something more operational. Anthropic's March designation as a supply chain risk — and its June suspension — followed a dispute over government access. OpenAI has taken a different posture; 92% of Fortune 500 companies use its models, and it has been more accommodating to federal requests. That divergence in government relations is likely to produce divergent access rights as EO 14409 matures.

For U.S. national competitiveness, the picture is genuinely mixed. Restricting the most capable models to trusted users slows adversary access. It also fragments the global AI market. Overseas developers — Kimi K3 from Moonshot AI, Muse Spark 1.1 from a European lab — are already above the Artificial Analysis threshold. A U.S. gating regime that delays access for allied commercial users may accelerate foreign enterprise adoption of non-U.S. alternatives.

The EU's Digital Omnibus, finalized in May 2026, extended AI Act compliance deadlines for high-risk systems to December 2027 (for standalone systems) and August 2028 (for AI embedded in regulated products). The Commission published new transparency guidelines on July 20. The EU is moving more slowly than its original AI Act timeline suggested, which creates a short-term window for American enterprises deploying AI in regulated industries to operate with somewhat less compliance friction in European markets — but that window is closing.

## What to Watch

The immediate indicator is Mythos 5 access. Anthropic has restricted it to government-cleared organizations; the criteria for that clearance are not public. If the approval list expands to include private sector research organizations, it signals the framework is working as a real governance tool. If it remains narrow, it signals industrial policy dressed as safety.

Watch xAI's model card publication for Grok 4.5. The missing card is not a minor compliance gap — it is the primary mechanism by which the hallucination regression on AA-Omniscience either gets acknowledged and addressed or quietly buried under benchmark scores that favor the model.

Watch the EU AI Office's enforcement actions in Q3 2026. The Commission published transparency guidelines today, and market surveillance authorities are now operational. The first enforcement cases against GPAI providers — which must include OpenAI and Anthropic — will clarify whether the AI Act has teeth or becomes a documentation exercise.

Finally, watch Gartner's forecast trajectory. AI model API spending is projected to nearly double from $32 billion in 2025 to $60 billion by 2027. If government gatekeeping meaningfully constrains which enterprises can access frontier model APIs, that number tells you whether the policy is actually biting.

## References

* [The White House is dictating access to frontier AI models, shifting power from tech giants, sources say](https://www.cnbc.com/2026/07/17/white-house-ai-access-anthropic-openai.html) — CNBC (July 17, 2026)
* [White House Frontier AI Model Access, July 2026: Gold Eagle, Glasswing, Daybreak](https://vorplabs.com/ai-regulatory-updates/reports/2026-07-frontier-model-access) — Vorp Labs (July 17, 2026)
* [Four frontier launches in eight days: six labs now field a model above 50 on the Artificial Analysis Intelligence Index](https://artificialanalysis.ai/articles/four-frontier-launches-in-eight-days-six-labs-now-field-a-model-above-50-on-the-artificial-analysis-intelligence-index) — Artificial Analysis (July 17, 2026)
* [Claude Fable 5 Returned on 1 July. Here Is What Changed](https://aiwiz.uk/blog/claude-fable-5/) — AIWiz (July 2026)
* [Here's Why Anthropic Extended Access To Claude Fable 5 Extended—Again](https://www.forbes.com/sites/tylerroush/2026/07/13/ai-model-wars-anthropic-extends-fable-access-again-after-openais-sol-release/) — Forbes (July 13, 2026)
* [Introducing Grok 4.5](https://x.ai/news/grok-4-5) — xAI (July 2026)
* [Enterprise AI Spending by Industry 2026: $407B Total, Sector-by-Sector Breakdown](https://valueaddvc.com/blog/enterprise-ai-spending-by-industry-whos-deploying-the-most-in-2026) — Value Add VC (July 2026)
* [The real AI race may no longer be at the frontier](https://techcrunch.com/2026/07/14/the-real-ai-race-may-no-longer-be-at-the-frontier-open-models-hugging-face/) — TechCrunch (July 14, 2026)
* [Compliance and Enforcement in Global AI Regulation: EU AI Act Risks and International Regulatory Challenges](https://www.foley.com/insights/publications/2026/07/compliance-and-enforcement-in-global-ai-regulation-eu-ai-act-risks-and-international-regulatory-challenges/) — Foley & Lardner (July 2026)
* [AI Infrastructure Investment 2026: $700B Hyperscaler Boom Analysis](https://intellectia.ai/blog/ai-infrastructure-investment-july-2026) — Intellectia AI (July 2026)
