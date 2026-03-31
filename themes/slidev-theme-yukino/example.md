---
theme: ./
title: Yukino Theme Preview
---

# Yukino

A bright, minimal theme for content-dense talks.

---
layout: section
---

<SectionLead
  eyebrow="Theme Direction"
  title="Text first. Visual second."
  subtitle="General markdown should stay clean in 16:9 without forcing everything into cards."
/>

- Light background with soft blue accent fields
- Tight heading rhythm and readable body text
- Minimal components for practical slide composition

---

## Markdown Readability

This theme is tuned for regular markdown writing flows. It keeps hierarchy obvious while staying visually quiet.

> Keep each slide focused on one claim, then support it with compact evidence.

### What it handles well

- Lists and sub-points with stable spacing
- Tables and code blocks without visual noise
- Mixed Korean and English text in one deck
- Component usage only where structure adds value

---

## Flow Component Example

<FlowGroup>
  <FlowItem title="Observe" description="Collect a reproducible symptom before touching implementation details." icon="01" />
  <FlowItem title="Inspect" icon="02">
    Read runtime behavior and isolate one root cause candidate.
  </FlowItem>
  <FlowItem title="Conclude" description="Turn findings into a small, verifiable decision for the next slide." icon="03" />
</FlowGroup>

---

## Data + Narrative

<div class="yukino-columns">
  <div>
    <StatLine label="Deck runtime" value="35 min" note="Estimated live session time" />
    <StatLine label="Core sections" value="4" />
    <StatLine label="Code samples" value="11" note="Most are executable snippets" />
  </div>

  <div>

| Stage | Focus |
| --- | --- |
| Discovery | Confirm what is actually happening |
| Analysis | Compare likely causes |
| Decision | Pick the smallest safe change |

  </div>
</div>

---
layout: intro
---

## Thank You

Use `theme: yukino` and start writing.
