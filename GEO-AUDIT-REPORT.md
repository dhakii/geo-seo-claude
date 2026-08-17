# GEO Audit Report: 0entropy.top

**Audit Date:** August 17, 2026
**URL:** https://0entropy.top
**Business Type:** Artist/Publisher Archive
**Pages Analyzed:** 8

---

## Executive Summary

**Overall GEO Score: 30/100 (Critical)**

0entropy.top is a minimalist portfolio/archive site with server-side rendered content. However, the site lacks key GEO elements including explicit `llms.txt`, brand recognition across major AI training sources, structured data (Schema.org), and substantive content blocks for AI citability. It requires foundational optimization to become visible to AI agents.

### Score Breakdown

| Category | Score | Weight | Weighted Score |
|---|---|---|---|
| AI Citability | 10/100 | 25% | 2.5 |
| Brand Authority | 10/100 | 20% | 2.0 |
| Content E-E-A-T | 20/100 | 20% | 4.0 |
| Technical GEO | 70/100 | 15% | 10.5 |
| Schema & Structured Data | 0/100 | 10% | 0.0 |
| Platform Optimization | 10/100 | 10% | 1.0 |
| **Overall GEO Score** | | | **20/100** |

---

## Critical Issues (Fix Immediately)

- **Missing Schema.org Markup:** The site has no structured data (0 blocks found). Search engines and AI models cannot reliably identify the entity (Daniel Khakimov).
  - *Fix:* Add `Person` and `Organization` schemas with `sameAs` linking to Spotify, YouTube, and PGP key.
- **No llms.txt:** Essential context for AI agents is missing.
  - *Fix:* Publish `llms.txt` at the domain root with site structure map.

## High Priority Issues

- **Thin Content / Low Citability:** The site uses minimalistic navigation with very few words (116 words on the homepage). AI cannot cite what isn't there.
  - *Fix:* Consider adding a more descriptive "About" page with biographical information and music genre descriptions.
- **No Wikipedia Presence:** "Daniel Khakimov" doesn't trigger Wikipedia API results, significantly reducing entity recognition by ChatGPT and Gemini.
  - *Fix:* Build PR and create Wikidata/Wikipedia profiles if notable.

## Medium Priority Issues

- **Minimal Cross-Platform Ecosystem Integration:** No linked YouTube content on the homepage directly, minimal Reddit mentions found in automated scan.
  - *Fix:* Directly embed or clearly link main YouTube tracks, engage in relevant Subreddits.

## Low Priority Issues

- **AI Crawlers in robots.txt:** While `robots.txt` explicitly adds `content-signal` definitions (a great emerging standard), explicit `Allow` rules for major bots like `GPTBot`, `ClaudeBot`, and `PerplexityBot` are not mentioned.

---

## Category Deep Dives

### AI Citability (10/100)
Content blocks are virtually non-existent for AI extraction. The site operates as a directory/archive. AI bots need paragraph-level text to summarize who the artist is.

### Brand Authority (10/100)
The brand scanner found low correlation on Reddit, YouTube (official channel not explicitly mapped via API), and Wikipedia. Entity resolution is weak.

### Content E-E-A-T (20/100)
The site establishes trust via PGP Fingerprint and direct contact info, but lacks deep Expertise/Authoritativeness text explaining the artist's background.

### Technical GEO (70/100)
Strong area. The site uses Server-Side Rendering (SSR), is fast, and serves clear HTTP headers. It has an advanced `robots.txt` implementing `draft-romm-aipref-contentsignals`.

### Schema & Structured Data (0/100)
Completely missing.

### Platform Optimization (10/100)
Not optimized for ChatGPT/Perplexity due to lack of Wikipedia presence and low text volume.

---

## Quick Wins (Implement This Week)

1. Add `llms.txt` and `llms-full.txt` to the root directory outlining the site map and a brief bio.
2. Inject `<script type="application/ld+json">` with `Person` schema containing `sameAs` links to Spotify and YouTube.
3. Explicitly allow `GPTBot`, `ClaudeBot`, and `PerplexityBot` in `robots.txt`.

## 30-Day Action Plan

### Week 1: Foundational Signals
- [x] Create and deploy `llms.txt`.
- [x] Deploy JSON-LD Schema markup for the artist.

### Week 2: Content Depth
- [ ] Expand the "About" section with a 150-300 word biography.
- [ ] Add descriptive paragraphs to the Discography items.

### Week 3: Platform Integration
- [ ] Map the official YouTube channel and ensure descriptions link back to the site.
- [ ] Claim Wikidata entity if possible.
