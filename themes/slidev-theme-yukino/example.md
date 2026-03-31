---
theme: ./
title: Yukino Theme Preview
presentedAt: 2026. 03. 31
presentedBy: nenw*
transition: fade
---

# Yukino

A bright, minimal theme for content-dense talks.

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
  <FlowItem title="Inspect">
    <template #icon>
        <lucide-arrow-right />
    </template>
    Read runtime behavior and isolate one root cause candidate.
  </FlowItem>
  <FlowItem title="Conclude" description="Turn findings into a small, verifiable decision for the next slide." icon="03" />
</FlowGroup>

---
layout: contents-left
---

<template #left>
  <img src="https://picsum.photos/700/1920" />
</template>

<SectionLead
  eyebrow="Images"
  title="Contents Left Structure"
  subtitle="General markdown should stay clean in 16:9 without forcing everything into cards."
/>

<FlowItem title="Inspect">
  <template #icon>
      <lucide-arrow-right />
  </template>
  Read runtime behavior and isolate one root cause candidate.
</FlowItem>

<FlowItem title="Hello">
  <template #icon>
      <lucide-user />
  </template>
  How are you
</FlowItem>

<FlowItem title="Sekai no">
  <template #icon>
      <lucide-clock />
  </template>
  Ichiban ohimesama
</FlowItem>

---
layout: intro
---

## Thank You

Use `theme: yukino` and start writing.
