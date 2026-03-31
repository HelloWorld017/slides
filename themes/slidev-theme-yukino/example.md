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
ratio: 30
---

<template #left>
  <img src="https://picsum.photos/700/1920" />
</template>

<div class="h-full">
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
</div>

---
layout: contents-left
---

<template #left>

```ts
// Code with me~

const salt = random(new Uint8Array(32));
const masterKey =
  await deriveMasterKey(password, salt);

const rootKeyRaw = random(new Uint8Array(32));
const rootKeyEncrypted =
  await encrypt(masterKey, rootKeyRaw);

const signingKey = await deriveSigningKey(rootKey);
const newManifest = await signManifest(signingKey, {
  ...manifest,
  crypto: {
    masterKey: rootKeyEncrypted.toBase64(),
    masterKeySalt: salt.toBase64(),
    nonce: crypto.randomUUID(),
    timestamp: Date.now(),
    signature: '',
  },
});
```

</template>

## Coding
coding, coding?

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.  
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

---

<Columns class="mt-12">
  <div>

  ## Haro
  Mado wo akete chiisaku tsubuyaita.  
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.  
  Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
  </div>

  <FlowGroup class="mt-12 gap-4">
    <FlowItem title="How Are You" description="Dare mo inai heya de hitori" icon="01" />
    <FlowItem title="Morning" description="Asa ga kitayo doshaburi no asa ga" icon="02" />
    <FlowItem title="Tick Tack" description="Watashi no neji wo dareka maite" icon="03" />
  </FlowGroup>
</Columns>

---

<div class="-mt-6" />

## Exclusive features

<Columns :count="3">
  <div class="flex flex-col gap-4">
    <img src="https://picsum.photos/seed/A/1080/1080" class="w-full object-cover object-center" />
    <FeatureItem title="Feature A">
      <template #icon><lucide-arrow-right /></template>
      Such wow
    </FeatureItem>
  </div>
  <div class="flex flex-col gap-4">
    <img src="https://picsum.photos/seed/B/1080/1080" class="w-full object-cover object-center" />
    <FeatureItem title="Feature B">
      <template #icon><lucide-user /></template>
      Many features
    </FeatureItem>
  </div>
  <div class="flex flex-col gap-4">
    <img src="https://picsum.photos/seed/C/1080/1080" class="w-full object-cover object-center" />
    <FeatureItem title="Feature C">
      <template #icon><lucide-apple /></template>
      Doge wow
    </FeatureItem>
  </div>
</Columns>

---
layout: intro
---

## Thank You

Use `theme: yukino` and start writing.
