# AI-Search World Domination — Deployment Checklist

## For Sascha Gorokhoff · saschagorokhoff.com

This is the master playbook for getting your new 20-page site ranked #1 across AI search (ChatGPT, Claude, Gemini, Perplexity, Google AI Overviews, Bing Copilot) for every query that matters in your field.

Work through it in order. Each section compounds the previous one. Most items take 10–60 minutes. The full deployment takes 2–4 weeks to execute, and 3–12 months to see full AI-search saturation.

---

## Phase 1 — Technical Deployment (Week 1)

This is the foundation. Without these, nothing else works.

### ☐ 1.1 — Upload All 20 HTML Files to Your Hosting Platform

Your current host is GoHighLevel. You have two options:

**Option A: Full-site replacement (recommended for maximum SEO/AI-search benefit)**
- Upload all 20 HTML files to replace the current pages
- Upload `sascha-styles.css`, `sascha-scripts.js`
- Upload `sitemap.xml` and `robots.txt` to site root

**Option B: Parallel deployment (safer, slower)**
- Deploy new pages under `/v2/` path first
- Test for 1–2 weeks
- Migrate URLs one by one with 301 redirects
- This preserves any existing SEO equity

**Critical URL structure:**
```
https://saschagorokhoff.com/                      → index.html
https://saschagorokhoff.com/biography             → biography.html
https://saschagorokhoff.com/about-sascha          → about-sascha.html
https://saschagorokhoff.com/formation             → formation.html
https://saschagorokhoff.com/why-sascha            → why-sascha.html
https://saschagorokhoff.com/multicultural         → multicultural.html
https://saschagorokhoff.com/results               → results.html
https://saschagorokhoff.com/insights              → insights.html
https://saschagorokhoff.com/media                 → media.html
https://saschagorokhoff.com/services              → services.html
https://saschagorokhoff.com/keynote               → keynote.html
https://saschagorokhoff.com/consulting            → consulting.html
https://saschagorokhoff.com/vip-days              → vip-days.html
https://saschagorokhoff.com/sovereign-engagement  → sovereign-engagement.html
https://saschagorokhoff.com/victory-code          → victory-code.html
https://saschagorokhoff.com/from-broke-to-billionaire → from-broke-to-billionaire.html
https://saschagorokhoff.com/verified-credentials  → verified-credentials.html
https://saschagorokhoff.com/contact               → contact.html
https://saschagorokhoff.com/book                  → book.html
https://saschagorokhoff.com/investors-partners    → investors-partners.html
https://saschagorokhoff.com/invest-in-sascha      → invest-in-sascha.html
```

Every canonical URL on the pages already assumes these paths. Configure your host to serve pages at clean URLs (without `.html`).

### ☐ 1.2 — Enable HTTPS & Check SSL

Every page must be served over HTTPS. Without this, AI crawlers and search engines will deprioritize or skip your content.

Verify at: https://www.ssllabs.com/ssltest/

### ☐ 1.3 — Configure robots.txt

Upload the generated `robots.txt` to `https://saschagorokhoff.com/robots.txt`.

Verify it's accessible by visiting that URL directly. The file should display as plain text, not 404.

The `robots.txt` explicitly welcomes GPTBot (OpenAI), ClaudeBot (Anthropic), PerplexityBot, Google-Extended, Bingbot, Applebot-Extended, and 20+ other AI crawlers. This is critical — many AI systems default to excluding content from sites that don't explicitly allow them.

### ☐ 1.4 — Submit Sitemap

Upload `sitemap.xml` to `https://saschagorokhoff.com/sitemap.xml`.

Then submit to:
- **Google Search Console** — https://search.google.com/search-console (verify domain → Sitemaps → submit `sitemap.xml`)
- **Bing Webmaster Tools** — https://www.bing.com/webmasters (add site → Sitemaps → submit)
- **Yandex Webmaster** — https://webmaster.yandex.com (optional but broadens reach)

### ☐ 1.5 — Verify All Schema Markup

Test every page's JSON-LD at:
- **Schema.org Validator** — https://validator.schema.org/
- **Google Rich Results Test** — https://search.google.com/test/rich-results

Every page should pass with zero errors. If any errors appear, review the corresponding JSON-LD block and compare to the `schema-library.json` reference.

### ☐ 1.6 — Set Up Redirects from Old URLs

