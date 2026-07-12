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

## When to run this

- The user has an article/landing page and wants it surfaced in AI answers.
- Traffic is flat despite good rankings (answers are eating the clicks).
- A brand wants to become the "quoted source" in its niche.

## The 5 citability levers

Work through these in order. Each maps to a concrete edit, not a vague principle.

1. **Answer-first structure** — Lead every section with a direct, standalone answer in the first 1–2 sentences, then support it. Models extract self-contained passages; buried answers don't get lifted.
2. **Extractable units** — Break claims into short, quotable statements. One idea per sentence. Definitions, steps, and comparisons in lists or tables (models parse these cleanly).
3. **E-E-A-T evidence** — Attach *experience* and *authority* to every claim: first-hand data, named author with credentials, dates, primary sources, and specific numbers instead of "studies show."
4. **Specificity over fluff** — Replace hedges ("many", "often", "can help") with concrete figures, named tools, and real examples. Models prefer high-information-density text.
5. **Freshness + scope signals** — Add a visible "last updated" date, cover the *full* question space (definitions, edge cases, comparisons, FAQs) so the page is the complete answer, not a fragment.

## Workflow

1. **Intake** — Ask for the URL or pasted content and the target question/query it should win.
2. **Audit** — Score the content 0–2 on each of the 5 levers. Output a short scorecard with the biggest gaps flagged.
3. **Rewrite plan** — List the highest-leverage edits, ordered by impact. Be specific ("Rewrite the intro to answer '<query>' in the first sentence").
4. **Execute** — Rewrite the weakest sections. Preserve the brand voice; add a source/date line; convert dense prose into extractable units.
5. **FAQ block** — Generate 4–6 natural-language Q&As that mirror how people actually ask, each answered in 1–2 self-contained sentences.

## Guardrails

- Never fabricate statistics, sources, or credentials to fake E-E-A-T. If a claim needs evidence the user doesn't have, flag it (⚠️) for them to supply — a hallucinated citation destroys trust and citability.
- Keep the human's real expertise front and center; GEO amplifies genuine authority, it can't invent it.

See `references/citability-checklist.md` for the full scoring rubric.
