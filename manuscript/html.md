# HTML

This section covers HTML as per [the living standard](https://html.spec.whatwg.org/multipage/) in <!-- @@ -->June and July 2024. Elements from earlier HTML specifications and proprietary elements are not included.

## Elements

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

### Void Elements

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

### Elements With Optional Start or End Tags

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

Elements that can be flow content under certain circumstances:

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

* `a`
* `abbr`
* `audio`
* `b`
* `bdi`
* `bdo`
* `br`
* `button`
* `canvas`
* `cite`
* `code`
* `data`
* `datalist`
* `del`
* `dfn`
* `em`
* `embed`
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
* `meter`
* `noscript`
* `object`
* `output`
* `picture`
* `progress`
* `q`
* `ruby`
* `s`
* `samp`
* `script`
* `select`
* `slot`
* `small`
* `span`
* `strong`
* `sub`
* `sup`
* `svg` (SVG)
* `template`
* `textarea`
* `time`
* `u`
* `var`
* `video`
* `wbr`

Also:

* Autonomous custom elements
* Text

Elements that can be phrasing content under certain circumstances:

* `area`
* `link`
* `meta`

#### Embedded Content

* `audio`
* `canvas`
* `embed`
* `iframe`
* `img`
* `math` (MathML)
* `object`
* `picture`
* `svg` (SVG)
* `video`

#### Interactive Content

* `button`
* `details`
* `embed`
* `iframe`
* `label`
* `select`
* `textarea`

Elements that can be interactive content under certain circumstances:

* `a`
* `audio`
* `img`
* `input`
* `video`

#### Form-Associated Elements

* `button`
* `fieldset`
* `input`
* `label`
* `object`
* `output`
* `select`
* `textarea`
* `img`

Also:

* Form-associated custom elements

#### Labelable Elements

* `button`
* `input`
* `meter`
* `output`
* `progress`
* `select`
* `textarea`

Also:

* Form-associated custom elements

#### Listed Elements

* `button`
* `fieldset`
* `input`
* `object`
* `output`
* `select`
* `textarea`

Also:

* Form-associated custom elements

#### Submittable Elements

* `button`
* `input`
* `select`
* `textarea`

Also:

* Form-associated custom elements

#### Resettable Elements

* `input`
* `output`
* `select`
* `textarea`

Also:

* Form-associated custom elements

#### Autocapitalize-Inheriting Elements

* `button`
* `fieldset`
* `input`
* `output`
* `select`
* `textarea

#### Palpable Content

* `a`
* `abbr`
* `address`
* `article`
* `aside`
* `b`
* `bdi`
* `bdo`
* `blockquote`
* `button`
* `canvas`
* `cite`
* `code`
* `data`
* `del`
* `details`
* `dfn`
* `div`
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
* `i`
* `iframe`
* `img`
* `ins`
* `kbd`
* `label`
* `main`
* `map`
* `mark`
* `math` (MathML)
* `meter`
* `nav`
* `object`
* `output`
* `p`
* `picture`
* `pre`
* `progress`
* `q`
* `ruby`
* `s`
* `samp`
* `search`
* `section`
* `select`
* `small`
* `span`
* `strong`
* `sub`
* `sup`
* `svg` (SVG)
* `table`
* `textarea`
* `time`
* `u`
* `var`
* `video`

Also:

* Autonomous custom elements

Elements that can be palpable content under certain circumstances:

* `audio`
* `dl`
* `input`
* `menu`
* `ol`
* `ul`
* Text that isn’t whitespace between elements

#### Script-Supporting Elements

* `script`
* `template`

## Attributes

Memorize all attributes, including event handler attributes. Repeat attribute mentions indicate different meanings. “HTML elements” refers to any element in the “http://www.w3.org/1999/xhtml” namespace namespace (including, as per the specification, XML documents). <!-- @@ Check on https://github.com/whatwg/html/issues/10414 and whether to include `onbeforeinput`! -->

| Attributes | Elements |
| --- | --- |
| `abbr` | `th` |
| `accept` | `input` |
| `accept-charset` | `form` |
| `accesskey` | HTML elements |
| `action` | `form` |
| `allow` | `iframe` |
| `allowfullscreen` | `iframe` |
| `alt` | `area`, `img`, `input` |
| `as` | `link` |
| `async` | `script` |
| `autocapitalize` | HTML elements |
| `autocomplete` | `form` |
| `autocomplete` | `input`, `select`, `textarea` |
| `autofocus` | HTML elements |
| `autoplay` | `audio`, `video` |
| `blocking` | `link`, `script`, `style` |
| `charset` | `meta` |
| `checked` | `input` |
| `cite` | `blockquote`, `del`, `ins`, `q` |
| `class` | HTML elements |
| `color` | `link` |
| `cols` | `textarea` |
| `colspan` | `td`, `th` |
| `content` | `meta` |
| `contenteditable` | HTML elements |
| `controls` | `audio`, `video` |
| `coords` | `area` |
| `crossorigin` | `audio`, `img`, `link`, `script`, `video` |
| `data` | `object` |
| `datetime` | `del`, `ins` |
| `datetime` | `time` |
| `decoding` | `img` |
| `default` | `track` |
| `defer` | `script` |
| `dir` | HTML elements |
| `dir` | `bdo` |
| `dirname` | `input`, `textarea` |
| `disabled` | `button`, `input`, `optgroup`, `option`, `select`, `textarea`, form-associated custom elements |
| `disabled` | `fieldset` |
| `disabled` | `link` |
| `download` | `a`, `area` |
| `draggable` | HTML elements |
| `enctype` | `form` |
| `enterkeyhint` | HTML elements |
| `fetchpriority` | `img`, `link`, `script` |
| `for` | `label` |
| `for` | `output` |
| `form` | `button`, `fieldset`, `input`, `object`, `output`, `select`, `textarea`, form-associated custom elements |
| `formaction` | `button`, `input` |
| `formenctype` | `button`, `input` |
| `formmethod` | `button`, `input` |
| `formnovalidate` | `button`, `input` |
| `formtarget` | `button`, `input` |
| `headers` | `td`, `th` |
| `height` | `canvas`, `embed`, `iframe`, `img`, `input`, `object`, `source` (`picture`), `video` |
| `hidden` | HTML elements |
| `high` | `meter` |
| `href` | `a`, `area` |
| `href` | `link` |
| `href` | `base` |
| `hreflang` | `a`, `link` |
| `http-equiv` | `meta` |
| `id` | HTML elements |
| `imagesizes` | `link` |
| `imagesrcset` | `link` |
| `inert` | HTML elements |
| `inputmode` | HTML elements |
| `integrity` | `link`, `script` |
| `is` | HTML elements |
| `ismap` | `img` |
| `itemid` | HTML elements |
| `itemprop` | HTML elements |
| `itemref` | HTML elements |
| `itemscope` | HTML elements |
| `itemtype` | HTML elements |
| `kind` | `track` |
| `label` | `optgroup`, `option`, `track` |
| `lang` | HTML elements |
| `list` | `input` |
| `loading` | `iframe`, `img` |
| `loop` | `audio`, `video` |
| `low` | `meter` |
| `max` | `input` |
| `max` | `meter`, `progress` |
| `maxlength` | `input`, `textarea` |
| `media` | `link`, `meta`, `source`, `style` |
| `method` | `form` |
| `min` | `input` |
| `min` | `meter` |
| `minlength` | `input`, `textarea` |
| `multiple` | `input`, `select` |
| `muted` | `audio`, `video` |
| `name` | `button`, `fieldset`, `input`, `output`, `select`, `textarea`, form-associated custom elements |
| `name` | `details` |
| `name` | `form` |
| `name` | `iframe`, `object` |
| `name` | `map` |
| `name` | `meta` |
| `name` | `slot` |
| `nomodule` | `script` |
| `nonce` | HTML elements |
| `novalidate` | `form` |
| `onafterprint` | `body` |
| `onauxclick` | HTML elements |
| `onbeforematch` | HTML elements |
| `onbeforeprint` | `body` |
| `onbeforeunload` | `body` |
| `onbeforetoggle` | HTML elements |
| `onblur` | HTML elements |
| `oncancel` | HTML elements |
| `oncanplay` | HTML elements |
| `oncanplaythrough` | HTML elements |
| `onchange` | HTML elements |
| `onclick` | HTML elements |
| `onclose` | HTML elements |
| `oncontextlost` | HTML elements |
| `oncontextmenu` | HTML elements |
| `oncontextrestored` | HTML elements |
| `oncopy` | HTML elements |
| `oncuechange` | HTML elements |
| `oncut` | HTML elements |
| `ondblclick` | HTML elements |
| `ondrag` | HTML elements |
| `ondragend` | HTML elements |
| `ondragenter` | HTML elements |
| `ondragleave` | HTML elements |
| `ondragover` | HTML elements |
| `ondragstart` | HTML elements |
| `ondrop` | HTML elements |
| `ondurationchange` | HTML elements |
| `onemptied` | HTML elements |
| `onended` | HTML elements |
| `onerror` | HTML elements |
| `onfocus` | HTML elements |
| `onformdata` | HTML elements |
| `onhashchange` | `body` |
| `oninput` | HTML elements |
| `oninvalid` | HTML elements |
| `onkeydown` | HTML elements |
| `onkeypress` | HTML elements |
| `onkeyup` | HTML elements |
| `onlanguagechange` | `body` |
| `onload` | HTML elements |
| `onloadeddata` | HTML elements |
| `onloadedmetadata` | HTML elements |
| `onloadstart` | HTML elements |
| `onmessage` | `body` |
| `onmessageerror` | `body` |
| `onmousedown` | HTML elements |
| `onmouseenter` | HTML elements |
| `onmouseleave` | HTML elements |
| `onmousemove` | HTML elements |
| `onmouseout` | HTML elements |
| `onmouseover` | HTML elements |
| `onmouseup` | HTML elements |
| `onoffline` | `body` |
| `ononline` | `body` |
| `onpageswap` | `body` |
| `onpagehide` | `body` |
| `onpagereveal` | `body` |
| `onpageshow` | `body` |
| `onpaste` | HTML elements |
| `onpause` | HTML elements |
| `onplay` | HTML elements |
| `onplaying` | HTML elements |
| `onpopstate` | `body` |
| `onprogress` | HTML elements |
| `onratechange` | HTML elements |
| `onreset` | HTML elements |
| `onresize` | HTML elements |
| `onrejectionhandled` | `body` |
| `onscroll` | HTML elements |
| `onscrollend` | HTML elements |
| `onsecuritypolicyviolation` | HTML elements |
| `onseeked` | HTML elements |
| `onseeking` | HTML elements |
| `onselect` | HTML elements |
| `onslotchange` | HTML elements |
| `onstalled` | HTML elements |
| `onstorage` | `body` |
| `onsubmit` | HTML elements |
| `onsuspend` | HTML elements |
| `ontimeupdate` | HTML elements |
| `ontoggle` | HTML elements |
| `onunhandledrejection` | `body` |
| `onunload` | `body` |
| `onvolumechange` | HTML elements |
| `onwaiting` | HTML elements |
| `onwheel` | HTML elements |
| `open` | `details` |
| `open` | `dialog` |
| `optimum` | `meter` |
| `pattern` | `input` |
| `ping` | `a`, `area` |
| `placeholder` | `input`, `textarea` |
| `playsinline` | `video` |
| `popover` | HTML elements |
| `popovertarget` | `button`, `input` |
| `popovertargetaction` | `button`, `input` |
| `poster` | `video` |
| `preload` | `audio`, `video` |
| `readonly` | `input`, `textarea` |
| `readonly` | form-associated custom elements |
| `referrerpolicy` | `a`, `area`, `iframe`, `img`, `link`, `script` |
| `rel` | `a`, `area` |
| `rel` | `link` |
| `required` | `input`, `select`, `textarea` |
| `reversed` | `ol` |
| `rows` | `textarea` |
| `rowspan` | `td`, `th` |
| `sandbox` | `iframe` |
| `scope` | `th` |
| `selected` | `option` |
| `shadowrootmode` | `template` |
| `shadowrootdelegatesfocus` | `template` |
| `shadowrootclonable` | `template` |
| `shadowrootserializable` | `template` |
| `shape` | `area` |
| `size` | `input`, `select` |
| `sizes` | `link` |
| `sizes` | `img`, `source` |
| `slot` | HTML elements |
| `span` | `col`, `colgroup` |
| `spellcheck` | HTML elements |
| `src` | `audio`, `embed`, `iframe`, `img`, `input`, `script`, `source` (`audio` and `video`), `track`, `video` |
| `srcdoc` | `iframe` |
| `srclang` | `track` |
| `srcset` | `img`, `source` |
| `start` | `ol` |
| `step` | `input` |
| `style` | HTML elements |
| `tabindex` | HTML elements |
| `target` | `a`, `area` |
| `target` | `base` |
| `target` | `form` |
| `title` | HTML elements |
| `title` | `abbr`, `dfn` |
| `title` | `input` |
| `title` | `link` |
| `title` | `link`, `style` |
| `translate` | HTML elements |
| `type` | `a`, `link` |
| `type` | `button` |
| `type` | `embed`, `object`, `source` |
| `type` | `input` |
| `type` | `ol` |
| `type` | `script` |
| `usemap` | `img` |
| `value` | `button`, `option` |
| `value` | `data` |
| `value` | `input` |
| `value` | `li` |
| `value` | `meter`, `progress` |
| `width` | `canvas`, `embed`, `iframe`, `img`, `input`, `object`, `source` (`picture`), `video` |
| `wrap` | `textarea` |
| `writingsuggestions` | HTML elements |

### Global Attributes

Memorize specifically those attributes that can be used on all HTML elements, now _excluding_ event handler attributes. <!-- 97: the 25 “main” ones as per https://html.spec.whatwg.org/multipage/dom.html#global-attributes, the 3 attributes `class`, `id`, and `slot`, and 69 event handler attributes [70/98 with `onbeforeinput`, https://github.com/whatwg/html/issues/10414] -->

* `accesskey`
* `autocapitalize`
* `autofocus`
* `class`
* `contenteditable`
* `dir`
* `draggable`
* `enterkeyhint`
* `hidden`
* `id`
* `inert`
* `inputmode`
* `is`
* `itemid`
* `itemprop`
* `itemref`
* `itemscope`
* `itemtype`
* `lang`
* `nonce`
* `popover`
* `slot`
* `spellcheck`
* `style`
* `tabindex`
* `title`
* `translate`
* `writingsuggestions`

I> Remember to whenever you have a question about HTML, to consult [the HTML specification](https://html.spec.whatwg.org/multipage/).

## Elements With Their Attributes

@@