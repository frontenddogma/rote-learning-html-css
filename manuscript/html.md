# HTML

This section covers HTML as per [the living standard](https://html.spec.whatwg.org/multipage/) in <!-- @@ -->June and July 2024. Elements from earlier HTML specifications and proprietary elements are not included.

### Element Meanings

Memorize the elements and their meanings (semantics):

* `a`: Anchor (hyperlink)
* `abbr`: Abbreviation
* `address`: Contact information
* `area`: Image map area
* `article`: Self-contained and distributable content
* `aside`: Related content
* `audio`: Audio content
* `b`: Attention
* `base`: Base URL
* `bdi`: Bidi isolation
* `bdo`: Bidi override
* `blockquote`: Long quotation
* `body`: Document body
* `br`: Line break
* `button`: Button
* `canvas`: Scriptable bitmap
* `caption`: Table caption
* `cite`: Citation
* `code`: Code fragment
* `col`: Table column
* `colgroup`: Table column group
* `data`: Content with machine-readable equivalent
* `datalist`: Predefined options for form controls
* `dd`: Description
* `del`: Deleted text
* `details`: Disclosure widget
* `dfn`: Instance definition
* `dialog`: User interaction
* `div`: Generic container
* `dl`: Description list
* `dt`: Description term
* `em`: Emphasis
* `embed`: Integration point
* `fieldset`: Form control group
* `figcaption`: `figure` caption
* `figure`: Self-contained flow content
* `footer`: Footer
* `form`: Form
* `h1`: Heading
* `h2`: Heading
* `h3`: Heading
* `h4`: Heading
* `h5`: Heading
* `h6`: Heading
* `head`: Document head
* `header`: Header
* `hgroup`: Heading and related content
* `hr`: Thematic break
* `html`: Document root
* `i`: Alternate voice
* `iframe`: Inline subwindow
* `img`: Image content
* `input`: Input field
* `ins`: Inserted text
* `kbd`: User input
* `label`: Form control caption
* `legend`: `fieldset` caption
* `li`: List item
* `link`: Resource link
* `main`: Dominant content
* `map`: Image map
* `mark`: Marked reference text
* `math`: MathML container
* `menu`: Menu list
* `meta`: Metadata
* `meter`: Scalar measurement
* `nav`: Navigation section
* `noscript`: Script fallback
* `object`: Generic content
* `ol`: Ordered list
* `optgroup`: `option` group
* `option`: Selectable choice
* `output`: Calculation or user action output
* `p`: Paragraph
* `picture`: Extended image content
* `pre`: Preformatted text
* `progress`: Progress of a task
* `q`: Short quotation
* `rp`: Ruby parentheses
* `rt`: Ruby text
* `ruby`: Ruby annotation(s)
* `s`: Irrelevance
* `samp`: Sample output
* `script`: Script
* `search`: Search controls or content
* `section`: Generic section
* `select`: `option` selector
* `slot`: Shadow tree slot
* `small`: Small print
* `source`: Media content
* `span`: Generic container
* `strong`: Importance
* `style`: Formatting
* `sub`: Subscript
* `summary`: `details` caption
* `sup`: Superscript
* `svg`: SVG container
* `table`: Table
* `tbody`: Table body
* `td`: Table data cell
* `template`: Fragment declaration
* `textarea`: Multi-line input field
* `tfoot`: Table footer
* `th`: Table header cell
* `thead`: Table header
* `time`: Date, time, time zone offset, or duration
* `title`: Document title
* `tr`: Table row
* `track`: Text track
* `u`: Annotation
* `ul`: Unordered list
* `var`: Variable
* `video`: Video content
* `wbr`: Line break opportunity

(Autonomous custom elements are not included in this list.)

## Void Elements

Memorize the elements that are void, i.e., that have no end tag in the HTML syntax:

* `area`
* `base`
* `br`
* `col`
* `embed`
* `hr`
* `img`
* `input`
* `link`
* `meta`
* `source`
* `track`
* `wbr`

In true HTML, you write these elements as `<elementname>`, e.g., `<area>`, `<img>`, or `<meta>`. There is no end tag and no slash.

## Elements With Optional Start or End Tags

Memorize the elements that have optional start and/or end tags. Void elements don’t have an end tag and are therefore included (but also called out) as well.

| Element | Void? | Optional Start Tag? | Optional End Tag? |
| --- | --- | --- | --- |
| `area` | Yes | No | Yes (void) |
| `base` | Yes | No | Yes (void) |
| `body` | No | Yes | Yes |
| `br` | Yes | No | Yes (void) |
| `caption` | No | No | Yes |
| `col` | Yes | No | Yes (void) |
| `colgroup` | No | Yes | Yes |
| `dd` | No | No | Yes |
| `dt` | No | No | Yes |
| `embed` | Yes | No | Yes (void) |
| `figcaption` | No | No | Yes |
| `head` | No | Yes | Yes |
| `hr` | Yes | No | Yes (void) |
| `html` | No | Yes | Yes |
| `img` | Yes | No | Yes (void) |
| `input` | Yes | No | Yes (void) |
| `li` | No | No | Yes |
| `link` | Yes | No | Yes (void) |
| `meta` | Yes | No | Yes (void) |
| `optgroup` | No | No | Yes |
| `option` | No | No | Yes |
| `p` | No | No | Yes |
| `rp` | No | No | Yes |
| `rt` | No | No | Yes |
| `source` | Yes | No | Yes (void) |
| `tbody` | No | Yes | Yes |
| `td` | No | No | Yes |
| `tfoot` | No | No | Yes |
| `th` | No | No | Yes |
| `thead` | No | No | Yes |
| `tr` | No | No | Yes |
| `track` | Yes | No | Yes (void) |
| `wbr` | Yes | No | Yes (void) |

### Element Categories

Understand the HTML content categories:

* Metadata content: sets up the presentation or behavior of the rest of a document’s content, sets up the relationship of a document with other documents, or conveys other information.
* Flow content: makes for the `body` of a document.
* Sectioning content: defines the scope of `header` and `footer` elements.
* Heading content: defines the heading of a section.
* Phrasing content: represents the text of a document.
* Embedded content: imports other resources or content into a document.
* Interactive content: serves user interaction.
* Form-associated elements: have a form owner.
* Labelable elements: may be associated with a `label` element.
* Listed elements: are listed in the `form.elements` and `fieldset.elements` APIs.
* Submittable elements: may be used to construct the entry list when a `form` element is being submitted.
* Resettable elements: may be affected when a `form` element is being reset.
* Autocapitalize-inheriting elements: inherit the `autocapitalize` attribute from their form owner.
* Palpable content: makes an element non-empty by providing either non-empty text, or something a user can view, hear, or interact with.
* Script-supporting elements: do not represent anything by themselves, but provide functionality.

Familiarize yourself with what elements are part of which category:

#### Metadata Content

* `base`
* `link`
* `meta`
* `noscript`
* `script`
* `style`
* `template`
* `title`

#### Flow Content

* `a`
* `abbr`
* `address`
* `article`
* `aside`
* `audio`
* `b`
* `bdi`
* `bdo`
* `blockquote`
* `br`
* `button`
* `canvas`
* `cite`
* `code`
* `data`
* `datalist`
* `del`
* `details`
* `dfn`
* `dialog`
* `div`
* `dl`
* `em`
* `embed`
* `fieldset`
* `figure`
* `footer`
* `form`
* `h1`
* `h2`
* `h3`
* `h4`
* `h5`
* `h6`
* `header`
* `hgroup`
* `hr`
* `i`
* `iframe`
* `img`
* `input`
* `ins`
* `kbd`
* `label`
* `map`
* `mark`
* `math` (MathML)
* `menu`
* `meter`
* `nav`
* `noscript`
* `object`
* `ol`
* `output`
* `p`
* `picture`
* `pre`
* `progress`
* `q`
* `ruby`
* `s`
* `samp`
* `script`
* `search`
* `section`
* `select`
* `slot`
* `small`
* `span`
* `strong`
* `sub`
* `sup`
* `svg` (SVG)
* `table`
* `template`
* `textarea`
* `time`
* `u`
* `ul`
* `var`
* `video`
* `wbr`

Also:

* Autonomous custom elements
* Text

Elements that can under certain circumstances be flow content:

* `area`
* `link`
* `main`
* `meta`

#### Sectioning Content

* `article`
* `aside`
* `nav`
* `section`

#### Heading Content

* `h1`
* `h2`
* `h3`
* `h4`
* `h5`
* `h6`
* `hgroup`

#### Phrasing Content

@@ https://html.spec.whatwg.org/multipage/indices.html#element-content-categories

@@ a; abbr; audio; b; bdi; bdo; br; button; canvas; cite; code; data; datalist; del; dfn; em; embed; i; iframe; img; input; ins; kbd; label; map; mark; MathML math; meter; noscript; object; output; picture; progress; q; ruby; s; samp; script; select; slot; small; span; strong; sub; sup; SVG svg; template; textarea; time; u; var; video; wbr; autonomous custom elements; Text	area (if it is a descendant of a map element); link (if it is allowed in the body); meta (if the itemprop attribute is present)

#### Embedded Content

@@ audio; canvas; embed; iframe; img; MathML math; object; picture; SVG svg; video

#### Interactive Content

@@ button; details; embed; iframe; label; select; textarea	a (if the href attribute is present); audio (if the controls attribute is present); img (if the usemap attribute is present); input (if the type attribute is not in the Hidden state); video (if the controls attribute is present)

#### Form-Associated Elements

@@ button; fieldset; input; label; object; output; select; textarea; img; form-associated custom elements

#### Labelable Elements

@@ button; input; meter; output; progress; select; textarea; form-associated custom elements

#### Listed Elements

@@ button; fieldset; input; object; output; select; textarea; form-associated custom elements

#### Submittable Elements

@@ button; input; select; textarea; form-associated custom elements

#### Resettable Elements

@@ input; output; select; textarea; form-associated custom elements

#### Autocapitalize-Inheriting Elements

@@ button; fieldset; input; output; select; textarea

#### Palpable Content

@@ a; abbr; address; article; aside; b; bdi; bdo; blockquote; button; canvas; cite; code; data; del; details; dfn; div; em; embed; fieldset; figure; footer; form; h1; h2; h3; h4; h5; h6; header; hgroup; i; iframe; img; ins; kbd; label; main; map; mark; MathML math; meter; nav; object; output; p; picture; pre; progress; q; ruby; s; samp; search; section; select; small; span; strong; sub; sup; SVG svg; table; textarea; time; u; var; video; autonomous custom elements	audio (if the controls attribute is present); dl (if the element's children include at least one name-value group); input (if the type attribute is not in the Hidden state); menu (if the element's children include at least one li element); ol (if the element's children include at least one li element); ul (if the element's children include at least one li element); Text that is not inter-element whitespace

#### Script-Supporting Elements

@@ script; template

## Attributes

@@ https://html.spec.whatwg.org/multipage/indices.html#attributes-3

### Global Attributes

@@ https://html.spec.whatwg.org/multipage/dom.html#global-attributes

I> Remember to whenever you have a question about HTML, to consult [the HTML specification](https://html.spec.whatwg.org/multipage/).