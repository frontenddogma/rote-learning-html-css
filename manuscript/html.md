# HTML

## Elements <!-- #elements -->

Memorize what elements are part of the HTML standard. (This list only includes element of the living standard—except `math`, `svg`, and custom elements—, and not of previous versions of HTML.)

| Element | Meaning | Void Element? | Start Tag Optional? | End Tag Optional? |
| --- | --- | --- | --- | --- |
| `a` | Anchor (hyperlink) | No | No | No |
| `abbr` | Abbreviation | No | No | No |
| `address` | Contact information | No | No | No |
| `area` | Image map area | Yes | No | Yes (void) |
| `article` | Self-contained and distributable content | No | No | No |
| `aside` | Related content | No | No | No |
| `audio` | Audio content | No | No | No |
| `b` | Attention | No | No | No |
| `base` | Base URL | Yes | No | Yes (void) |
| `bdi` | Bidi isolation | No | No | No |
| `bdo` | Bidi override | No | No | No |
| `blockquote` | Long quotation | No | No | No |
| `body` | Document body | No | Yes | Yes |
| `br` | Line break | Yes | No | Yes (void) |
| `button` | Button | No | No | No |
| `canvas` | Scriptable bitmap | No | No | No |
| `caption` | Table caption | No | No | Yes |
| `cite` | Citation | No | No | No |
| `code` | Code fragment | No | No | No |
| `col` | Table column | Yes | No | Yes (void) |
| `colgroup` | Table column group | No | Yes | Yes |
| `data` | Content with machine-readable equivalent | No | No | No |
| `datalist` | Predefined options for form controls | No | No | No |
| `dd` | Description | No | No | Yes |
| `del` | Deleted text | No | No | No |
| `details` | Disclosure widget | No | No | No |
| `dfn` | Instance definition | No | No | No |
| `dialog` | User interaction | No | No | No |
| `div` | Generic container | No | No | No |
| `dl` | Description list | No | No | No |
| `dt` | Description term | No | No | Yes |
| `em` | Emphasis | No | No | No |
| `embed` | Integration point | Yes | No | Yes (void) |
| `fieldset` | Form control group | No | No | No |
| `figcaption` | `figure` caption | No | No | Yes |
| `figure` | Self-contained flow content | No | No | No |
| `footer` | Footer | No | No | No |
| `form` | Form | No | No | No |
| `h1` | Heading | No | No | No |
| `h2` | Heading | No | No | No |
| `h3` | Heading | No | No | No |
| `h4` | Heading | No | No | No |
| `h5` | Heading | No | No | No |
| `h6` | Heading | No | No | No |
| `head` | Document head | No | Yes | Yes |
| `header` | Header | No | No | No |
| `hgroup` | Heading and related content | No | No | No |
| `hr` | Thematic break | Yes | No | Yes (void) |
| `html` | Document root | No | Yes | Yes |
| `i` | Alternate voice | No | No | No |
| `iframe` | Inline subwindow | No | No | No |
| `img` | Image content | Yes | No | Yes (void) |
| `input` | Input field | Yes | No | Yes (void) |
| `ins` | Inserted text | No | No | No |
| `kbd` | User input | No | No | No |
| `label` | Form control caption | No | No | No |
| `legend` | `fieldset` caption | No | No | No |
| `li` | List item | No | No | Yes |
| `link` | Resource link | Yes | No | Yes (void) |
| `main` | Dominant content | No | No | No |
| `map` | Image map | No | No | No |
| `mark` | Marked reference text | No | No | No |
| `menu` | Menu list | No | No | No |
| `meta` | Metadata | Yes | No | Yes (void) |
| `meter` | Scalar measurement | No | No | No |
| `nav` | Navigation section | No | No | No |
| `noscript` | Script fallback | No | No | No |
| `object` | Generic content | No | No | No |
| `ol` | Ordered list | No | No | No |
| `optgroup` | `option` group | No | No | Yes |
| `option` | Selectable choice | No | No | Yes |
| `output` | Calculation or user action output | No | No | No |
| `p` | Paragraph | No | No | Yes |
| `picture` | Extended image content | No | No | No |
| `pre` | Preformatted text | No | No | No |
| `progress` | Progress of a task | No | No | No |
| `q` | Short quotation | No | No | No |
| `rp` | Ruby parentheses | No | No | Yes |
| `rt` | Ruby text | No | No | Yes |
| `ruby` | Ruby annotation(s) | No | No | No |
| `s` | Irrelevance | No | No | No |
| `samp` | Sample output | No | No | No |
| `script` | Script | No | No | No |
| `search` | Search controls or content | No | No | No |
| `section` | Generic section | No | No | No |
| `select` | `option` selector | No | No | No |
| `slot` | Shadow tree slot | No | No | No |
| `small` | Small print | No | No | No |
| `source` | Media content | Yes | No | Yes (void) |
| `span` | Generic container | No | No | No |
| `strong` | Importance | No | No | No |
| `style` | Formatting | No | No | No |
| `sub` | Subscript | No | No | No |
| `summary` | `details` caption | No | No | No |
| `sup` | Superscript | No | No | No |
| `table` | Table | No | No | No |
| `tbody` | Table body | No | Yes | Yes |
| `td` | Table data cell | No | No | Yes |
| `template` | Fragment declaration | No | No | No |
| `textarea` | Multi-line input field | No | No | No |
| `tfoot` | Table footer | No | No | Yes |
| `th` | Table header cell | No | No | Yes |
| `thead` | Table header | No | No | Yes |
| `time` | Date, time, time zone offset, or duration | No | No | No |
| `title` | Document title | No | No | No |
| `tr` | Table row | No | No | Yes |
| `track` | Text track | Yes | No | Yes (void) |
| `u` | Annotation | No | No | No |
| `ul` | Unordered list | No | No | No |
| `var` | Variable | No | No | No |
| `video` | Video content | No | No | No |
| `wbr` | Line break opportunity | Yes | No | Yes (void) |

### Element Meanings <!-- #elements.semantics -->

Now memorize the elements and their meanings (semantics):

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

@@ https://html.spec.whatwg.org/multipage/indices.html#element-content-categories

Familiarize yourself with what elements are part of which category:

#### Metadata Content

@@ base; link; meta; noscript; script; style; template; title

#### Flow Content

@@ a; abbr; address; article; aside; audio; b; bdi; bdo; blockquote; br; button; canvas; cite; code; data; datalist; del; details; dfn; dialog; div; dl; em; embed; fieldset; figure; footer; form; h1; h2; h3; h4; h5; h6; header; hgroup; hr; i; iframe; img; input; ins; kbd; label; map; mark; MathML math; menu; meter; nav; noscript; object; ol; output; p; picture; pre; progress; q; ruby; s; samp; script; search; section; select; slot; small; span; strong; sub; sup; SVG svg; table; template; textarea; time; u; ul; var; video; wbr; autonomous custom elements; Text	area (if it is a descendant of a map element); link (if it is allowed in the body); main (if it is a hierarchically correct main element); meta (if the itemprop attribute is present)

#### Sectioning Content

@@ article; aside; nav; section

#### Heading Content

@@ h1; h2; h3; h4; h5; h6; hgroup

#### Phrasing Content

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

## Attributes <!-- #attributes -->

@@ https://html.spec.whatwg.org/multipage/indices.html#attributes-3

### Global Attributes <!-- #attributes.global -->

@@ https://html.spec.whatwg.org/multipage/dom.html#global-attributes