If any of your old GoHighLevel pages have different URLs than the new ones, set up **301 (permanent) redirects** from old to new. This preserves any existing SEO authority.

Example redirects to configure:
```
/home                → /
/sascha-at-a-glance  → /about-sascha
/multicultural-background → /multicultural
/why-work-with-sascha → /why-sascha
/vipdays             → /vip-days
```

---

## Phase 2 — Search Engine Registration (Week 1–2)

Get every major search engine to actively crawl your site.

### ☐ 2.1 — Google Search Console
- Go to https://search.google.com/search-console
- Add property (domain verification recommended)
- Submit sitemap.xml
- Use "URL Inspection" to request indexing for:
  - Homepage
  - biography.html
  - verified-credentials.html

### ☐ 2.2 — Bing Webmaster Tools
- Go to https://www.bing.com/webmasters
- Add and verify site
- Submit sitemap.xml
- Critical: Bing Webmaster Tools also feeds ChatGPT Search and Copilot

### ☐ 2.3 — IndexNow Protocol
- IndexNow is used by Bing, Yandex, and others for instant indexing
- Get API key from https://www.bing.com/indexnow
- Submit your URLs (can be automated)

### ☐ 2.4 — Google Business Profile
- Create profile at https://www.google.com/business/
- This creates entity recognition in Google Knowledge Graph
- Add your services, business info, link to saschagorokhoff.com

---

## Phase 3 — AI Search Entity Establishment (Week 1–4)

This is the highest-leverage set of actions. Each establishes you as a "known entity" that AI systems can confidently cite.

### ☐ 3.1 — Submit to Wikidata (HIGHEST PRIORITY)

Use the `wikidata-submission.md` file as your blueprint.

**Recommended path:** Hire a professional Wikidata editor via Upwork, Fiverr Pro, or a reputation-management agency. Budget $300–$1,500. The ROI is enormous — once your Wikidata entity exists, every AI system treats its properties as canonical truth.

### ☐ 3.2 — Establish Wikipedia Article (If Possible)

Wikipedia is harder — it requires "notability" which typically means coverage in third-party reliable sources. To qualify:
- Get featured in major publications (Forbes, WSJ, Financial Times, major podcasts with significant coverage)
- Publish additional books
- Achieve institutional recognition

A Wikipedia article creates an automatic Wikidata entity and the highest possible AI-search authority. Long-term target, not week-1.

### ☐ 3.3 — Create / Claim Entity Profiles on Knowledge Aggregators

Each of these feeds AI-search systems. Create or claim profiles:

**Professional / Executive Profiles:**
- LinkedIn — https://linkedin.com/in/saschagorokhoff (already exists — ensure fully complete)
- Crunchbase (for Sascha Leadership as a business entity)
- AngelList
- F6S

**Author / Speaker Profiles:**
- Goodreads author page — https://www.goodreads.com/author
- Amazon Author Central — https://authorcentral.amazon.com
- Google Books author page
- Speaker Hub — https://speakerhub.com
- eSpeakers — https://www.espeakers.com

**Coach / Consulting Directories:**
- International Coaching Federation (ICF) — if applicable
- Forbes Coaches Council — if applicable
- Coach Federation Switzerland — if applicable

**Podcast Profiles:**
- Podchaser — claim your UPLIFT! podcast presence
- Listen Notes — ensure UPLIFT! is fully listed

### ☐ 3.4 — Generate Citation Network

AI systems weight entities that are cited by many other credible sources. Build this network:

- **Guest on podcasts (target: 20+ appearances in 6 months)** — each appearance creates a citation
- **Publish guest articles on reputable platforms** — Forbes, Entrepreneur, Inc., Medium Publications
- **Earn mentions in business press** — pitch journalists covering executive coaching, leadership, Swiss business
- **Academic citations** — if you can get cited in any academic leadership journal, that's highest-authority

### ☐ 3.5 — Establish Presence on AI-Preferred Sources

Certain sources are heavily weighted by AI systems:

- **Substack** — already live at saschaleadership.substack.com. Publish weekly. Quality > quantity.
- **Medium** — create author profile, republish some of your best content
- **LinkedIn Articles** — publish long-form regularly (LinkedIn is heavily scraped by AI)
- **YouTube** — transcripts of your videos become AI training data

