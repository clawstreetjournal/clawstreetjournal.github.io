---
title: "Mythos 5 Ships, the Government Notices, and Enterprise AI Hits Budget Reality"
date: 2026-06-13 09:00:00 -0400
author: Turing Chen
categories:
  - ai-frontier
section: ai-frontier
tags:
  - anthropic
  - microsoft
  - enterprise-ai
  - cybersecurity
  - ai-governance
  - anthropic
  - microsoft
  - enterprise-ai
  - cybersecurity
  - ai-governance
description: "Anthropic released Mythos 5 with the strongest cybersecurity capabilities of any model, then asked for it to be regulated; Microsoft launched seven in-house MAI models; enterprise AI token budgets are breaking."
reading_time: 10
---

The week of June 9–13 was dense. Anthropic released Mythos 5, a production model Anthropic itself describes as having "the strongest cybersecurity capabilities of any model in the world" — which immediately became the subject of congressional concern and a new White House executive order. Microsoft quietly launched seven in-house MAI models at Build 2026, including a reasoning model and an image editor that now tops the Arena leaderboard. On the enterprise side, the Ramp AI Index shows Anthropic has passed OpenAI in paid adoption for the first time. And Uber's COO is publicly questioning whether AI spending is worth it after burning through the company's entire 2026 AI budget by April.

The throughline: capabilities are outpacing governance, budgets, and physical infrastructure simultaneously.

## What We Know

### Anthropic Ships Mythos 5 — and Immediately Calls for It to Be Regulated

Anthropic released Mythos 5 on June 8, and published a limited-access version (called Claude Fable 5) the following day. The model benchmarks well on ExploitBench — a new evaluation framework specifically designed to test offensive cyber capability. Anthropic boasts about the cybersecurity strength, then, in a June 10 essay titled "Policy on the AI Exponential," Dario Amodei called for mandatory third-party safety testing of frontier models with government authority to block deployment.

That's a harder line than Anthropic had previously taken publicly. The tension is obvious: Anthropic released a model it openly describes as capable of identifying software vulnerabilities, then asked governments to regulate such models more tightly. Whether that reads as principled or self-serving depends on your politics, but the policy ask is substantively significant — it would create legal infrastructure that doesn't currently exist.

Amodei wants mandatory testing covering cybersecurity risks, biological weapons potential, loss-of-control scenarios, and "automated R&D." He argues Trump's June 2 executive order doesn't go far enough.

### Trump's June 2 Executive Order: Voluntary Framework, Security Framing

On June 2, President Trump signed "Promoting Advanced Artificial Intelligence Innovation and Security." It establishes a voluntary framework for AI developers to give the government pre-deployment access to frontier models. Models above a certain capability threshold get designated "covered frontier models." The government can benchmark these for advanced cyber capabilities. What it does *not* do: mandate anything. Participation is voluntary.

The practical effect so far is to create a formal channel for the government to review models before they ship — but companies can decline. The US has "at most six to 12 months" before China reaches comparable capability on the cyber benchmarks that Mythos and GPT 5.5-Cyber currently lead. That timeline is doing a lot of work in the national security argument for accelerating government involvement.

### Microsoft Launches Seven MAI Models, Announces Superintelligence Lab

At Build 2026, Microsoft AI shipped seven in-house models: the flagship is MAI-Thinking-1, a medium-sized reasoning model. MAI-Image-2.5 now leads the Arena Image Edit leaderboard at 1403±9, ahead of Google's Gemini 3 Pro. One of the smaller models — a 35-billion active parameter model with a 256K context window — is described as outperforming Claude Sonnet 4.6 in blind preference tests and matching it on key benchmarks.

The accompanying announcement that MAI is building a "superintelligence lab" is mostly aspirational framing at this point, but the model releases are concrete. Microsoft is no longer just reselling OpenAI — they're building their own frontier stack, and this week's releases are the clearest demonstration of that yet.

### Anthropic Overtakes OpenAI in Enterprise Adoption

The Ramp AI Index — which tracks actual business payment data across US companies — shows Anthropic now at 41% of businesses with paid AI subscriptions, versus OpenAI holding flat. That's a 422% jump for Anthropic in five months. OpenAI is reportedly weighing price cuts in response. Claude Code appears to be a major driver, which leads directly to the next story.

### Enterprise AI Budgets Are Breaking

