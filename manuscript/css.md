# CSS {#toc-css}

This section covers CSS as per the [CSS Snapshot 2023](https://www.w3.org/TR/css-2023/) as well as CSS working drafts as of <!-- @@ -->June 2024.

I> Identifying and maintaining overviews of CSS selectors, at-rules, and especially properties, including their status and support, is a notoriously difficult task. For CSS properties, the best resource may be the [_List of CSS Properties, Both Proposed and Standard_](https://www.w3.org/Style/CSS/all-properties.en.html), maintained by Bert Bos (W3C). Usually, as in this case, collecting this information requires consulting various specifications, and still comes with a probability of error.

## Selectors

Memorize all selectors, to improve your ability to target elements for styling.

| Selector | Form |
| --- | --- |
| Universal selector | `*` |
| Type (element name) selector | `E` |
| Descendant combinator (` `) | `E F` |
| Child combinator (`>`) | `E > F` |
| Next-sibling combinator (`+`) | `E + F` |
| Subsequent-sibling combinator (`~`) | `E ~ F` |
| Column combinator (`\|\|`) | `F \|\| E` |
| Class selector | `E.warning` |
| ID selector | `E#myid` |
| Attribute presence  and value selector | `E[foo]` |
| Attribute presence  and value selector | `E[foo='bar']` |
| Attribute presence  and value selector | `E[foo~='bar']` |
| Substring matching attribute selector | `E[foo^='bar']` |
| Substring matching attribute selector | `E[foo$='bar']` |
| Substring matching attribute selector | `E[foo*='bar']` |
| Attribute presence  and value selector | `E[foo\|='en']` |
| Case-sensitivity | `E[foo='bar' i]` |
| Case-sensitivity | `E[foo='bar' s]` |
| `:root` pseudo-class | `E:root` |
| `:empty` pseudo-class | `E:empty` |
| `:nth-child()` pseudo-class | `E:nth-child(n [of S]?)` |
| `:nth-last-child()` pseudo-class | `E:nth-last-child(n [of S]?)` |
| `:first-child` pseudo-class | `E:first-child` |
| `:last-child` pseudo-class | `E:last-child` |
| `:only-child` pseudo-class | `E:only-child` |
| `:nth-of-type()` pseudo-class | `E:nth-of-type(n)` |
| `:nth-last-of-type()` pseudo-class | `E:nth-last-of-type(n)` |
| `:first-of-type` pseudo-class | `E:first-of-type` |
| `:last-of-type` pseudo-class | `E:last-of-type` |
| `:only-of-type` pseudo-class | `E:only-of-type` |
| `:nth-col()` pseudo-class | `E:nth-col(n)` |
| `:nth-last-col()` pseudo-class | `E:nth-last-col(n)` |
| Negation (matches-none) pseudo-class `:not()` | `E:not(s1, s2, …)` |
| Matches-any pseudo-class `:is()` | `E:is(s1, s2, …)` |
| Specificity-adjustment pseudo-class `:where()` | `E:where(s1, s2, …)` |
| Relational pseudo-class `:has()` | `E:has(rs1, rs2, …)` |
| Directionality pseudo-class `:dir()` | `E:dir(ltr)` |
| Language pseudo-class `:lang()` | `E:lang(zh, '*-hant')` |
| Hyperlink pseudo-class `:any-link` | `E:any-link` |
| Link history pseudo-class `:link` | `E:link` |
| Link history pseudo-class `:visited` | `E:visited` |
| Local link pseudo-class `:local-link` | `E:local-link` |
| Target pseudo-class `:target` | `E:target` |
| Target container pseudo-class `:target-within` | `E:target-within` |
| Reference element pseudo-class `:scope` | `E:scope` |
| Current-element pseudo-class `:current` | `E:current` |
| Current-element pseudo-class `:current` | `E:current(s)` |
| Past-element pseudo-class `:past` | `E:past` |
| Future-element pseudo-class `:future` | `E:future` |
| Activation pseudo-class `:active` | `E:active` |
| Pointer hover pseudo-class `:hover` | `E:hover` |
| Input focus pseudo-class `:focus` | `E:focus` |
| Focus container pseudo-class `:focus-within` | `E:focus-within` |
| Focus-indicated pseudo-class `:focus-visible` | `E:focus-visible` |
| `:enabled` pseudo-class | `E:enabled` |
| `:disabled` pseudo-class | `E:disabled` |
| Mutability pseudo-class `:read-write` | `E:read-write` |
| Mutability pseudo-class `:read-only` | `E:read-only` |
| Placeholder-shown pseudo-class `:placeholder-shown` | `E:placeholder-shown` |
| Default-option pseudo-class `:default` | `E:default` |
| Selected-option pseudo-class `:checked` | `E:checked` |
| Indeterminate-value pseudo-class `:indeterminate` | `E:indeterminate` |
| Validity pseudo-class `:valid` | `E:valid` |
| Validity pseudo-class `:invalid` | `E:invalid` |
| Range pseudo-class `:in-range` | `E:in-range` |
| Range pseudo-class `:out-of-range` | `E:out-of-range` |
| Optionality pseudo-classes `:required` | `E:required` |
| Optionality pseudo-classes `:optional` | `E:optional` |
| Empty-value pseudo-class `:blank` | `E:blank` |
| User-interaction pseudo-class `:user-valid` | `E:user-valid` |
| User-interaction pseudo-class `:user-invalid` | `E:user-invalid` |
| `::before` pseudo-element | `E::before` |
| `::after` pseudo-element | `E::after` |
| `::first-letter` pseudo-element | `E::first-letter` |
| `::first-line` pseudo-element | `E::first-line` |
| `::selection` pseudo-element | `E::selection` |
| `::backdrop` pseudo-element | `E::backdrop` |
| `::marker` pseudo-element | `E::marker` |
| `::placeholder` pseudo-element | `E::placeholder` |
| `::file-selector-button` pseudo-element | `E::file-selector-button` |
| `::grammar-error` pseudo-element | `E::grammar-error` |
| `::spelling-error` pseudo-element | `E::spelling-error` |
| `::target-text` pseudo-element | `E::target-text` |
| `::cue` pseudo-element | `E::cue` |
| `::slotted()` pseudo-element | `E::slotted()` |
| `::part()` pseudo-element | `E::part()` |

## Properties

Memorize the CSS properties and their specification context, to gain a better sense of what CSS may allow you to do.

| Property | Specification (Most Mature, Most Recent) |
| --- | --- |
| `accent-color` | CSS Basic User Interface Module Level 4 |
| `align-content` | CSS Flexible Box Layout Module Level 1 |
| `align-items` | CSS Flexible Box Layout Module Level 1 |
| `align-self` | CSS Flexible Box Layout Module Level 1 |
| `alignment-baseline` | CSS Inline Layout Module Level 3 |
| `all` | CSS Cascading and Inheritance Level 3 |
| `anchor-name` | CSS Anchor Positioning |
| `anchor-scope` | CSS Anchor Positioning |
| `animation` | CSS Animations Level 1 |
| `animation-composition` | CSS Animations Level 2 |
| `animation-delay` | CSS Animations Level 1 |
| `animation-direction` | CSS Animations Level 1 |
| `animation-duration` | CSS Animations Level 1 |
| `animation-fill-mode` | CSS Animations Level 1 |
| `animation-iteration-count` | CSS Animations Level 1 |
| `animation-name` | CSS Animations Level 1 |
| `animation-play-state` | CSS Animations Level 1 |
| `animation-range` | Scroll-driven Animations |
| `animation-range-end` | Scroll-driven Animations |
| `animation-range-start` | Scroll-driven Animations |
| `animation-timeline` | CSS Animations Level 2 |
| `animation-timing-function` | CSS Animations Level 1 |
| `appearance` | CSS Basic User Interface Module Level 4 |
| `aspect-ratio` | CSS Box Sizing Module Level 4 |
| `azimuth` | CSS 2.1 |
| `backface-visibility` | CSS Transforms Module Level 2 |
| `background` | CSS 2.1 |
| `background-attachment` | CSS 2.1 |
| `background-blend-mode` | Compositing and Blending Level 1 |
| `background-clip` | CSS Backgrounds and Borders Module Level 3 |
| `background-color` | CSS 2.1 |
| `background-image` | CSS 2.1 |
| `background-origin` | CSS Backgrounds and Borders Module Level 3 |
| `background-position` | CSS 2.1 |
| `background-repeat` | CSS 2.1 |
| `background-size` | CSS Backgrounds and Borders Module Level 3 |
| `baseline-shift` | CSS Inline Layout Module Level 3 |
| `baseline-source` | CSS Inline Layout Module Level 3 |
| `block-ellipsis` | CSS Overflow Module Level 4 |
| `block-size` | CSS Logical Properties and Values Level 1 |
| `block-step` | CSS Rhythmic Sizing |
| `block-step-align` | CSS Rhythmic Sizing |
| `block-step-insert` | CSS Rhythmic Sizing |
| `block-step-round` | CSS Rhythmic Sizing |
| `block-step-size` | CSS Rhythmic Sizing |
| `bookmark-label` | CSS Generated Content Module Level 3 |
| `bookmark-level` | CSS Generated Content Module Level 3 |
| `bookmark-state` | CSS Generated Content Module Level 3 |
| `border` | CSS 2.1 |
| `border-block` | CSS Logical Properties and Values Level 1 |
| `border-block-color` | CSS Logical Properties and Values Level 1 |
| `border-block-end` | CSS Logical Properties and Values Level 1 |
| `border-block-end-color` | CSS Logical Properties and Values Level 1 |
| `border-block-end-style` | CSS Logical Properties and Values Level 1 |
| `border-block-end-width` | CSS Logical Properties and Values Level 1 |
| `border-block-start` | CSS Logical Properties and Values Level 1 |
| `border-block-start-color` | CSS Logical Properties and Values Level 1 |
| `border-block-start-style` | CSS Logical Properties and Values Level 1 |
| `border-block-start-width` | CSS Logical Properties and Values Level 1 |
| `border-block-style` | CSS Logical Properties and Values Level 1 |
| `border-block-width` | CSS Logical Properties and Values Level 1 |
| `border-bottom` | CSS 2.1 |
| `border-bottom-color` | CSS 2.1 |
| `border-bottom-left-radius` | CSS Backgrounds and Borders Module Level 3 |
| `border-bottom-right-radius` | CSS Backgrounds and Borders Module Level 3 |
| `border-bottom-style` | CSS 2.1 |
| `border-bottom-width` | CSS 2.1 |
| `border-boundary` | CSS Round Display Level 1 |
| `border-collapse` | CSS 2.1 |
| `border-color` | CSS 2.1 |
| `border-end-end-radius` | CSS Logical Properties and Values Level 1 |
| `border-end-start-radius` | CSS Logical Properties and Values Level 1 |
| `border-image` | CSS Backgrounds and Borders Module Level 3 |
| `border-image-outset` | CSS Backgrounds and Borders Module Level 3 |
| `border-image-repeat` | CSS Backgrounds and Borders Module Level 3 |
| `border-image-slice` | CSS Backgrounds and Borders Module Level 3 |
| `border-image-source` | CSS Backgrounds and Borders Module Level 3 |
| `border-image-width` | CSS Backgrounds and Borders Module Level 3 |
| `border-inline` | CSS Logical Properties and Values Level 1 |
| `border-inline-color` | CSS Logical Properties and Values Level 1 |
| `border-inline-end` | CSS Logical Properties and Values Level 1 |
| `border-inline-end-color` | CSS Logical Properties and Values Level 1 |
| `border-inline-end-style` | CSS Logical Properties and Values Level 1 |
| `border-inline-end-width` | CSS Logical Properties and Values Level 1 |
| `border-inline-start` | CSS Logical Properties and Values Level 1 |
| `border-inline-start-color` | CSS Logical Properties and Values Level 1 |
| `border-inline-start-style` | CSS Logical Properties and Values Level 1 |
| `border-inline-start-width` | CSS Logical Properties and Values Level 1 |
| `border-inline-style` | CSS Logical Properties and Values Level 1 |
| `border-inline-width` | CSS Logical Properties and Values Level 1 |
| `border-left` | CSS 2.1 |
| `border-left-color` | CSS 2.1 |
| `border-left-style` | CSS 2.1 |
| `border-left-width` | CSS 2.1 |
| `border-radius` | CSS Backgrounds and Borders Module Level 3 |
| `border-right` | CSS 2.1 |
| `border-right-color` | CSS 2.1 |
| `border-right-style` | CSS 2.1 |
| `border-right-width` | CSS 2.1 |
| `border-spacing` | CSS 2.1 |
| `border-start-end-radius` | CSS Logical Properties and Values Level 1 |
| `border-start-start-radius` | CSS Logical Properties and Values Level 1 |
| `border-style` | CSS 2.1 |
| `border-top` | CSS 2.1 |
| `border-top-color` | CSS 2.1 |
| `border-top-left-radius` | CSS Backgrounds and Borders Module Level 3 |
| `border-top-right-radius` | CSS Backgrounds and Borders Module Level 3 |
| `border-top-style` | CSS 2.1 |
| `border-top-width` | CSS 2.1 |
| `border-width` | CSS 2.1 |
| `bottom` | CSS 2.1 |
| `box-decoration-break` | CSS Fragmentation Module Level 3 |
| `box-shadow` | CSS Backgrounds and Borders Module Level 3 |
| `box-sizing` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `box-snap` | CSS Line Grid Module Level 1 |
| `break-after` | CSS Fragmentation Module Level 3 |
| `break-before` | CSS Fragmentation Module Level 3 |
| `break-inside` | CSS Fragmentation Module Level 3 |
| `caption-side` | CSS 2.1 |
| `caret` | CSS Basic User Interface Module Level 4 |
| `caret-color` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `caret-shape` | CSS Basic User Interface Module Level 4 |
| `clear` | CSS 2.1 |
| `clip` | CSS 2.1 |
| `clip-path` | CSS Masking Module Level 1 |
| `clip-rule` | CSS Masking Module Level 1 |
| `color` | CSS Color Module Level 3 |
| `color-adjust` | CSS Color Adjustment Module Level 1 |
| `color-interpolation-filters` | Filter Effects Module Level 1 |
| `color-scheme` | CSS Color Adjustment Module Level 1 |
| `column-count` | CSS Multi-column Layout Module Level 1 |
| `column-fill` | CSS Multi-column Layout Module Level 1 |
| `column-gap` | CSS Box Alignment Module Level 3 |
| `column-rule` | CSS Multi-column Layout Module Level 1 |
| `column-rule-color` | CSS Multi-column Layout Module Level 1 |
| `column-rule-style` | CSS Multi-column Layout Module Level 1 |
| `column-rule-width` | CSS Multi-column Layout Module Level 1 |
| `column-span` | CSS Multi-column Layout Module Level 1 |
| `column-width` | CSS Multi-column Layout Module Level 1 |
| `columns` | CSS Multi-column Layout Module Level 1 |
| `contain` | CSS Containment Module Level 1 |
| `contain-intrinsic-block-size` | CSS Box Sizing Module Level 4 |
| `contain-intrinsic-height` | CSS Box Sizing Module Level 4 |
| `contain-intrinsic-inline-size` | CSS Box Sizing Module Level 4 |
| `contain-intrinsic-size` | CSS Box Sizing Module Level 4 |
| `contain-intrinsic-width` | CSS Box Sizing Module Level 4 |
| `container` | CSS Containment Module Level 3 |
| `container-name` | CSS Containment Module Level 3 |
| `container-type` | CSS Containment Module Level 3 |
| `content` | CSS 2.1 |
| `content-visibility` | CSS Containment Module Level 2 |
| `continue` | CSS Overflow Module Level 4 |
| `counter-increment` | CSS 2.1 |
| `counter-reset` | CSS 2.1 |
| `counter-set` | CSS Lists and Counters Module Level 3 |
| `cue` | CSS 2.1 |
| `cue-after` | CSS 2.1 |
| `cue-before` | CSS 2.1 |
| `cursor` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `direction` | CSS Writing Modes Level 3 |
| `display` | CSS 2.1 |
| `dominant-baseline` | CSS Inline Layout Module Level 3 |
| `elevation` | CSS 2.1 |
| `empty-cells` | CSS 2.1 |
| `fill` | CSS Fill and Stroke Module Level 3 |
| `fill-break` | CSS Fill and Stroke Module Level 3 |
| `fill-color` | CSS Fill and Stroke Module Level 3 |
| `fill-image` | CSS Fill and Stroke Module Level 3 |
| `fill-opacity` | CSS Fill and Stroke Module Level 3 |
| `fill-origin` | CSS Fill and Stroke Module Level 3 |
| `fill-position` | CSS Fill and Stroke Module Level 3 |
| `fill-repeat` | CSS Fill and Stroke Module Level 3 |
| `fill-rule` | CSS Fill and Stroke Module Level 3 |
| `fill-size` | CSS Fill and Stroke Module Level 3 |
| `filter` | Filter Effects Module Level 1 |
| `flex` | CSS Flexible Box Layout Module Level 1 |
| `flex-basis` | CSS Flexible Box Layout Module Level 1 |
| `flex-direction` | CSS Flexible Box Layout Module Level 1 |
| `flex-flow` | CSS Flexible Box Layout Module Level 1 |
| `flex-grow` | CSS Flexible Box Layout Module Level 1 |
| `flex-shrink` | CSS Flexible Box Layout Module Level 1 |
| `flex-wrap` | CSS Flexible Box Layout Module Level 1 |
| `float` | CSS 2.1 |
| `float-defer` | CSS Page Floats |
| `float-offset` | CSS Page Floats |
| `float-reference` | CSS Page Floats |
| `flood-color` | Filter Effects Module Level 1 |
| `flood-opacity` | Filter Effects Module Level 1 |
| `flow-from` | CSS Regions Module Level 1 |
| `flow-into` | CSS Regions Module Level 1 |
| `font` | CSS Fonts Module Level 3 |
| `font-family` | CSS Fonts Module Level 3 |
| `font-feature-settings` | CSS Fonts Module Level 3 |
| `font-kerning` | CSS Fonts Module Level 3 |
| `font-language-override` | CSS Fonts Module Level 4 |
| `font-optical-sizing` | CSS Fonts Module Level 4 |
| `font-palette` | CSS Fonts Module Level 4 |
| `font-size` | CSS Fonts Module Level 3 |
| `font-size-adjust` | CSS Fonts Module Level 3 |
| `font-stretch` | CSS Fonts Module Level 3 |
| `font-style` | CSS Fonts Module Level 3 |
| `font-synthesis` | CSS Fonts Module Level 3 |
| `font-synthesis-position` | CSS Fonts Module Level 4 |
| `font-synthesis-small-caps` | CSS Fonts Module Level 4 |
| `font-synthesis-style` | CSS Fonts Module Level 4 |
| `font-synthesis-weight` | CSS Fonts Module Level 4 |
| `font-variant` | CSS Fonts Module Level 3 |
| `font-variant-alternates` | CSS Fonts Module Level 4 |
| `font-variant-caps` | CSS Fonts Module Level 3 |
| `font-variant-east-asian` | CSS Fonts Module Level 3 |
| `font-variant-emoji` | CSS Fonts Module Level 4 |
| `font-variant-ligatures` | CSS Fonts Module Level 3 |
| `font-variant-numeric` | CSS Fonts Module Level 3 |
| `font-variant-position` | CSS Fonts Module Level 3 |
| `font-variation-settings` | CSS Fonts Module Level 4 |
| `font-weight` | CSS Fonts Module Level 3 |
| `font-width` | CSS Fonts Module Level 4 |
| `footnote-display` | CSS Generated Content for Paged Media Module |
| `footnote-policy` | CSS Generated Content for Paged Media Module |
| `forced-color-adjust` | CSS Color Adjustment Module Level 1 |
| `gap` | CSS Box Alignment Module Level 3 |
| `glyph-orientation-vertical` | CSS Writing Modes Level 3 |
| `grid` | CSS Grid Layout Module Level 2 |
| `grid-area` | CSS Grid Layout Module Level 2 |
| `grid-auto-columns` | CSS Grid Layout Module Level 2 |
| `grid-auto-flow` | CSS Grid Layout Module Level 2 |
| `grid-auto-rows` | CSS Grid Layout Module Level 2 |
| `grid-column` | CSS Grid Layout Module Level 2 |
| `grid-column-end` | CSS Grid Layout Module Level 2 |
| `grid-column-start` | CSS Grid Layout Module Level 2 |
| `grid-row` | CSS Grid Layout Module Level 2 |
| `grid-row-end` | CSS Grid Layout Module Level 2 |
| `grid-row-start` | CSS Grid Layout Module Level 2 |
| `grid-template` | CSS Grid Layout Module Level 2 |
| `grid-template-areas` | CSS Grid Layout Module Level 2 |
| `grid-template-columns` | CSS Grid Layout Module Level 2 |
| `grid-template-rows` | CSS Grid Layout Module Level 2 |
| `hanging-punctuation` | CSS Text Module Level 3 |
| `height` | CSS 2.1 |
| `hyphenate-character` | CSS Text Module Level 4 |
| `hyphenate-limit-chars` | CSS Text Module Level 4 |
| `hyphenate-limit-last` | CSS Text Module Level 4 |
| `hyphenate-limit-lines` | CSS Text Module Level 4 |
| `hyphenate-limit-zone` | CSS Text Module Level 4 |
| `hyphens` | CSS Text Module Level 3 |
| `image-orientation` | CSS Images Module Level 3 |
| `image-rendering` | CSS Images Module Level 3 |
| `image-resolution` | CSS Images Module Level 4 |
| `initial-letter` | CSS Inline Layout Module Level 3 |
| `initial-letter-align` | CSS Inline Layout Module Level 3 |
| `initial-letter-wrap` | CSS Inline Layout Module Level 3 |
| `inline-size` | CSS Logical Properties and Values Level 1 |
| `inline-sizing` | CSS Inline Layout Module Level 3 |
| `inset` | CSS Logical Properties and Values Level 1 |
| `inset-area` | CSS Anchor Positioning |
| `inset-block` | CSS Logical Properties and Values Level 1 |
| `inset-block-end` | CSS Logical Properties and Values Level 1 |
| `inset-block-start` | CSS Logical Properties and Values Level 1 |
| `inset-inline` | CSS Logical Properties and Values Level 1 |
| `inset-inline-end` | CSS Logical Properties and Values Level 1 |
| `inset-inline-start` | CSS Logical Properties and Values Level 1 |
| `isolation` | Compositing and Blending Level 1 |
| `justify-content` | CSS Flexible Box Layout Module Level 1 |
| `justify-items` | CSS Box Alignment Module Level 3 |
| `justify-self` | CSS Box Alignment Module Level 3 |
| `left` | CSS 2.1 |
| `letter-spacing` | CSS 2.1 |
| `lighting-color` | Filter Effects Module Level 1 |
| `line-break` | CSS Text Module Level 3 |
| `line-clamp` | CSS Overflow Module Level 4 |
| `line-grid` | CSS Line Grid Module Level 1 |
| `line-height` | CSS 2.1 |
| `line-height-step` | CSS Rhythmic Sizing |
| `line-padding` | CSS Text Module Level 4 |
| `line-snap` | CSS Line Grid Module Level 1 |
| `list-style` | CSS 2.1 |
| `list-style-image` | CSS 2.1 |
| `list-style-position` | CSS 2.1 |
| `list-style-type` | CSS 2.1 |
| `margin` | CSS Box Model Module Level 3 |
| `margin-block` | CSS Logical Properties and Values Level 1 |
| `margin-block-end` | CSS Logical Properties and Values Level 1 |
| `margin-block-start` | CSS Logical Properties and Values Level 1 |
| `margin-bottom` | CSS Box Model Module Level 3 |
| `margin-break` | CSS Fragmentation Module Level 4 |
| `margin-inline` | CSS Logical Properties and Values Level 1 |
| `margin-inline-end` | CSS Logical Properties and Values Level 1 |
| `margin-inline-start` | CSS Logical Properties and Values Level 1 |
| `margin-left` | CSS Box Model Module Level 3 |
| `margin-right` | CSS Box Model Module Level 3 |
| `margin-top` | CSS Box Model Module Level 3 |
| `margin-trim` | CSS Box Model Module Level 4 |
| `marker` | SVG Markers |
| `marker-end` | SVG Markers |
| `marker-knockout-left` | SVG Markers |
| `marker-knockout-right` | SVG Markers |
| `marker-mid` | SVG Markers |
| `marker-pattern` | SVG Markers |
| `marker-segment` | SVG Markers |
| `marker-side` | CSS Lists and Counters Module Level 3 |
| `marker-start` | SVG Markers |
| `mask` | CSS Masking Module Level 1 |
| `mask-border` | CSS Masking Module Level 1 |
| `mask-border-mode` | CSS Masking Module Level 1 |
| `mask-border-outset` | CSS Masking Module Level 1 |
| `mask-border-repeat` | CSS Masking Module Level 1 |
| `mask-border-slice` | CSS Masking Module Level 1 |
| `mask-border-source` | CSS Masking Module Level 1 |
| `mask-border-width` | CSS Masking Module Level 1 |
| `mask-clip` | CSS Masking Module Level 1 |
| `mask-composite` | CSS Masking Module Level 1 |
| `mask-image` | CSS Masking Module Level 1 |
| `mask-mode` | CSS Masking Module Level 1 |
| `mask-origin` | CSS Masking Module Level 1 |
| `mask-position` | CSS Masking Module Level 1 |
| `mask-repeat` | CSS Masking Module Level 1 |
| `mask-size` | CSS Masking Module Level 1 |
| `mask-type` | CSS Masking Module Level 1 |
| `max-block-size` | CSS Logical Properties and Values Level 1 |
| `max-height` | CSS 2.1 |
| `max-inline-size` | CSS Logical Properties and Values Level 1 |
| `max-lines` | CSS Overflow Module Level 4 |
| `max-width` | CSS 2.1 |
| `min-block-size` | CSS Logical Properties and Values Level 1 |
| `min-height` | CSS 2.1 |
| `min-inline-size` | CSS Logical Properties and Values Level 1 |
| `min-intrinsic-sizing` | CSS Box Sizing Module Level 4 |
| `min-width` | CSS 2.1 |
| `mix-blend-mode` | Compositing and Blending Level 1 |
| `nav-down` | CSS Basic User Interface Module Level 4 |
| `nav-left` | CSS Basic User Interface Module Level 4 |
| `nav-right` | CSS Basic User Interface Module Level 4 |
| `nav-up` | CSS Basic User Interface Module Level 4 |
| `object-fit` | CSS Images Module Level 3 |
| `object-position` | CSS Images Module Level 3 |
| `offset` | Motion Path Module Level 1 |
| `offset-anchor` | Motion Path Module Level 1 |
| `offset-distance` | Motion Path Module Level 1 |
| `offset-path` | Motion Path Module Level 1 |
| `offset-position` | Motion Path Module Level 1 |
| `offset-rotate` | Motion Path Module Level 1 |
| `opacity` | CSS Color Module Level 3 |
| `order` | CSS Flexible Box Layout Module Level 1 |
| `orphans` | CSS 2.1 |
| `outline` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `outline-color` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `outline-offset` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `outline-style` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `outline-width` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `overflow` | CSS 2.1 |
| `overflow-anchor` | CSS Scroll Anchoring Module Level 1 |
| `overflow-block` | CSS Overflow Module Level 3 |
| `overflow-clip-margin` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-block` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-block-end` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-block-start` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-bottom` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-inline` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-inline-end` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-inline-start` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-left` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-right` | CSS Overflow Module Level 4 |
| `overflow-clip-margin-top` | CSS Overflow Module Level 4 |
| `overflow-inline` | CSS Overflow Module Level 3 |
| `overflow-wrap` | CSS Text Module Level 3 |
| `overflow-x` | CSS Overflow Module Level 3 |
| `overflow-y` | CSS Overflow Module Level 3 |
| `overscroll-behavior` | CSS Overscroll Behavior Module Level 1 |
| `overscroll-behavior-block` | CSS Overscroll Behavior Module Level 1 |
| `overscroll-behavior-inline` | CSS Overscroll Behavior Module Level 1 |
| `overscroll-behavior-x` | CSS Overscroll Behavior Module Level 1 |
| `overscroll-behavior-y` | CSS Overscroll Behavior Module Level 1 |
| `padding` | CSS Box Model Module Level 3 |
| `padding-block` | CSS Logical Properties and Values Level 1 |
| `padding-block-end` | CSS Logical Properties and Values Level 1 |
| `padding-block-start` | CSS Logical Properties and Values Level 1 |
| `padding-bottom` | CSS Box Model Module Level 3 |
| `padding-inline` | CSS Logical Properties and Values Level 1 |
| `padding-inline-end` | CSS Logical Properties and Values Level 1 |
| `padding-inline-start` | CSS Logical Properties and Values Level 1 |
| `padding-left` | CSS Box Model Module Level 3 |
| `padding-right` | CSS Box Model Module Level 3 |
| `padding-top` | CSS Box Model Module Level 3 |
| `page` | CSS Paged Media Module Level 3 |
| `page-break-after` | CSS 2.1 |
| `page-break-before` | CSS 2.1 |
| `page-break-inside` | CSS 2.1 |
| `pause` | CSS 2.1 |
| `pause-after` | CSS 2.1 |
| `pause-before` | CSS 2.1 |
| `perspective` | CSS Transforms Module Level 2 |
| `perspective-origin` | CSS Transforms Module Level 2 |
| `pitch` | CSS 2.1 |
| `pitch-range` | CSS 2.1 |
| `place-content` | CSS Box Alignment Module Level 3 |
| `place-items` | CSS Box Alignment Module Level 3 |
| `place-self` | CSS Box Alignment Module Level 3 |
| `play-during` | CSS 2.1 |
| `position` | CSS 2.1 |
| `position-anchor` | CSS Anchor Positioning |
| `position-try` | CSS Anchor Positioning |
| `position-try-options` | CSS Anchor Positioning |
| `position-try-order` | CSS Anchor Positioning |
| `print-color-adjust` | CSS Color Adjustment Module Level 1 |
| `quotes` | CSS 2.1 |
| `region-fragment` | CSS Regions Module Level 1 |
| `resize` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `rest` | CSS Speech Module Level 1 |
| `rest-after` | CSS Speech Module Level 1 |
| `rest-before` | CSS Speech Module Level 1 |
| `richness` | CSS 2.1 |
| `right` | CSS 2.1 |
| `rotate` | CSS Transforms Module Level 2 |
| `row-gap` | CSS Box Alignment Module Level 3 |
| `ruby-align` | CSS Ruby Annotation Layout Module Level 1 |
| `ruby-merge` | CSS Ruby Annotation Layout Module Level 1 |
| `ruby-overhang` | CSS Ruby Annotation Layout Module Level 1 |
| `ruby-position` | CSS Ruby Annotation Layout Module Level 1 |
| `running` | CSS Generated Content for Paged Media Module |
| `scale` | CSS Transforms Module Level 2 |
| `scroll-behavior` | CSS Overflow Module Level 3 |
| `scroll-margin` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-block` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-block-end` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-block-start` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-bottom` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-inline` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-inline-end` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-inline-start` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-left` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-right` | CSS Scroll Snap Module Level 1 |
| `scroll-margin-top` | CSS Scroll Snap Module Level 1 |
| `scroll-padding` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-block` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-block-end` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-block-start` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-bottom` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-inline` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-inline-end` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-inline-start` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-left` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-right` | CSS Scroll Snap Module Level 1 |
| `scroll-padding-top` | CSS Scroll Snap Module Level 1 |
| `scroll-snap-align` | CSS Scroll Snap Module Level 1 |
| `scroll-snap-stop` | CSS Scroll Snap Module Level 1 |
| `scroll-snap-type` | CSS Scroll Snap Module Level 1 |
| `scroll-timeline` | Scroll-driven Animations |
| `scroll-timeline-axis` | Scroll-driven Animations |
| `scroll-timeline-name` | Scroll-driven Animations |
| `scrollbar-color` | CSS Scrollbars Styling Module Level 1 |
| `scrollbar-gutter` | CSS Overflow Module Level 3 |
| `scrollbar-width` | CSS Scrollbars Styling Module Level 1 |
| `shape-image-threshold` | CSS Shapes Module Level 1 |
| `shape-inside` | CSS Round Display Level 1 |
| `shape-margin` | CSS Shapes Module Level 1 |
| `shape-outside` | CSS Shapes Module Level 1 |
| `spatial-navigation-action` | CSS Spatial Navigation Level 1 |
| `spatial-navigation-contain` | CSS Spatial Navigation Level 1 |
| `spatial-navigation-function` | CSS Spatial Navigation Level 1 |
| `speak` | CSS 2.1 |
| `speak-as` | CSS Speech Module Level 1 |
| `speak-header` | CSS 2.1 |
| `speak-numeral` | CSS 2.1 |
| `speak-punctuation` | CSS 2.1 |
| `speech-rate` | CSS 2.1 |
| `stress` | CSS 2.1 |
| `string-set` | CSS Generated Content for Paged Media Module |
| `stroke` | CSS Fill and Stroke Module Level 3 |
| `stroke-align` | CSS Fill and Stroke Module Level 3 |
| `stroke-alignment` | SVG Strokes |
| `stroke-break` | CSS Fill and Stroke Module Level 3 |
| `stroke-color` | CSS Fill and Stroke Module Level 3 |
| `stroke-dash-corner` | CSS Fill and Stroke Module Level 3 |
| `stroke-dash-justify` | CSS Fill and Stroke Module Level 3 |
| `stroke-dashadjust` | SVG Strokes |
| `stroke-dasharray` | CSS Fill and Stroke Module Level 3 |
| `stroke-dashcorner` | SVG Strokes |
| `stroke-dashoffset` | CSS Fill and Stroke Module Level 3 |
| `stroke-image` | CSS Fill and Stroke Module Level 3 |
| `stroke-linecap` | CSS Fill and Stroke Module Level 3 |
| `stroke-linejoin` | CSS Fill and Stroke Module Level 3 |
| `stroke-miterlimit` | CSS Fill and Stroke Module Level 3 |
| `stroke-opacity` | CSS Fill and Stroke Module Level 3 |
| `stroke-origin` | CSS Fill and Stroke Module Level 3 |
| `stroke-position` | CSS Fill and Stroke Module Level 3 |
| `stroke-repeat` | CSS Fill and Stroke Module Level 3 |
| `stroke-size` | CSS Fill and Stroke Module Level 3 |
| `stroke-width` | CSS Fill and Stroke Module Level 3 |
| `tab-size` | CSS Text Module Level 3 |
| `table-layout` | CSS 2.1 |
| `text-align` | CSS 2.1 |
| `text-align-all` | CSS Text Module Level 3 |
| `text-align-last` | CSS Text Module Level 3 |
| `text-autospace` | CSS Text Module Level 4 |
| `text-box-edge` | CSS Inline Layout Module Level 3 |
| `text-box-trim` | CSS Inline Layout Module Level 3 |
| `text-combine-upright` | CSS Writing Modes Level 3 |
| `text-decoration` | CSS 2.1 |
| `text-decoration-color` | CSS Text Decoration Module Level 3 |
| `text-decoration-line` | CSS Text Decoration Module Level 3 |
| `text-decoration-skip` | CSS Text Decoration Module Level 4 |
| `text-decoration-skip-box` | CSS Text Decoration Module Level 4 |
| `text-decoration-skip-ink` | CSS Text Decoration Module Level 4 |
| `text-decoration-skip-inset` | CSS Text Decoration Module Level 4 |
| `text-decoration-skip-self` | CSS Text Decoration Module Level 4 |
| `text-decoration-skip-spaces` | CSS Text Decoration Module Level 4 |
| `text-decoration-style` | CSS Text Decoration Module Level 3 |
| `text-decoration-thickness` | CSS Text Decoration Module Level 4 |
| `text-emphasis` | CSS Text Decoration Module Level 3 |
| `text-emphasis-color` | CSS Text Decoration Module Level 3 |
| `text-emphasis-position` | CSS Text Decoration Module Level 3 |
| `text-emphasis-skip` | CSS Text Decoration Module Level 4 |
| `text-emphasis-style` | CSS Text Decoration Module Level 3 |
| `text-group-align` | CSS Text Module Level 4 |
| `text-indent` | CSS 2.1 |
| `text-justify` | CSS Text Module Level 3 |
| `text-orientation` | CSS Writing Modes Level 3 |
| `text-overflow` | CSS Basic User Interface Module Level 3 (CSS3 UI) |
| `text-shadow` | CSS Text Decoration Module Level 3 |
| `text-spacing` | CSS Text Module Level 4 |
| `text-spacing-trim` | CSS Text Module Level 4 |
| `text-transform` | CSS 2.1 |
| `text-underline-offset` | CSS Text Decoration Module Level 4 |
| `text-underline-position` | CSS Text Decoration Module Level 3 |
| `text-wrap` | CSS Text Module Level 4 |
| `text-wrap-mode` | CSS Text Module Level 4 |
| `text-wrap-style` | CSS Text Module Level 4 |
| `timeline-scope` | Scroll-driven Animations |
| `top` | CSS 2.1 |
| `transform` | CSS Transforms Module Level 1 |
| `transform-box` | CSS Transforms Module Level 1 |
| `transform-origin` | CSS Transforms Module Level 1 |
| `transform-style` | CSS Transforms Module Level 2 |
| `transition` | CSS Transitions |
| `transition-behavior` | CSS Transitions Level 2 |
| `transition-delay` | CSS Transitions |
| `transition-duration` | CSS Transitions |
| `transition-property` | CSS Transitions |
| `transition-timing-function` | CSS Transitions |
| `translate` | CSS Transforms Module Level 2 |
| `unicode-bidi` | CSS Writing Modes Level 3 |
| `user-select` | CSS Basic User Interface Module Level 4 |
| `vertical-align` | CSS 2.1 |
| `view-timeline` | Scroll-driven Animations |
| `view-timeline-axis` | Scroll-driven Animations |
| `view-timeline-inset` | Scroll-driven Animations |
| `view-timeline-name` | Scroll-driven Animations |
| `view-transition-class` | CSS View Transitions Module Level 2 |
| `view-transition-name` | CSS View Transitions Module Level 1 |
| `visibility` | CSS 2.1 |
| `voice-balance` | CSS Speech Module Level 1 |
| `voice-duration` | CSS Speech Module Level 1 |
| `voice-family` | CSS 2.1 |
| `voice-pitch` | CSS Speech Module Level 1 |
| `voice-range` | CSS Speech Module Level 1 |
| `voice-rate` | CSS Speech Module Level 1 |
| `voice-stress` | CSS Speech Module Level 1 |
| `voice-volume` | CSS Speech Module Level 1 |
| `volume` | CSS 2.1 |
| `white-space` | CSS 2.1 |
| `white-space-collapse` | CSS Text Module Level 4 |
| `white-space-trim` | CSS Text Module Level 4 |
| `widows` | CSS 2.1 |
| `width` | CSS 2.1 |
| `will-change` | CSS Will Change Module Level 1 |
| `word-break` | CSS Text Module Level 3 |
| `word-space-transform` | CSS Text Module Level 4 |
| `word-spacing` | CSS 2.1 |
| `word-wrap` | CSS Text Module Level 3 |
| `wrap-after` | CSS Text Module Level 4 |
| `wrap-before` | CSS Text Module Level 4 |
| `wrap-flow` | CSS Exclusions Module Level 1 |
| `wrap-inside` | CSS Text Module Level 4 |
| `wrap-through` | CSS Exclusions Module Level 1 |
| `writing-mode` | CSS Writing Modes Level 3 |
| `z-index` | CSS 2.1 |
| `--*` | CSS Custom Properties for Cascading Variables Module Level 1 |

## at-Rules

Memorize the CSS at-rules, to explore additional ways of styling documents and web apps.

* `@annotation`
* `@character-variant`
* `@charset`
* `@counter-style`
* `@font-face`
* `@font-feature-values`
* `@font-palette-values`
* `@historical-forms`
* `@import`
* `@keyframes`
* `@layer`
* `@media`
* `@page`
* `@namespace`
* `@ornaments`
* `@property`
* `@scope`
* `@starting-style`
* `@styleset`
* `@stylistic`
* `@supports`
* `@swash`

I> Whenever you have a question related to CSS, remember to always consult [the CSS specifications](https://www.w3.org/Style/CSS/Overview.en.html) first.

{pagebreak}