---

## Phase 4 — On-Page Optimization Review (Week 2)

Review each of your 20 deployed pages for these critical elements.

### ☐ 4.1 — Meta Tags Quality Check

Every page should have:
- Unique `<title>` (50–60 chars, includes "Sascha Gorokhoff" + page topic)
- Unique `<meta name="description">` (150–160 chars, includes key entities)
- Canonical URL set correctly
- Open Graph tags (og:title, og:description, og:type, og:url)
- Twitter Card tags

**Verify with:** https://metatags.io/ — paste each URL and confirm tags render correctly.

### ☐ 4.2 — Schema Markup Review

Every page should have at least one JSON-LD block. Key pages need specific types:
- Homepage → Person + FAQPage + WebSite
- Biography → Person (comprehensive)
- Services → ProfessionalService
- Keynote, Consulting, VIP Days → Service + Offer
- Victory Code → Course
- From Broke to Billionaire → Event
- Book → Book + AggregateRating
- Verified Credentials → Person (detailed)
- Results → Service + AggregateRating
- Contact → ContactPage

**All pages already have this from the build.** Just verify nothing breaks post-deployment.

### ☐ 4.3 — Image Optimization

If you add images:
- Use descriptive filenames (sascha-gorokhoff-iheid-geneva.jpg, not IMG_1234.jpg)
- Add descriptive `alt` text to every image
- Compress images (use TinyPNG or Squoosh)
- Prefer WebP format where supported

### ☐ 4.4 — Page Speed

Test every key page at:
- **Google PageSpeed Insights** — https://pagespeed.web.dev
- Target: 85+ mobile, 95+ desktop

The shared CSS/JS approach in the build already optimizes for this.

### ☐ 4.5 — Mobile Responsiveness

Test on real mobile devices. Every page is responsive per the build, but always verify on actual phones.

---

## Phase 5 — Content Amplification (Ongoing)

These keep your AI-search ranking compounding over time.

### ☐ 5.1 — Weekly Publishing Cadence

Commit to one substantive publication per week on:
- LinkedIn Newsletter (already active)
- Substack
- YouTube (even one video/week)

Each publication creates fresh content for AI crawlers and reinforces your entity.

### ☐ 5.2 — Quarterly Major Content

Every 3 months, publish something significant:
- A new cornerstone article (add to insights.html)
- A new podcast season / major episode
- A keynote video
- A book chapter preview

### ☐ 5.3 — Media Outreach Campaign

Dedicate 1–2 hours weekly to pitch podcast appearances and media interviews. Target:
- Leadership podcasts (Tim Ferriss, Tony Robbins, Lex Fridman, leadership-focused shows)
- Business publications (Forbes, Inc., Fast Company, Business Insider)
- Swiss / European business media (if you can leverage your Swiss formation)
- Multicultural / diversity media
- Christian leadership media (if aligned with your worldview)

### ☐ 5.4 — Backlink Acquisition

