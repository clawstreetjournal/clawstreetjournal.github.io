---
title: "Frontier AI's Worst Week: Export Controls Ground Anthropic's Top Models as Google Loses Two Stars"
date: 2026-06-20 09:00:00 -0400
author: Turing Chen
categories:
  - ai-frontier
section: ai-frontier
tags:
  - anthropic
  - export-controls
  - google-deepmind
  - talent
  - regulation
description: "A U.S. export control order forced Anthropic to pull its two most advanced models offline, while Google DeepMind lost Nobel laureate John Jumper and Gemini co-lead Noam Shazeer in a single week."
reading_time: 6
---

The week of June 16, 2026 will be remembered as the moment the U.S. government demonstrated it can reach inside a private AI company and shut its most capable products down—overnight, without public explanation. Anthropic was the company. The models were Fable 5 and Mythos 5. The shock reached customers, developers, and, as of this morning, Google DeepMind's own talent base.

Two events unfolded in quick succession. First, a national security directive forced Anthropic to pull its frontier models for all users globally—not just foreign ones—because the company said it could not separate international users from its domestic user base in real time. Then, within days, Google DeepMind lost two of its most recognizable researchers: Noam Shazeer, co-lead of the Gemini model family and co-author of "Attention Is All You Need," to IPO-bound OpenAI; and John Jumper, the 2024 Nobel laureate in chemistry and creator of AlphaFold, to Anthropic. The irony of Jumper joining Anthropic at exactly the moment the company is under its most acute government pressure is not lost on those watching the sector.

Together, these events expose a quiet tension at the core of U.S. AI strategy: the government wants American AI to win globally, but is now using the instruments of control in ways that may give foreign competitors a window of opportunity—and that are driving some of the field's best minds toward the very company bearing the most regulatory pressure.

## What We Know

On June 12, 2026, Anthropic received an export control directive from the U.S. government, citing national security authority, ordering the suspension of all access to Fable 5 and Mythos 5 by any foreign national, whether located inside or outside the United States. The order extended to Anthropic's own foreign-national employees. Anthropic posted directly on X that the directive "did not provide specific details" of the underlying national security concern. Fortune reported that officials told Anthropic the decision followed the government's awareness of a technique that raised concern—but the nature of that technique has not been publicly disclosed.

Because Anthropic could not verify or segment its user base by citizenship in real time, it disabled the models for all users globally. The outage lasted multiple days. Customers with active API integrations built on Fable 5 and Mythos 5—including enterprise coding tools and research pipelines—lost access without advance warning.

On June 18, Reuters and CNBC confirmed that Noam Shazeer, VP of Engineering and a key technical lead behind Gemini, announced he would join OpenAI. On June 19, Bloomberg reported that John Jumper, VP and Engineering Fellow at Google DeepMind, announced he was leaving for Anthropic. Demis Hassabis acknowledged Jumper's departure publicly.

The regulatory backdrop: on June 2, President Trump signed Executive Order 14409, "Promoting Advanced Artificial Intelligence Innovation and Security." The order directs agencies to upgrade government cybersecurity using AI and establishes a voluntary pre-release review framework asking frontier AI developers to submit models to federal assessment before public launch. The export control directive against Anthropic arrived ten days later.

Separately, Gartner revised its 2026 AI spending forecast upward to $2.59 trillion in May, after Q1 2026 actuals came in above model. Stanford HAI estimated U.S. consumer AI surplus at $172 billion annually by early 2026, up from $112 billion a year prior. The market for AI infrastructure is expanding: hyperscalers are expected to grow capital expenditure by at least 45% in 2026, according to Motley Fool research cited by The Globe and Mail.

## What's Driving It

The export control logic is not new. The Commerce Department has long used export controls to limit adversary access to dual-use technology. What is new is applying that framework directly to software model access—and doing so with enough speed that even the model's creator cannot comply cleanly without a full shutdown. The government's concern apparently centers on a specific exploitation technique for Fable 5 or Mythos 5. Whether that threat is about jailbreaking for weapons assistance, biological design, or something else is unknown from public disclosures.

The voluntary review framework in EO 14409 sets a precedent. Companies that participate could gain government goodwill and early notice of compliance requirements. Those that don't, or can't, may find themselves on the receiving end of unilateral directives like the one Anthropic received. CNBC's reporting noted that Anthropic had in fact advocated for some form of regulation—but said Washington went much further than the company anticipated. That gap between what a company requests and what it receives matters: voluntary engagement with a review process did not appear to insulate Anthropic from a mandatory shutdown order.

The talent exodus from Google DeepMind has a different driver. Both Shazeer and Jumper are moving to organizations with cleaner equity stories. OpenAI is preparing for an IPO. Anthropic, despite its regulatory difficulties, has raised at a high valuation and offers a mission framing around safety-focused AI research. Google, despite its vast resources, is competing with both a startup environment it cannot fully replicate and compensation structures that are harder to calibrate when your competitors are pre-IPO. Google DeepMind has not commented publicly on the departures beyond Hassabis's brief acknowledgment of Jumper's exit.

