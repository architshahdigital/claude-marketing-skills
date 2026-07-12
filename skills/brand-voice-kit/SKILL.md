---
name: brand-voice-kit
description: >
  Define a brand's voice and turn it into a reusable rule set that keeps every piece of
  AI-generated content on-brand. Use when the user is setting up a brand voice, wants
  consistency across writers/channels, needs a voice guide, or wants to "make this sound
  like us." Produces a voice profile (traits, do/don't, lexicon, examples) that can be
  pasted into any content prompt as guardrails. Triggers on: "brand voice", "tone of voice",
  "make it sound like us", "voice guide", "brand consistency", "style guide", "on-brand".
---

# Brand Voice Kit

A brand voice only works if it's *operational* — specific enough that a person or a model can apply it without guessing. This skill turns fuzzy adjectives ("professional but friendly") into a concrete rule set you can drop into any content workflow as guardrails.

## Two modes

- **Define** — build a voice profile from scratch (new brand, or never documented)
- **Enforce** — take an existing voice profile and rewrite/QA a draft against it

## Building the voice profile (Define)

Gather inputs first: what the brand does, who it talks to, 2–3 sample pieces they *like*, and any they *don't*.

Then produce:

1. **Voice traits (3–4)** — each as a spectrum with a chosen position, e.g. *Formal ―—●— Casual*, *Playful —●—— Serious*. Vague single words aren't enough.
2. **Do / Don't table** — concrete behaviors, not adjectives:

| Do | Don't |
|----|-------|
| Short, active sentences | Corporate hedging ("we strive to…") |
| Speak to "you" directly | Third-person distance |
| Concrete examples & numbers | Buzzword stacking |

3. **Lexicon** — words/phrases the brand *uses* and ones it *bans*; preferred spellings, emoji policy, punctuation quirks.
4. **Before/after examples** — 2–3 rewrites showing a generic line turned on-brand. Examples teach faster than rules.
5. **The one-line north star** — a single sentence that captures the voice (a writer should be able to sanity-check any draft against it).

## Enforcing (rewrite / QA mode)

Given a draft + a voice profile:
- Flag every line that violates a Do/Don't or uses a banned word
- Rewrite flagged lines to match, preserving meaning
- Return a short "voice score" and what changed

## How to use the output

Paste the voice profile into the top of any content prompt (or the `content-repurposing-engine` / `carousel-studio` skills) as the brand-voice context — every downstream piece then inherits the same guardrails.

## Guardrails

- Anchor the profile in the brand's *real* samples, not generic best practice — voice is a fingerprint, not a template.
- Don't over-constrain: leave room for the message; the voice serves communication, not the reverse.
