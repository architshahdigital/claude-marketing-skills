---
name: content-repurposing-engine
description: >
  Turn one hero asset (blog post, newsletter, video transcript, webinar) into a full set
  of platform-native content — LinkedIn, Instagram, X, and a short-form video script —
  each rewritten for its platform instead of copy-pasted. Use when the user has one long
  piece and needs a week of content from it, wants to repurpose, or is building a content
  calendar from existing material. Produces ready-to-schedule copy per platform with a
  fact-check pass. Triggers on: "repurpose", "turn this into posts", "content from this
  blog/video", "week of content", "atomize", "multi-platform content".
---

# Content Repurposing Engine

One idea, produced once, deployed everywhere — but *native* everywhere. This skill atomizes a hero asset into platform-specific content so each piece earns attention on its own channel rather than reading like a cross-post.

## Fallback: Running in Cloud/Web Environments (e.g., Claude.ai, CoWork)

If you are running in a cloud-based or web-based environment (such as Claude.ai web or CoWork) where local file system or repository access is unavailable:
1. Ask the user to paste their long-form text (blog post, newsletter, script, transcript) directly into the chat.
2. Ask the user to specify their brand voice or style guide (if any).
3. Perform the analysis, extraction, and rewriting manually in-context.
4. Output the structural theme analysis and the platform-native drafts matching the templates below.

---

## Workflow

1. **Analysis & Extraction:**
   - Ingest the long-form source document.
   - Extract the core thesis, 3–5 supporting points, any data/metrics/proof points, and 3–5 potential hooks.

2. **Aesthetic Audit & Exclusions:**
   - Establish rules for what to avoid (e.g., cliché intros, corporate jargon, generic formatting).

3. **Platform-Native Writing:**
   - Write drafts for the requested platforms:
     - **LinkedIn:** Focused on professional insights, clean spacing, and a clear call-to-action.
     - **Instagram Captions:** Frontloaded hook, storytelling/educational focus.
     - **X (Twitter) Thread:** 4-5 tweet thread outline focusing on a single, clear narrative arc.
     - **Short-form Video Script:** 25-35s vertical video script with voiceover and visual/B-roll cues.

4. **Fact-Checking Gate:**
   - Flag any specific numbers, historical details, or claims that must be validated before going live.

---

## Templates & Output Format

Ensure the output is clean and ready to copy-paste into scheduling tools:

### 1. LinkedIn Post Draft
> **Format:** Clean spacing, active voice, bold first line, no hashtags in body.
```markdown
[Hook: Bold contrarian take or compelling stat]

[Body: 3 short, bulleted insights explaining the concept]

[CTA: Friendly invitation to discuss or check the main link]
```

### 2. Instagram Caption Drafts
Generate 3 variations (Educational, Story-based, Contrarian) using this structure:
```markdown
📸 [Headline Hook - CAPITALIZED]

[Conversational body copy explaining the concept]

📍 [Clear Actionable CTA]
```

### 3. X (Twitter) Thread Outline
```markdown
🧵 1/4 [The Hook: What is this thread about and why read it?]
🧵 2/4 [The core problem or context]
🧵 3/4 [The main solution or step]
🧵 4/4 [Conclusion & CTA]
```

### 4. Reel/TikTok Video Script (25-30 seconds)

| Time | Visual / B-Roll Cue | Audio / Voiceover |
| :---: | :--- | :--- |
| **0-2s** | *[On-screen text: Bold hook. Zoom in on speaker]* | "[Hook: Speak directly to the pain point/solution]" |
| **2-10s** | *[Transition: Screen capture or physical gesture]* | "[Deliver the core insight or step 1]" |
| **10-20s**| *[Transition: High-pace edit showing action]* | "[Deliver step 2 and the payoff]" |
| **20-30s**| *[Visual: Point to link or smile at camera]* | "[Call to action: Shop the link in bio/save this post]" |

> [!WARNING]
> Keep the spoken copy conversational and brief. Avoid text-heavy slides or complex sentence structures.