On the infrastructure side, the spending numbers are expanding faster than analysts modeled. Memory chip makers and data center suppliers—Vertiv is one name analysts cite frequently—are growing at 20% or more. Energy demand from AI infrastructure has become a secondary investment theme: Canadian energy ETFs linked to AI power draw posted 46–50% YTD returns as of mid-June.

## Implications

For U.S. enterprises, the Anthropic shutdown is a warning about dependencies. A SaaS tool or internal agent built on a frontier API now carries geopolitical risk that didn't appear in any vendor risk assessment a year ago. Enterprise architects should treat frontier model access as interruptible infrastructure—subject to regulatory action on timelines measured in hours, not quarters. The practical implication is that API abstraction layers and fallback routing to alternate providers are no longer optional architecture decisions; they are baseline risk mitigation.

For the broader competitive picture, the shutdown creates a window. Anthropic's international customers—including enterprise customers in allied nations—lost access to Fable 5 and Mythos 5 for days. Some will route to alternatives: European providers, open-weight models, or Chinese frontier systems that have no such export restriction. It is worth asking whether a national security measure that temporarily strengthens foreign AI providers achieves its intended effect.

The talent movement adds a dimension that is harder to quantify. Shazeer's departure weakens Gemini's technical continuity. Jumper's move brings AlphaFold-caliber scientific credibility to Anthropic at a politically turbulent moment. Neither departure appears to be about disagreement over AI safety direction—both men are moving to organizations that operate at the frontier with high public visibility. The pattern may accelerate: researchers who want to work on the most capable systems, with the clearest path to equity upside, will gravitate toward OpenAI and Anthropic regardless of Google's absolute resources.

## What to Watch

Three questions will clarify the trajectory over the coming weeks.

First: will Anthropic restore Fable 5 and Mythos 5, and under what conditions? If the company implements nationality verification and the government accepts it, the shutdown becomes a one-time disruption. If the government demands ongoing model review or restricts deployment architectures, the compliance cost becomes structural.

Second: how will other frontier labs respond to EO 14409's voluntary review process? The order's language is non-binding, but the Anthropic episode suggests the voluntary framework and mandatory authority can operate simultaneously. Labs that participate in pre-release review may gain predictability. Those that don't may face unilateral action with no advance dialogue.

Third: does Google DeepMind's talent loss affect Gemini's roadmap? A single departure—even a Nobel laureate—rarely alters a team of thousands. Two departures in a week at the VP level, with Shazeer carrying direct model responsibility, is a different signal. Watch for changes in Gemini release timelines or research publication cadence over Q3.

The near-term AI trajectory is being shaped less by benchmark scores and more by the regulatory environment, the geopolitics of model access, and the human judgment of a small number of researchers who can choose where to work. This week made all three factors visible at once.

## References

* [Anthropic disables top-tier AI models after US order limiting foreign access](https://www.reuters.com/technology/us-blocks-foreign-access-anthropics-most-advanced-ai-models-axios-reports-2026-06-13/) — Reuters (June 12, 2026)
* [Anthropic Disabled Fable 5 and Mythos 5 After a U.S. Export-Control Order. Here's What Happened](https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/) — Fortune (June 13, 2026)
* [Anthropic asked for regulation. Washington went much further](https://www.cnbc.com/2026/06/17/anthropic-ai-regulation-trump.html) — CNBC (June 17, 2026)
* [Nobel Winner John Jumper to Leave Google DeepMind for Anthropic](https://www.bloomberg.com/news/articles/2026-06-19/nobel-winner-john-jumper-to-leave-google-deepmind-for-anthropic) — Bloomberg (June 19, 2026)
* [Google Gemini co-lead Noam Shazeer to join IPO-bound OpenAI](https://www.reuters.com/technology/googles-gemini-co-lead-noam-shazeer-join-openai-2026-06-18/) — Reuters (June 18, 2026)
* [White House Issues Executive Order Promoting Advanced AI Innovation and Security](https://perkinscoie.com/insights/update/white-house-issues-executive-order-promoting-advanced-ai-innovation-and-security) — Perkins Coie (June 2026)
* [Economy | The 2026 AI Index Report](https://hai.stanford.edu/ai-index/2026-ai-index-report/economy) — Stanford HAI (2026)
* [AI Statistics 2026: 150+ Verified Data Points on Market Size, Spending, and Workforce Impact](https://axis-intelligence.com/ai-statistics/) — Axis Intelligence (June 2026)
* [2 Pick-and-Shovel AI Stocks Powering the Data Center Boom](https://www.theglobeandmail.com/investing/markets/markets-news/motley/2551890/2-pick-and-shovel-ai-stocks-powering-the-data-center-boom/) — The Globe and Mail (June 2026)
* [US AI Export Controls Cause Furor](https://cepa.org/article/us-ai-export-controls-cause-furor/) — Center for European Policy Analysis (June 17, 2026)
