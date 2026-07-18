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

## Fallback: Running in Cloud/Web Environments (e.g., Claude.ai, CoWork)

If you are running in a cloud-based or web-based environment (such as Claude.ai web or CoWork) where local file system or repository access is unavailable:
1. Ask the user to paste 2-3 examples of writing they like, 1-2 examples they dislike, and their target audience.
2. Conduct the voice analysis and build the rule set manually in-context.
3. Output the structured Voice Profile using the templates below.

---

## Workflow

1. **Intake & Material Review:**
   - Gather sample articles, emails, or posts.
   - Define target customer persona and context (e.g., B2B enterprise vs. consumer D2C).

2. **Establish Voice Traits (3–4 traits):**
   - Define traits as clear spectrums (e.g., Formal to Casual). Specify where on the spectrum the brand sits.

3. **Define Do / Don't Rules:**
   - Map exact language behaviors, not just adjectives. Specify what to write and what to avoid.

4. **Lexicon & Formatting Rules:**
   - Document permitted terminology, banned buzzwords, emoji policies, and punctuation quirks.

5. **Provide Before / After Examples:**
   - Provide 2–3 side-by-side examples showing a generic sentence rewritten to match the brand voice.

---

## Templates & Output Format

Ensure the brand voice profile is generated in a clean, drop-in format:

### 1. Brand Voice Profile

#### 🏷️ Voice Traits & Spectrums
*   **Trait 1: [Name, e.g. Conversational]** — *Warm, personal, direct to consumer.*
    `Formal ―――—●― Casual`
*   **Trait 2: [Name, e.g. High Information]** — *Stat-driven, direct, educational.*
    `Speculative ―――——● High-Proof`

#### 📝 Rules Matrix

| Do | Don't |
| :--- | :--- |
| **Write short, active sentences.** | **Corporate hedging (e.g., "we strive to").** |
| **Address the reader as "you" directly.** | **Third-person distance (e.g., "users should").** |
| **Use concrete examples and exact stats.** | **Buzzword stacking (e.g., "synergy", "disruptive").** |

#### 📖 Lexicon & Guidelines
*   **Approved Terms:** `[term1]`, `[term2]`, `[term3]`
*   **Banned Buzzwords:** `[word1]`, `[word2]`, `[word3]`
*   **Emoji/Formatting Policy:** *E.g., Maximum 1 emoji per paragraph, no emojis in headers.*

#### 🔄 Voice Refinement Examples

```diff
- [Generic: Our platform assists businesses in optimizing their social campaigns for enhanced user engagement.]
+ [On-Brand: We build tools that make your ads stand out so you get more clicks and sales.]
```

> [!TIP]
> **The One-Line North Star:** Create a single, memorable sentence that sums up the voice (e.g., *"Write like an experienced colleague explaining a concept over coffee."*) so writers can quickly QA their drafts.
