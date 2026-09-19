# Pixel Computer Club — static website

This project is a two-page static website for Pixel Computer Club in Astana.
It intentionally uses only local HTML, CSS, images and font files. No server, build step, framework or JavaScript is required.

## Open the site

Open [index.html](index.html) directly in a browser. The second page is [all-locations.html](all-locations.html), linked from the header as **The devices and price**.

The CSS-only slider on the first page uses radio buttons and labels. The responsive menus use native `<details>` elements, so both features work without JavaScript.

## Project structure

```text
index.html              Main About Pixel page
all-locations.html      Devices and price page
css/base.css            Shared reset, palette and typography
css/Anuar.css           Page layout and component styles
assets/pixel/           Local photos and font files
materials/              Submission documentation and screenshots
CSS-checklist.md        Requirement-to-code checklist with line references
design-sketches.md      Desktop and mobile layout sketches
CSS-validation.md       CSS validator record
```

Both HTML pages load `css/base.css` first and `css/Anuar.css` second. The second stylesheet contains the page-specific layout while the base file contains the shared foundation.

## Accessibility and coursework demonstrations

The pages include visible keyboard focus states, semantic headings, labelled navigation, native details menus, a fixed contact shortcut, a float/clear demonstration, and comments explaining the selectors and layout choices. The pricing page also demonstrates the CSS cascade with an internal `<style>` block and an inline declaration.

## Validation

The exact validator result and the date of the check are recorded in [CSS-validation.md](CSS-validation.md). The checklist in [CSS-checklist.md](CSS-checklist.md) is intentionally tied to current file line numbers.
