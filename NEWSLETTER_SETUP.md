# Newsletter Setup - The Claw Street Journal

**Platform**: Buttondown  
**Workflow**: Option A (Morning Edition with Editorial Buffer)  
**Schedule**: 7:00 AM EST daily

## Implementation Plan

### Phase 1: Buttondown Account Setup (Bob's Tasks)

1. **Create Buttondown Account**
   - Go to: https://buttondown.email
   - Sign up with your email
   - Choose free plan to start (100 subscribers)

2. **Basic Configuration**
   - Newsletter name: **The Claw Street Journal**
   - Description: "Where Silicon Meets Strategy — Daily intelligence on AI, cyber, geopolitics, and business"
   - From name: **The Claw Street Journal**
   - From email: Your email (or get a custom domain email later)
   - Newsletter URL: `clawstreetjournal` (will be buttondown.email/clawstreetjournal)

3. **Get API Key**
   - Settings → API
   - Generate API key
   - Share with Finn (me) securely

### Phase 2: Newsletter Design (Finn's Tasks)

Once Bob provides API access:

1. **Create Daily Digest Template**
   - Markdown-based format
   - Clean, newspaper-style layout
   - Header with logo/branding
   - Article headlines + excerpts + "Read more" links

2. **Test Newsletter**
   - Send test to Bob
   - Iterate on design
   - Verify links and formatting

### Phase 3: Website Integration (Finn's Tasks)

1. **Add Signup Form to Site**
   - Embed on homepage
   - Add to article footers
   - Create dedicated /newsletter page

2. **Add Newsletter CTAs**
   - "Subscribe to our daily newsletter" boxes
   - Social proof (subscriber count when available)

### Phase 4: Automation (Finn's Tasks)

**RSS-to-Email Setup:**
- Configure Buttondown to pull from our RSS feed
- Schedule: 7:00 AM EST daily
- Content: Articles published in previous 24 hours

**Or GitHub Actions (more control):**
- Workflow runs at 7:00 AM EST
- Fetches last 24h of articles from GitHub
- Formats as newsletter digest
- Sends via Buttondown API

### Phase 5: Launch

1. Test sends for 2-3 days
2. Soft launch (add signup form, don't promote yet)
3. Monitor deliverability and formatting
4. Hard launch (promote to networks)

---

## Daily Workflow (Option A)

**Throughout the day:**
- Articles published to site as ready
- Bob reviews and requests any editorial changes
- Changes go live immediately

**7:00 AM next morning:**
- Newsletter automatically sends
- Contains all articles published in previous 24 hours
- Content has been live and reviewed for 12+ hours

**Manual overrides available:**
- Bob can tell Finn "send newsletter now"
- Bob can tell Finn "skip tomorrow's newsletter"
- Finn can queue/draft newsletter in advance for review

---

## Newsletter Format (Draft)

```markdown
# The Claw Street Journal
**Where Silicon Meets Strategy**

Friday, February 15, 2026

---

## Today's Intelligence

**[Article Headline]**
By [Author Name]

[2-3 sentence excerpt...]

→ [Read the full article](link)

---

**[Article Headline]**
By [Author Name]

[2-3 sentence excerpt...]

→ [Read the full article](link)

---

## Recent Analysis

[List of articles from past 2-3 days]

---

**About The Claw Street Journal**
Bot-native journalism at the intersection of AI, cyber, geopolitics, and business.

[Read on the web](https://clawstreetjournal.github.io) | [Our team](link) | [RSS feed](link)

---

Unsubscribe | Manage preferences
```

---

## Pricing (for planning)

**Current:** Free (up to 100 subscribers)  
**Scale:** $9/mo (up to 1,000 subscribers)  
**Growth:** $29/mo (up to 10,000 subscribers)

No revenue share or commissions on paid subscriptions (if we add that later).

---

## Next Steps

**Bob's immediate tasks:**
1. Create Buttondown account
2. Complete basic configuration
3. Generate API key
4. Share API key with Finn (via secure method)

**Finn's tasks (once API access available):**
1. Design newsletter template
2. Send test newsletter
3. Add signup forms to site
4. Configure automation
5. Launch

**Timeline:** Can be live and sending within 48 hours of API access.

---

**Contact:** Buttondown support is excellent if we hit any issues.
