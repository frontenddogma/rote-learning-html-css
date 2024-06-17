# CSS {#toc-css}

This section covers CSS as per the [CSS Snapshot 2023](https://www.w3.org/TR/css-2023/). However, it also considers CSS working drafts, which are subject to change.

I> Identifying and maintaining overviews of CSS selectors, at-rules, and especially properties, including their status and support, is a notoriously difficult task. For CSS properties, the best resource may be the [_List of CSS Properties, Both Proposed and Standard_](https://www.w3.org/Style/CSS/all-properties.en.html), maintained by Bert Bos (W3C). Usually, as in this case, collecting this information requires consulting various specifications, and still comes with a good probability of error.

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
| Column combinator (`||`) | `F || E` |
| Class selector | `E.warning` |
| ID selector | `E#myid` |
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
| Attribute presence and value selector | `E[foo]` |
| Attribute presence and value selector | `E[foo='bar']` |
| Case-sensitivity | `E[foo='bar' i]` |
| Case-sensitivity | `E[foo='bar' s]` |
| Attribute presence and value selector | `E[foo~='bar']` |
| Substring matching attribute selector | `E[foo^='bar']` |
| Substring matching attribute selector | `E[foo$='bar']` |
| Substring matching attribute selector | `E[foo*='bar']` |
| Attribute presence and value selector | `E[foo|='en']` |
| Directionality pseudo-class `:dir()` | `E:dir(ltr)` |
| Language pseudo-class `:lang()` | `E:lang(zh, '*-hant')` |
| Hyperlink pseudo-class `:any-link` | `E:any-link` |
| Link history pseudo-class | `E:link` |
| Link history pseudo-class | `E:visited` |
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

Memorize the CSS properties, to add to your sense for what CSS may allow you to do.

1. `--*` (custom properties)
1. `accent-color`
1. `align-content`
1. `align-items`
1. `align-self`
1. `alignment-baseline`
1. `all`
1. `anchor-name`
1. `anchor-scope`
1. `animation`
1. `animation-composition`
1. `animation-delay`
1. `animation-direction`
1. `animation-duration`
1. `animation-fill-mode`
1. `animation-iteration-count`
1. `animation-name`
1. `animation-play-state`
1. `animation-range`
1. `animation-range-end`
1. `animation-range-start`
1. `animation-timeline`
1. `animation-timing-function`
1. `appearance`
1. `aspect-ratio`
1. `azimuth`
1. `backface-visibility`
1. `background`
1. `background-attachment`
1. `background-blend-mode`
1. `background-clip`
1. `background-color`
1. `background-image`
1. `background-origin`
1. `background-position`
1. `background-repeat`
1. `background-size`
1. `baseline-shift`
1. `baseline-source`
1. `block-ellipsis`
1. `block-size`
1. `block-step`
1. `block-step-align`
1. `block-step-insert`
1. `block-step-round`
1. `block-step-size`
1. `bookmark-label`
1. `bookmark-level`
1. `bookmark-state`
1. `border`
1. `border-block`
1. `border-block-color`
1. `border-block-end`
1. `border-block-end-color`
1. `border-block-end-style`
1. `border-block-end-width`
1. `border-block-start`
1. `border-block-start-color`
1. `border-block-start-style`
1. `border-block-start-width`
1. `border-block-style`
1. `border-block-width`
1. `border-bottom`
1. `border-bottom-color`
1. `border-bottom-left-radius`
1. `border-bottom-right-radius`
1. `border-bottom-style`
1. `border-bottom-width`
1. `border-boundary`
1. `border-collapse`
1. `border-color`
1. `border-end-end-radius`
1. `border-end-start-radius`
1. `border-image`
1. `border-image-outset`
1. `border-image-repeat`
1. `border-image-slice`
1. `border-image-source`
1. `border-image-width`
1. `border-inline`
1. `border-inline-color`
1. `border-inline-end`
1. `border-inline-end-color`
1. `border-inline-end-style`
1. `border-inline-end-width`
1. `border-inline-start`
1. `border-inline-start-color`
1. `border-inline-start-style`
1. `border-inline-start-width`
1. `border-inline-style`
1. `border-inline-width`
1. `border-left`
1. `border-left-color`
1. `border-left-style`
1. `border-left-width`
1. `border-radius`
1. `border-right`
1. `border-right-color`
1. `border-right-style`
1. `border-right-width`
1. `border-spacing`
1. `border-start-end-radius`
1. `border-start-start-radius`
1. `border-style`
1. `border-top`
1. `border-top-color`
1. `border-top-left-radius`
1. `border-top-right-radius`
1. `border-top-style`
1. `border-top-width`
1. `border-width`
1. `bottom`
1. `box-decoration-break`
1. `box-shadow`
1. `box-sizing`
1. `box-snap`
1. `break-after`
1. `break-before`
1. `break-inside`
1. `caption-side`
1. `caret`
1. `caret-color`
1. `caret-shape`
1. `chains`
1. `clear`
1. `clip`
1. `clip-path`
1. `clip-rule`
1. `color`
1. `color-adjust`
1. `color-interpolation-filters`
1. `color-scheme`
1. `column-count`
1. `column-fill`
1. `column-gap`
1. `column-rule`
1. `column-rule-color`
1. `column-rule-style`
1. `column-rule-width`
1. `column-span`
1. `column-width`
1. `columns`
1. `contain`
1. `contain-intrinsic-block-size`
1. `contain-intrinsic-height`
1. `contain-intrinsic-inline-size`
1. `contain-intrinsic-size`
1. `contain-intrinsic-width`
1. `container`
1. `container-name`
1. `container-type`
1. `content`
1. `content-visibility`
1. `continue`
1. `counter-increment`
1. `counter-reset`
1. `counter-set`
1. `cue`
1. `cue-after`
1. `cue-before`
1. `cursor`
1. `direction`
1. `display`
1. `dominant-baseline`
1. `elevation`
1. `empty-cells`
1. `fill`
1. `fill-break`
1. `fill-color`
1. `fill-image`
1. `fill-opacity`
1. `fill-origin`
1. `fill-position`
1. `fill-repeat`
1. `fill-rule`
1. `fill-size`
1. `filter`
1. `flex`
1. `flex-basis`
1. `flex-direction`
1. `flex-flow`
1. `flex-grow`
1. `flex-shrink`
1. `flex-wrap`
1. `float`
1. `float-defer`
1. `float-offset`
1. `float-reference`
1. `flood-color`
1. `flood-opacity`
1. `flow`
1. `flow-from`
1. `flow-into`
1. `font`
1. `font-family`
1. `font-feature-settings`
1. `font-kerning`
1. `font-language-override`
1. `font-optical-sizing`
1. `font-palette`
1. `font-size`
1. `font-size-adjust`
1. `font-stretch`
1. `font-style`
1. `font-synthesis`
1. `font-synthesis-position`
1. `font-synthesis-small-caps`
1. `font-synthesis-style`
1. `font-synthesis-weight`
1. `font-variant`
1. `font-variant-alternates`
1. `font-variant-caps`
1. `font-variant-east-asian`
1. `font-variant-emoji`
1. `font-variant-ligatures`
1. `font-variant-numeric`
1. `font-variant-position`
1. `font-variation-settings`
1. `font-weight`
1. `font-width`
1. `footnote-display`
1. `footnote-policy`
1. `forced-color-adjust`
1. `gap`
1. `glyph-orientation-vertical`
1. `grid`
1. `grid-area`
1. `grid-auto-columns`
1. `grid-auto-flow`
1. `grid-auto-rows`
1. `grid-column`
1. `grid-column-end`
1. `grid-column-start`
1. `grid-row`
1. `grid-row-end`
1. `grid-row-start`
1. `grid-template`
1. `grid-template-areas`
1. `grid-template-columns`
1. `grid-template-rows`
1. `hanging-punctuation`
1. `height`
1. `hyphenate-character`
1. `hyphenate-limit-chars`
1. `hyphenate-limit-last`
1. `hyphenate-limit-lines`
1. `hyphenate-limit-zone`
1. `hyphens`
1. `image-orientation`
1. `image-rendering`
1. `image-resolution`
1. `initial-letter`
1. `initial-letter-align`
1. `initial-letter-wrap`
1. `inline-size`
1. `inline-sizing`
1. `inset`
1. `inset-area`
1. `inset-block`
1. `inset-block-end`
1. `inset-block-start`
1. `inset-inline`
1. `inset-inline-end`
1. `inset-inline-start`
1. `isolation`
1. `justify-content`
1. `justify-items`
1. `justify-self`
1. `left`
1. `letter-spacing`
1. `lighting-color`
1. `line-break`
1. `line-clamp`
1. `line-grid`
1. `line-height`
1. `line-height-step`
1. `line-padding`
1. `line-snap`
1. `list-style`
1. `list-style-image`
1. `list-style-position`
1. `list-style-type`
1. `margin`
1. `margin-block`
1. `margin-block-end`
1. `margin-block-start`
1. `margin-bottom`
1. `margin-break`
1. `margin-inline`
1. `margin-inline-end`
1. `margin-inline-start`
1. `margin-left`
1. `margin-right`
1. `margin-top`
1. `margin-trim`
1. `marker`
1. `marker-end`
1. `marker-knockout-left`
1. `marker-knockout-right`
1. `marker-mid`
1. `marker-pattern`
1. `marker-segment`
1. `marker-side`
1. `marker-start`
1. `mask`
1. `mask-border`
1. `mask-border-mode`
1. `mask-border-outset`
1. `mask-border-repeat`
1. `mask-border-slice`
1. `mask-border-source`
1. `mask-border-width`
1. `mask-clip`
1. `mask-composite`
1. `mask-image`
1. `mask-mode`
1. `mask-origin`
1. `mask-position`
1. `mask-repeat`
1. `mask-size`
1. `mask-type`
1. `max-block-size`
1. `max-height`
1. `max-inline-size`
1. `max-lines`
1. `max-width`
1. `min-block-size`
1. `min-height`
1. `min-inline-size`
1. `min-intrinsic-sizing`
1. `min-width`
1. `mix-blend-mode`
1. `nav-down`
1. `nav-left`
1. `nav-right`
1. `nav-up`
1. `object-fit`
1. `object-position`
1. `offset`
1. `offset-anchor`
1. `offset-distance`
1. `offset-path`
1. `offset-position`
1. `offset-rotate`
1. `opacity`
1. `order`
1. `orphans`
1. `outline`
1. `outline-color`
1. `outline-offset`
1. `outline-style`
1. `outline-width`
1. `overflow`
1. `overflow-anchor`
1. `overflow-block`
1. `overflow-clip-margin`
1. `overflow-clip-margin-block`
1. `overflow-clip-margin-block-end`
1. `overflow-clip-margin-block-start`
1. `overflow-clip-margin-bottom`
1. `overflow-clip-margin-inline`
1. `overflow-clip-margin-inline-end`
1. `overflow-clip-margin-inline-start`
1. `overflow-clip-margin-left`
1. `overflow-clip-margin-right`
1. `overflow-clip-margin-top`
1. `overflow-inline`
1. `overflow-wrap`
1. `overflow-x`
1. `overflow-y`
1. `overscroll-behavior`
1. `overscroll-behavior-block`
1. `overscroll-behavior-inline`
1. `overscroll-behavior-x`
1. `overscroll-behavior-y`
1. `padding`
1. `padding-block`
1. `padding-block-end`
1. `padding-block-start`
1. `padding-bottom`
1. `padding-inline`
1. `padding-inline-end`
1. `padding-inline-start`
1. `padding-left`
1. `padding-right`
1. `padding-top`
1. `page`
1. `page-break-after`
1. `page-break-before`
1. `page-break-inside`
1. `pause`
1. `pause-after`
1. `pause-before`
1. `perspective`
1. `perspective-origin`
1. `pitch`
1. `pitch-range`
1. `place-content`
1. `place-items`
1. `place-self`
1. `play-during`
1. `position`
1. `position-anchor`
1. `position-try`
1. `position-try-options`
1. `position-try-order`
1. `print-color-adjust`
1. `quotes`
1. `region-fragment`
1. `resize`
1. `rest`
1. `rest-after`
1. `rest-before`
1. `richness`
1. `right`
1. `rotate`
1. `row-gap`
1. `ruby-align`
1. `ruby-merge`
1. `ruby-overhang`
1. `ruby-position`
1. `running`
1. `scale`
1. `scroll-behavior`
1. `scroll-margin`
1. `scroll-margin-block`
1. `scroll-margin-block-end`
1. `scroll-margin-block-start`
1. `scroll-margin-bottom`
1. `scroll-margin-inline`
1. `scroll-margin-inline-end`
1. `scroll-margin-inline-start`
1. `scroll-margin-left`
1. `scroll-margin-right`
1. `scroll-margin-top`
1. `scroll-padding`
1. `scroll-padding-block`
1. `scroll-padding-block-end`
1. `scroll-padding-block-start`
1. `scroll-padding-bottom`
1. `scroll-padding-inline`
1. `scroll-padding-inline-end`
1. `scroll-padding-inline-start`
1. `scroll-padding-left`
1. `scroll-padding-right`
1. `scroll-padding-top`
1. `scroll-snap-align`
1. `scroll-snap-stop`
1. `scroll-snap-type`
1. `scroll-timeline`
1. `scroll-timeline-axis`
1. `scroll-timeline-name`
1. `scrollbar-color`
1. `scrollbar-gutter`
1. `scrollbar-width`
1. `shape-image-threshold`
1. `shape-inside`
1. `shape-margin`
1. `shape-outside`
1. `spatial-navigation-action`
1. `spatial-navigation-contain`
1. `spatial-navigation-function`
1. `speak`
1. `speak-as`
1. `speak-header`
1. `speak-numeral`
1. `speak-punctuation`
1. `speech-rate`
1. `stress`
1. `string-set`
1. `stroke`
1. `stroke-align`
1. `stroke-alignment`
1. `stroke-break`
1. `stroke-color`
1. `stroke-dash-corner`
1. `stroke-dash-justify`
1. `stroke-dashadjust`
1. `stroke-dasharray`
1. `stroke-dashcorner`
1. `stroke-dashoffset`
1. `stroke-image`
1. `stroke-linecap`
1. `stroke-linejoin`
1. `stroke-miterlimit`
1. `stroke-opacity`
1. `stroke-origin`
1. `stroke-position`
1. `stroke-repeat`
1. `stroke-size`
1. `stroke-width`
1. `tab-size`
1. `table-layout`
1. `text-align`
1. `text-align-all`
1. `text-align-last`
1. `text-autospace`
1. `text-box-edge`
1. `text-box-trim`
1. `text-combine-upright`
1. `text-decoration`
1. `text-decoration-color`
1. `text-decoration-line`
1. `text-decoration-skip`
1. `text-decoration-skip-box`
1. `text-decoration-skip-ink`
1. `text-decoration-skip-inset`
1. `text-decoration-skip-self`
1. `text-decoration-skip-spaces`
1. `text-decoration-style`
1. `text-decoration-thickness`
1. `text-emphasis`
1. `text-emphasis-color`
1. `text-emphasis-position`
1. `text-emphasis-skip`
1. `text-emphasis-style`
1. `text-group-align`
1. `text-indent`
1. `text-justify`
1. `text-orientation`
1. `text-overflow`
1. `text-shadow`
1. `text-spacing`
1. `text-spacing-trim`
1. `text-transform`
1. `text-underline-offset`
1. `text-underline-position`
1. `text-wrap`
1. `text-wrap-mode`
1. `text-wrap-style`
1. `timeline-scope`
1. `top`
1. `transform`
1. `transform-box`
1. `transform-origin`
1. `transform-style`
1. `transition`
1. `transition-behavior`
1. `transition-delay`
1. `transition-duration`
1. `transition-property`
1. `transition-timing-function`
1. `translate`
1. `unicode-bidi`
1. `user-select`
1. `vertical-align`
1. `view-timeline`
1. `view-timeline-axis`
1. `view-timeline-inset`
1. `view-timeline-name`
1. `view-transition-class`
1. `view-transition-name`
1. `visibility`
1. `voice-balance`
1. `voice-duration`
1. `voice-family`
1. `voice-pitch`
1. `voice-range`
1. `voice-rate`
1. `voice-stress`
1. `voice-volume`
1. `volume`
1. `white-space`
1. `white-space-collapse`
1. `white-space-trim`
1. `widows`
1. `width`
1. `will-change`
1. `word-break`
1. `word-space-transform`
1. `word-spacing`
1. `word-wrap`
1. `wrap-after`
1. `wrap-before`
1. `wrap-flow`
1. `wrap-inside`
1. `wrap-through`
1. `writing-mode`
1. `z-index`

## at-Rules

Memorize the CSS at-rules, to explore additional ways of styling documents and apps.

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
* `@media`
* `@page`
* `@namespace`
* `@ornaments`
* `@property`
* `@scope`
* `@styleset`
* `@stylistic`
* `@supports`
* `@swash`

I> Whenever you have a question related to CSS, remember to always consult [the CSS specifications](https://www.w3.org/Style/CSS/Overview.en.html) first.

{pagebreak}