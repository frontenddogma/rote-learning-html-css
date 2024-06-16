# CSS

This section covers CSS as per the [CSS Snapshot 2023](https://www.w3.org/TR/css-2023/). However, it also considers CSS working drafts, which are subject to change.

## Selectors

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
| Attribute presence and value selector | `E[foo="bar"]` |
| Case-sensitivity | `E[foo="bar" i]` |
| Case-sensitivity | `E[foo="bar" s]` |
| Attribute presence and value selector | `E[foo~="bar"]` |
| Substring matching attribute selector | `E[foo^="bar"]` |
| Substring matching attribute selector | `E[foo$="bar"]` |
| Substring matching attribute selector | `E[foo*="bar"]` |
| Attribute presence and value selector | `E[foo|="en"]` |
| Directionality pseudo-class `:dir()` | `E:dir(ltr)` |
| Language pseudo-class `:lang()` | `E:lang(zh, "*-hant")` |
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

@@ https://www.w3.org/TR/css-2023/#properties

## at-Rules

@@ https://www.w3.org/TR/css-2023/#at-rules

I> Whenever you have a question related to CSS, remember to always consult [the CSS specifications](https://www.w3.org/Style/CSS/Overview.en.html) first.