# slidev-theme-yukino

[![NPM version](https://img.shields.io/npm/v/slidev-theme-yukino?color=3AB9D4&label=)](https://www.npmjs.com/package/slidev-theme-yukino)

A bright, text-first [Slidev](https://github.com/slidevjs/slidev) theme inspired by editorial layouts and clean blue accent decks.

<!--
  Learn more about how to write a theme:
  https://sli.dev/guide/write-theme.html
--->

<!--
  run `npm run dev` to check out the slides for more details of how to start writing a theme
-->

<!--
  Put some screenshots here to demonstrate your theme

  Live demo: [...]
-->

## Install

Add the following frontmatter to your `slides.md`. Start Slidev then it will prompt you to install the theme automatically.

<pre><code>---
theme: <b>yukino</b>
---</code></pre>

Learn more about [how to use a theme](https://sli.dev/guide/theme-addon#use-theme).

## Layouts

This theme provides the following layouts:

- `cover`
- `intro`
- `section`

## Components

This theme provides the following components:

- `SectionLead`
  - Small kicker + title + subtitle block for section opening slides.
- `FlowGroup`
  - Wrapper for step-by-step flow content.
- `FlowItem`
  - Icon/title/description item for process or agenda slides.
- `StatLine`
  - Minimal key-value row with optional note.

## Utility Classes

- `yukino-columns`
  - Responsive two-column grid for content-heavy slides.

## Contributing

- `npm install`
- `npm run dev` to start theme preview of `example.md`
- Edit the `example.md` and style to see the changes
- `npm run export` to generate the preview PDF
- `npm run screenshot` to generate the preview PNG
