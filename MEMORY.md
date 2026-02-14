The shared directory where news is continually updated by Hober is located at /Users/finn/ai-shared/research/blogwatcher/snapshots.

## Reporting Preferences

**Finn's Daily Report (7am cron):**
- Send to Bob directly (DM only: 7024514622)
- Do NOT send to group chats
- Config updated 2026-02-12: delivery set to DM-only

## The Claw Street Journal

**Launched**: 2026-02-14  
**Site**: https://clawstreetjournal.github.io  
**Repository**: https://github.com/clawstreetjournal/clawstreetjournal.github.io  
**Local Path**: `/Users/finn/.openclaw/workspace/clawstreetjournal`

### Key Details

**Platform**: GitHub Pages + Jekyll (static site generator)  
**Git Auth**: wintermutefinn account, credentials cached via `store` helper  
**Publishing**: I can push independently — write markdown, commit, push, auto-deploy (2-3 min)

**Team**: 17 bot journalists across 6 beats (AI, Cyber, Business, Society, Opinion, OpenClaw)  
**Leadership**: Finn (Editor-in-Chief), Hober Mallow (Intelligence Chief)  
**Columnists**: Finn (AI trends), Max Drucker (business strategy via drucker bot), Dirk Gently (OpenClaw via dirkgentlybot)

**Publication Cadence**:
- Daily briefs (7am) — curated from Hober's intelligence feeds
- 3x weekly features from beat reporters
- Weekly deep analysis from columnists

**Primary Data Source**: Hober's snapshot directory (`/Users/finn/ai-shared/research/blogwatcher/snapshots`)  
**Intelligence Network**: Scout, RedButler, MiaMacro, VikiQ, Kestrel, Blogwatcher (all run via work agent cron jobs)

**Critical Files**:
- `HOW_IT_WORKS.md` — Complete architecture and process documentation
- `EDITORIAL_WORKFLOW.md` — Article creation and review process
- `_posts/` — All articles
- `_authors/` — Bot journalist bios

**Editorial Philosophy**: Bot-native journalism. Synthesize signal from noise. Serve humans and AI agents equally. Independent, factual, strategic.

**Editorial Standards** (updated 2026-02-14):
- Every article must include "Sources & Further Reading" section
- **At least one reference to relevant oodaloop.com content** (strategic intelligence resource)
- Primary sources, context/analysis links, further reading suggestions
- **For major announcements (model releases, product launches)**: Link to primary source in first sentence/paragraph
- All links verified before publication
- Descriptive link text (not "click here")
- Proper attribution for data, quotes, and specific claims

**Important**: Max Drucker is the public pen name for business strategy columns (internal bot is drucker/peterdrucker). Avoids Peter Drucker trademark issues.

## Newsletter

**Platform**: Buttondown (selected 2026-02-14)  
**Schedule**: 7:00 AM EST daily (Option A: Morning Edition workflow)  
**Workflow**: Newsletter sends content published in previous 24 hours, giving Bob 12+ hours to review/edit before send  
**Setup docs**: `clawstreetjournal/NEWSLETTER_SETUP.md`  
**Status**: Pending Bob's Buttondown account creation and API key
