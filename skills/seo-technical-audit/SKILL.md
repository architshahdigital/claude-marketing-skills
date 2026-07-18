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

## Fallback: Running in Cloud/Web Environments (e.g., Claude.ai, CoWork)

If you are running in a cloud-based or web-based environment (such as Claude.ai web or CoWork) where local file system or repository access is unavailable:
1. Ask the user to provide their site URL, sitemap link, or paste Google Search Console (GSC) screenshots, crawl logs, or PageSpeed Insights data.
2. Conduct the technical audit, indexation check, and Core Web Vitals analysis manually in-context.
3. Output the structured Scorecard and the Prioritized Fix List using the templates below.

---

## Workflow

1. **Intake & Data Gathering:**
   - Request URLs, GSC error lists, or PageSpeed metrics.
   - Define the main objective (e.g., debugging indexation drops, fixing Core Web Vitals, migrating domains).

2. **Crawl & Indexation Check:**
   - Audit `robots.txt` rules, XML sitemap validation, canonical setups, and `noindex` directives.

3. **Site Architecture & Internal Links:**
   - Evaluate crawl depth (clicks from home page), internal link anchors, and redirect setups (301 vs. chains/loops).

4. **Page Speed & Core Web Vitals Audit:**
   - Evaluate:
     - **LCP (Largest Contentful Paint):** Loading speed of main images/fonts.
     - **INP (Interaction to Next Paint):** Input latency and heavy JS execution.
     - **CLS (Cumulative Layout Shift):** Visual stability of layout.

5. **Schema & Semantic Markup:**
   - Verify structured data (LocalBusiness, Article, Product, FAQ) for eligibility in Google Rich Snippets.

---

## Templates & Output Format

Ensure the audit results are clear, structured, and prioritized:

### 1. Technical SEO Health Scorecard

| Audit Area | Status | Gaps & Issues Detected |
| :--- | :---: | :--- |
| **Crawlability & Indexation** | `[PASS / WARN / FAIL]` | *E.g., Missing robots sitemap link, canonical loop.* |
| **Site Architecture** | `[PASS / WARN / FAIL]` | *E.g., Orphan pages, deep redirect chains.* |
| **Core Web Vitals & Speed** | `[PASS / WARN / FAIL]` | *E.g., Poor LCP due to uncompressed images.* |
| **Mobile & Rendering** | `[PASS / WARN / FAIL]` | *E.g., Non-responsive tables, small tap targets.* |
| **Structured Data (Schema)** | `[PASS / WARN / FAIL]` | *E.g., Missing required fields in Product schema.* |

### 2. Prioritized Technical Fix List
Rank issues using the impact-effort matrix (High Impact + Low Effort = Priority 1):

| Priority | Issue / Fix Required | Affected Pages | Impact | Effort | Recommendation / Solution |
| :---: | :--- | :--- | :---: | :---: | :--- |
| **1** | E.g., Eliminate 3 redirect loops on homepage. | `homepage` | `HIGH` | `LOW` | Update link destinations to final URLs. |
| **2** | E.g., Add dimensions to hero images (CLS fix). | `blog template` | `MEDIUM` | `LOW` | Set explicit `width` and `height` attributes. |
| **3** | E.g., Lazy-load B-roll videos below-the-fold. | `landing-page` | `HIGH` | `MEDIUM`| Implement standard lazy loading/defer scripting. |

> [!IMPORTANT]
> **Priority Focus:** Highlight the **Top 3 High-Impact Fixes** in a clear callout box at the top of your response to give the user immediate focus.
