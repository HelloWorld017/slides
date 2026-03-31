# slidev-theme-yukino

[![NPM version](https://img.shields.io/npm/v/slidev-theme-yukino?color=3AB9D4&label=)](https://www.npmjs.com/package/slidev-theme-yukino)

A styleboard-driven [Slidev](https://github.com/slidevjs/slidev) theme that blends:

- clean science/education deck structure
- editorial minimal grid composition
- optional high-contrast business/urban mood (`class: yukino-night`)

The theme ships with expressive typography, adaptive spacing, layered backgrounds, and custom layouts for key presentation moments.

## Quick Start

Use this in your slide frontmatter:

<pre><code>---
theme: <b>yukino</b>
---</code></pre>

For local preview inside this package:

- `npm install`
- `npm run dev`

## Install

Add the following frontmatter to your `slides.md`. Start Slidev then it will prompt you to install the theme automatically.

<pre><code>---
theme: <b>yukino</b>
---</code></pre>

Learn more about [how to use a theme](https://sli.dev/guide/theme-addon#use-theme).

## Layouts

This theme provides the following layouts:

- `cover` - split hero with a right-side preview rail
- `intro` - opening slide with strong headline hierarchy
- `section` - section divider for chapter transitions
- `statement` - oversized slogan/impact slide
- `end` - closing slide style

All built-in Slidev layouts are still available through `layouts-base.css`.

## Components

This theme provides the following components:

- None yet (utility classes are provided in CSS instead)

## Utility Classes

- `.yukino-kicker` - compact label pill for section tags
- `.yukino-panel` - elevated content panel
- `.yukino-grid` - responsive two-column content grid
- `.yukino-stat` - metric card block
- `.yukino-night` - optional dark/high-contrast mood per slide

## Contributing

- `npm install`
- `npm run dev` to start theme preview of `example.md`
- Edit the `example.md` and style to see the changes
- `npm run export` to generate the preview PDF
- `npm run screenshot` to generate the preview PNG
