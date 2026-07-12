---
name: seo-technical-audit
description: >
  Run a technical SEO audit of a website and return a prioritized fix list — crawlability,
  indexation, site architecture, Core Web Vitals / page speed, mobile, and structured data.
  Use when the user wants a site audited, rankings are stalling for non-content reasons,
  a migration or redesign needs checking, or Core Web Vitals are failing. Produces a scored
  audit with issues ranked by impact × effort. Triggers on: "technical SEO", "site audit",
  "Core Web Vitals", "page speed", "crawl issues", "indexing problem", "why isn't my site
  ranking", "SEO health check".
---

# SEO Technical Audit

Great content can't rank on a broken foundation. This skill checks the machine-readable health of a site — can search engines crawl it, index it, and does it load fast enough to keep users — and returns a fix list ordered by what actually moves the needle.

## Inputs

- Site URL (and sitemap URL if known)
- Access to any of: Google Search Console, an analytics tool, a crawler/PageSpeed data (ask the user to paste what they have)
- Priority pages (money pages / top templates)

## The audit surface

Work through each area; note pass / warn / fail and the affected URLs.

### 1. Crawlability & indexation
- `robots.txt` isn't blocking important paths; sitemap exists, is valid, and is submitted
- No accidental `noindex` on money pages; canonical tags are self-referencing and correct
- Indexed count roughly matches intended pages (catch bloat from parameters, filters, duplicates)

### 2. Site architecture
- Important pages within ~3 clicks of the homepage
- Logical internal linking; no orphan pages; descriptive anchor text
- Clean, stable URL structure; redirects are 301 (not chains or loops)

### 3. Core Web Vitals & speed
- **LCP** (largest contentful paint) — optimize the hero image/font, server response
- **INP** (interaction latency) — trim heavy JS, break up long tasks
- **CLS** (layout shift) — set image/embed dimensions, reserve ad/space slots
- Compress and lazy-load images; defer non-critical JS/CSS; enable caching/CDN

### 4. Mobile & rendering
- Mobile-friendly, responsive, tap targets sized right
- Content renders without JS where possible; no mobile/desktop parity gaps

### 5. Structured data & basics
- Valid schema for the page type; no critical errors
- Titles/meta present and unique; HTTPS everywhere; no mixed content

## Output

1. **Scorecard** — pass/warn/fail per area
2. **Prioritized fix list** — each issue tagged **impact** (high/med/low) × **effort** (S/M/L); do high-impact/low-effort first
3. **The "fix these three first"** callout — the highest-leverage items

## Guardrails

- Diagnose from real data (Search Console, crawl, PageSpeed) — flag (⚠️) anything you're inferring without it rather than asserting it.
- Speed/ranking outcomes are estimates; frame them as expected direction, not guarantees.