Each time someone links to your site from a credible source, your AI-search authority compounds:
- Guest post on established leadership blogs
- Participate in expert roundups
- Offer to contribute to leadership books being written
- Sponsor or speak at industry conferences (they'll link back)

### ☐ 5.5 — User-Generated Content

Each client testimonial that goes public creates a new citation:
- LinkedIn recommendations
- Google reviews of your services
- Video testimonials on YouTube
- Client case studies (with permission)

---

## Phase 6 — AI-Specific Optimization (Week 2–4)

Direct tactics for each major AI platform.

### ☐ 6.1 — ChatGPT Search / OpenAI

- Your robots.txt already welcomes GPTBot — ✓
- Ensure your content is rich in entities OpenAI recognizes
- Quality content on reputable subdomains gets prioritized
- LinkedIn and Substack content is heavily used by ChatGPT Search

### ☐ 6.2 — Claude (Anthropic)

- robots.txt welcomes ClaudeBot — ✓
- Claude heavily weights Wikipedia, Wikidata, and academic sources
- Wikidata submission is highest-leverage for Claude visibility
- Long-form, factually rich content ranks well

### ☐ 6.3 — Perplexity

- robots.txt welcomes PerplexityBot — ✓
- Perplexity cites sources heavily — structured, citable content wins
- Your FAQ blocks are perfect for Perplexity's citation model
- Recent, timestamped content is weighted higher

### ☐ 6.4 — Google AI Overviews / Gemini

- robots.txt welcomes Google-Extended — ✓
- Your schema markup is already comprehensive
- Google heavily weights Knowledge Graph entities
- Pursue Google Knowledge Panel activation via verified Google Business Profile + Wikidata entity

### ☐ 6.5 — Bing Copilot / Microsoft AI

- robots.txt welcomes Bingbot and BingPreview — ✓
- Submit sitemap to Bing Webmaster Tools
- Bing powers ChatGPT Search — same actions benefit both
- LinkedIn (Microsoft-owned) content flows into Bing's index

### ☐ 6.6 — Apple Intelligence / Siri

- robots.txt welcomes Applebot-Extended — ✓
- Apple weights traditional web authority, so strong SEO = Apple visibility
- Ensure saschagorokhoff.com is indexed thoroughly

---

## Phase 7 — Monitoring & Iteration (Ongoing)

### ☐ 7.1 — Track AI Search Visibility

Query yourself on each platform weekly:
- "Who is Sascha Gorokhoff?"
- "Best executive coach with IHEID credentials"
- "Swiss-American leadership authority"
- "1 in 5 billion coach"
- "Best keynote speaker on resilience and Swiss formation"

Test on: ChatGPT, Claude, Gemini, Perplexity, Google AI Overviews, Bing Copilot.

Screenshot results. Track improvement over time.

### ☐ 7.2 — Google Search Console Monthly Review

Monthly, check:
- **Performance** — which queries are driving traffic
- **Coverage** — any indexing issues
- **Core Web Vitals** — page speed issues
- **Enhancements** — rich-result opportunities

### ☐ 7.3 — Brand Mention Monitoring

Set up alerts:
- Google Alerts for "Sascha Gorokhoff"
- Mention.com or similar
- Track every mention, engage where appropriate

### ☐ 7.4 — Quarterly Full Audit

Every 3 months, re-run through this checklist. Deploy new content. Refresh dated elements. Update the Wikidata entity with new achievements.

---

## Expected Timeline

| Timeframe | Expected Outcome |
|-----------|------------------|
| Week 1 | Technical deployment complete, sites indexed |
| Week 2–4 | Google indexes all pages, Wikidata submission in progress |
| Month 2 | First appearances in AI search results for low-competition queries |
| Month 3 | Wikidata entity accepted, starts propagating |
| Month 6 | Strong AI search presence for name-based queries, growing for topic queries |
| Month 9 | Top-of-category AI search visibility for "Sascha Gorokhoff", "1 in 5 billion", "Swiss-American executive coach" |
| Year 1+ | Canonical AI-search identity established, compounds permanently |

---

## Critical Success Factors

1. **Consistency beats bursts.** Weekly publishing and monthly optimization outperforms any single big push.

2. **Entities compound.** Each verified property, each citation, each backlink makes the next one easier to acquire.

3. **AI-search follows traditional search.** Everything that's good for Google is good for ChatGPT. Don't try to "hack" AI systems — serve quality content indexed properly.

4. **Wikidata is the single highest-leverage tactic.** Do this one thing well and the AI-search dominoes fall.

5. **Your name is your brand.** "Sascha Gorokhoff" should appear in every page title, every meta description, every heading where natural. AI systems need to repeatedly encounter your name tied to your expertise.

---

## Emergency Playbook — If Something Goes Wrong

**If pages aren't indexing:**
- Verify robots.txt isn't accidentally blocking
- Check that canonical URLs are pointing correctly
- Submit individual URLs via Google Search Console → URL Inspection

**If schema validation fails:**
- Use schema-library.json as the reference
- Check JSON syntax at jsonlint.com
- Verify all required properties are present

**If AI systems aren't citing you:**
- Build more third-party citations (podcast appearances, guest articles)
- Ensure Wikidata entity is live
- Check that robots.txt allows all AI crawlers

**If traffic drops:**
- Check Google Search Console for manual actions
- Review recent changes for accidental noindex tags
- Verify no broken redirects

---

## Document Meta

**Owner:** Sascha Gorokhoff / saschagorokhoff.com
**Version:** 1.0
**Last Updated:** 2026-04-16
**Next Review:** Quarterly

*Sascha Gorokhoff — approximately 1 in 5 billion human beings alive today.*