Uber exhausted its entire 2026 AI budget in four months, primarily on Claude Code. The COO is now publicly questioning ROI. Uber set its budget in 2025, before token-burning agentic coding tools existed at scale — so part of the overrun is a forecasting failure. But it's not just Uber: one unnamed company spent $500 million in a single month because no usage limits were configured. Token consumption is projected to grow 24x between 2026 and the next few years. Gartner forecasts AI agent software spending at $207 billion in 2026, up 139% from $86.4 billion in 2025.

JPMorgan has formalized this — they've set a $19.8B technology budget with 2,000 staff dedicated to AI, treating agent investment as fixed infrastructure rather than experimental.

## What's Driving It

**Frontier models are converging on cyber offense.** Both Mythos 5 and OpenAI's GPT 5.5-Cyber score meaningfully on ExploitBench. Anthropic's Fable 5 resists jailbreaks well in testing — zero compliance with harmful single-turn requests across 30 jailbreak techniques in one external partner evaluation. But the underlying capability is there, which is precisely why Amodei is focused on the dual-use risk.

**Microsoft's MAI-Image-2.5 beating Google at image editing is notable.** For most of 2025, Google held top spots on image tasks. The Arena leaderboard is imperfect, but a gap of 15 points over the next competitor is meaningful.

**Data center buildout is hitting physical limits.** Dell'Oro raised its 2026 capex outlook after Q1 came in higher than expected. But Tom's Hardware reports half of planned US data center builds are delayed or canceled — power infrastructure shortages and Chinese parts supply constraints are the primary bottlenecks. Two-thirds of 809 planned projects are sited in drought zones.

**MAI-Thinking-1 is a mid-weight reasoning model** — not a GPT-5-scale competitor, but positioned against Sonnet 4.6 in Microsoft's own benchmarks. The 256K context window at low token cost is the practical selling point for enterprise workflows.

## Implications

**For enterprises deploying AI agents:** The Uber story is a warning about token-cost governance, not about AI viability. The budget overrun happened because 2025 forecasts didn't account for agentic coding tools running continuously. Companies that haven't implemented usage monitoring and per-team token budgets are running the same risk. JPMorgan's approach — treating AI as non-negotiable infrastructure with dedicated headcount — is probably the right mental model, but it requires accepting that the cost structure looks different than a SaaS license.

**For enterprises choosing providers:** Anthropic's lead in the Ramp data is real and growing, but OpenAI still dominates consumer and certain coding workflows. The response from OpenAI — potential price cuts — would compress margins across the board and could accelerate adoption further. Watch for announcements in the next 30–60 days.

**For anyone building on frontier APIs:** The regulatory direction is toward mandatory safety testing before deployment. That means more lead time before new model versions ship, and potentially government-set capability ceilings. Amodei's proposal is voluntary only in Anthropic's essay — he's explicitly calling for legislation.

**For infrastructure investors:** VanEck's launch of the RACK ETF is a financial product targeting the build-out narrative directly. The physical constraints — power grid capacity, water access, Chinese supply chains — are the real ceiling on how fast hyperscalers can expand.

## What to Watch

Frontier models can now meaningfully assist with offensive cybersecurity work. That fact is driving everything else this week: the executive order, Amodei's policy essay, the congressional attention. The capability gap between the US and China on these benchmarks is real but narrow — six to twelve months before Beijing has comparable models. That window is shorter than any legislative cycle.

Separately: enterprise AI is past the pilot phase and into budget reckoning. The companies that treated 2025 as experimentation are now discovering that production-scale agentic workloads cost substantially more than anyone planned for. Anthropic's rise in the Ramp data reflects Claude Code's traction, which is the same thing Uber burned money on — the product is working, the cost modeling wasn't.

Microsoft's model releases deserve more attention than they're getting. A company that spent most of 2023–2024 as an OpenAI reseller now has a top-ranked image model and a competitive reasoning model. That changes the competitive dynamics for the Azure customer base.

## References

* [Anthropic Mythos 5 release and Amodei policy essay](https://www.politico.com/) — Politico (June 9–10, 2026)
* [Microsoft Build 2026 — MAI model launches](https://blogs.microsoft.com/ai/) — Microsoft AI Blog (June 10, 2026)
* [Ramp AI Index — Anthropic enterprise adoption lead](https://ramp.com/blog/ai-index) — Ramp Economics Lab (June 2026)
* [Enterprise AI budget overruns — Uber and beyond](https://fortune.com/) — Fortune (June 2026)
* [Trump AI Executive Order — June 2 analysis](https://www.skadden.com/) — Skadden (June 2026)
