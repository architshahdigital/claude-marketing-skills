---
name: geo-content-optimizer
description: >
  Optimize any piece of content to be cited and surfaced by AI answer engines
  (ChatGPT, Google AI Overviews, Perplexity, Gemini) — not just ranked by classic
  search. Use when the user wants to improve AI visibility, "get cited by ChatGPT",
  audit content for GEO/AEO, add answer-first structure, strengthen E-E-A-T signals,
  or turn an existing article into something a language model will quote. Produces a
  prioritized rewrite plan plus the rewritten sections. Triggers on: "GEO", "AEO",
  "AI visibility", "get cited", "answer engine optimization", "optimize for ChatGPT/
  Perplexity/AI Overviews".
---

# GEO Content Optimizer

Classic SEO gets you ranked. **Generative Engine Optimization (GEO)** gets you *quoted* — cited inside an AI answer where the click, the trust, and the brand lift now happen. This skill audits content against the signals language models actually reward and rewrites it to be citable.

## Fallback: Running in Cloud/Web Environments (e.g., Claude.ai, CoWork)

If you are running in a cloud-based or web-based environment (such as Claude.ai web or CoWork) where local file system or repository access is unavailable:
1. Ask the user to paste the target article text or provide the URL directly in the chat.
2. Ask the user to define the target query/topic they want the content to be cited for.
3. Perform the complete audit and rewrite manually within your conversation context.
4. Output the same formatted scorecard and rewrite templates as defined below.

---

## Workflow

1. **Intake & Discovery:**
   - Locate the target page content (either by reading a local file, or asking the user to paste it).
   - Get the primary search query or question they want the page to answer.

2. **The 5-Lever Citability Audit:**
   - Evaluate the content from 0 (absent) to 2 (strong) across these 5 levers:
     - **Answer-First Structure:** Are direct, self-contained answers placed at the start of each section?
     - **Extractable Units:** Are claims written in short, simple sentences, using bullet points/tables where possible?
     - **E-E-A-T Evidence:** Are claims backed by primary data, credentials, and update dates?
     - **Specificity:** Are vague descriptions replaced with concrete numbers, names, and tools?
     - **Freshness + Scope:** Is the date visible, and are related edge cases, comparisons, and FAQs covered?
   
3. **Generate Scorecard:**
   - Present a formatted markdown table scoring each lever, followed by an overall Citability Score (out of 10).

4. **Rewrite Plan & Execution:**
   - List the exact edits needed (ranked by impact).
   - Rewrite the weak sections of the content, highlighting the "Before" vs "After" changes in side-by-side or stacked diffs.

5. **Generate FAQ Block:**
   - Create 4-6 natural language Q&As designed specifically to match typical question intents.

## Templates & Output Format

### Citability Scorecard

| Lever | Score (0-2) | Gap / Assessment |
| :--- | :---: | :--- |
| **Answer-First Structure** | `[0/1/2]` | *Assessment of whether the main answers are immediately visible.* |
| **Extractable Units** | `[0/1/2]` | *Assessment of prose density and structure.* |
| **E-E-A-T Evidence** | `[0/1/2]` | *Assessment of primary data, sources, and author credentials.* |
| **Specificity** | `[0/1/2]` | *Assessment of data precision vs. vague hedges.* |
| **Freshness + Scope** | `[0/1/2]` | *Assessment of date signals and comprehensive coverage.* |

> [!TIP]
> **Total Citability Score:** `X / 10` (8+ is highly citable)

### Rewrite Example Format
```diff
- [Before: buried answer, passive language, vague stats]
+ [After: direct answer-first, active language, specific numbers, and E-E-A-T citation]
```

## Guardrails
- **Never fabricate E-E-A-T details:** If primary sources, author credentials, or data is missing, flag it (⚠️) and prompt the user to provide real information. Do not invent it.
- **Maintain Tone:** Ensure rewritten sections respect the brand's original voice guide.
