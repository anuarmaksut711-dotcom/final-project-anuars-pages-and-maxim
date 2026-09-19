# CSS checklist

Line numbers below refer to the current files in this project. Re-run `rg -n` or open the linked files if the files are edited later.

| Requirement | Selector / property | File and line | Purpose | Status |
|---|---|---:|---|---|
| Shared stylesheet order | `base.css` then `Anuar.css` | `index.html:10-11`, `all-locations.html:10-11` | Loads the shared foundation before page-specific rules. | Done |
| Author metadata | `<meta name="author" content="Anuar Maksut Se - 2537">` | `index.html:6`; `all-locations.html:6` | Identifies the author using the standard metadata name. | Done |
| Semantic navigation list | `<nav>` with `<ul>` and `<li>` | `index.html:29-87`; `all-locations.html:28-85` | Exposes the primary and mobile navigation as lists for assistive technology. | Done |
| Heading hierarchy | `h1`, `h2`, `h3` | `index.html:97, 106`; `all-locations.html:96, 105, 159`; dropdown/footer labels use styled paragraphs. | Avoids skipped `h4`/`h5` levels while preserving visual design. | Done |
| Copyright entity | `&copy; 2026 Pixel Computer Club` | `index.html:204`; `all-locations.html:203` | Provides the required copyright notice in the footer. | Done |
| Palette | `--pixel-*` variables | `css/base.css:3-13` | Limits the design system to five named colors. | Done |
| Two font families and fallbacks | `@font-face`, `font-family` | `css/base.css:15-46, 63-64`; `css/Anuar.css:323-325` | Documents local fonts and readable fallback stacks. | Done |
| Adjacent selector | `h2 + p` | `css/base.css:89-92` | Removes an unexpected gap directly after a heading. | Done |
| Explicit focus state | `a:focus`, `button:focus`, `summary:focus` | `css/base.css:81-87` | Preserves visible keyboard focus. | Done |
| Hover and focus comments | `:hover`, `:focus-visible` | `css/base.css:75-79`; `css/Anuar.css:109-118` | Explains pointer and keyboard interaction states. | Done |
| Direct-child selector | `>` | `css/Anuar.css:84-103` | Styles only the immediate navigation summary child. | Done |
| Attribute selector | `[open]` | `css/Anuar.css:138-142` | Shows native details menus while open. | Done |
| Pseudo-elements | `::before`, `::after` | `css/Anuar.css:285-289, 777-786, 838-858` | Creates decorative fades, markers and button edges without markup. | Done |
| Structural selector | `:nth-child` | `css/Anuar.css:491-498` | Gives the Duo and VIP cards their distinct palette treatment. | Done |
| Flexbox alignment | `display:flex`, `align-items`, `justify-content`, `gap` | `css/Anuar.css:66-75` | Aligns and spaces the desktop navigation. | Done |
| Flexible wrapping | `flex-wrap` | `css/Anuar.css:72, 257` | Allows navigation content to adapt to narrower widths. | Done |
| Static positioning | `position: static` | `css/Anuar.css:1-7` | Explicitly documents normal flow for the page wrapper. | Done |
| Fixed positioning | `position: fixed` | `css/Anuar.css:9-22` | Keeps the Contact shortcut visible while scrolling. | Done |
| Float and clear | `float: left`, `clear: both` | `css/Anuar.css:687-706`; `index.html:161-165` | Wraps text around a demo image and clears the float afterward. | Done |
| Margin-auto centering | `margin: 0 auto` | `css/Anuar.css:312, 352, 681, 757` | Centers the content, slider and gallery while keeping side padding. | Done |
| Transform centering | `transform: translateY(-50%)` | `css/Anuar.css:618-628` | Centers slider controls relative to the slider height. | Done |
| ID rationale | `#main-content`, `#organizations`, `#contact`, slide IDs | `index.html:88, 170, 194`; `all-locations.html:87, 193`; `index.html:107-112`; `css/Anuar.css:563-569` | Gives anchor destinations and CSS-only radio states stable IDs. | Done |
| Internal CSS | `<style>` | `index.html:13-18`; `all-locations.html:13-18` | Demonstrates a page-level rule after external CSS. | Done |
| Inline CSS | `style="..."` | `index.html:103`; `all-locations.html:146` | Demonstrates the highest-priority declaration in the cascade. | Done |
| CSS-only interaction | radio selectors and `<details>` | `index.html:107-159`; `css/Anuar.css:563-642` | Provides the slider and menus without JavaScript. | Done |
