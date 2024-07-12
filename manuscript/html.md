# HTML {#toc-html}

This section covers HTML as per [the living standard](https://html.spec.whatwg.org/multipage/) in <!-- @@ -->July 2024. Elements from earlier HTML specifications and proprietary elements are not included.

## Elements

### Element Meanings

Memorize the elements and their meanings (semantics), to know what elements there are and what purposes they serve.

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
* `h1`: Heading, level 1
* `h2`: Heading, level 2
* `h3`: Heading, level 3
* `h4`: Heading, level 4
* `h5`: Heading, level 5
* `h6`: Heading, level 6
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

### Void Elements

Memorize the void elements, i.e., elements that have no end tag in the HTML syntax:

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

I> In HTML (i.e., in HTML not following an XML syntax), you write these elements as `<elementname>`, like `<area>`, `<img>`, or `<meta>`. There’s no end tag and no slash.

### Elements With Optional Start or End Tags

Memorize the elements with optional start and end tags, to be able to omit them, should you choose to use this feature of HTML. Void elements don’t have an end tag and are therefore included (but also called out) as well.

| Element | Void? | Optional Start Tag? | Optional End Tag? |
| --- | --- | --- | --- |
| `area` | yes | no | yes (void) |
| `base` | yes | no | yes (void) |
| `body` | no | yes | yes |
| `br` | yes | no | yes (void) |
| `caption` | no | no | yes |
| `col` | yes | no | yes (void) |
| `colgroup` | no | yes | yes |
| `dd` | no | no | yes |
| `dt` | no | no | yes |
| `embed` | yes | no | yes (void) |
| `figcaption` | no | no | yes |
| `head` | no | yes | yes |
| `hr` | yes | no | yes (void) |
| `html` | no | yes | yes |
| `img` | yes | no | yes (void) |
| `input` | yes | no | yes (void) |
| `li` | no | no | yes |
| `link` | yes | no | yes (void) |
| `meta` | yes | no | yes (void) |
| `optgroup` | no | no | yes |
| `option` | no | no | yes |
| `p` | no | no | yes |
| `rp` | no | no | yes |
| `rt` | no | no | yes |
| `source` | yes | no | yes (void) |
| `tbody` | no | yes | yes |
| `td` | no | no | yes |
| `tfoot` | no | no | yes |
| `th` | no | no | yes |
| `thead` | no | no | yes |
| `tr` | no | no | yes |
| `track` | yes | no | yes (void) |
| `wbr` | yes | no | yes (void) |

### Element Categories

Memorize the HTML content categories, to maximize opportunities to use the respective elements correctly.

#### Metadata Content

Metadata content sets up the presentation or behavior of the rest of a document’s content, establishes a document’s relationship with other documents, or conveys other information.

* `base`
* `link`
* `meta`
* `noscript`
* `script`
* `style`
* `template`
* `title`

#### Flow Content

Flow content makes for the `body` of a document.

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
* Autonomous custom elements
* Text

Elements that can be flow content under certain circumstances:

* `area`
* `link`
* `main`
* `meta`

#### Sectioning Content

Sectioning content defines document sections, and thus the scope of `header` and `footer` elements.

* `article`
* `aside`
* `nav`
* `section`

#### Heading Content

Heading content defines the respective heading of a section.

* `h1`
* `h2`
* `h3`
* `h4`
* `h5`
* `h6`
* `hgroup`

#### Phrasing Content

Phrasing content represents the text of a document.

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
* Autonomous custom elements
* Text

Elements that can be phrasing content under certain circumstances:

* `area`
* `link`
* `meta`

#### Palpable Content

Palpable content makes an element non-empty by providing non-empty text or something a user can perceive or interact with.

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
* Autonomous custom elements

Elements that can be palpable content under certain circumstances:

* `audio`
* `dl`
* `input`
* `menu`
* `ol`
* `ul`
* Text that isn’t whitespace between elements

#### Embedded Content

Embedded content imports other resources and content into a document.

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

Interactive content serves user interaction.

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

Form-associated elements are elements that have a form owner.

* `button`
* `fieldset`
* `input`
* `label`
* `object`
* `output`
* `select`
* `textarea`
* `img`
* Form-associated custom elements

#### Labelable Elements

Labelable elements are elements that can be associated with a `label` element.

* `button`
* `input`
* `meter`
* `output`
* `progress`
* `select`
* `textarea`
* Form-associated custom elements

#### Listed Elements

Listed elements are listed in the `form.elements` and `fieldset.elements` APIs.

* `button`
* `fieldset`
* `input`
* `object`
* `output`
* `select`
* `textarea`
* Form-associated custom elements

#### Submittable Elements

Submittable elements may be used to construct the respective entry list when a `form` element is being submitted.

* `button`
* `input`
* `select`
* `textarea`
* Form-associated custom elements

#### Resettable Elements

Resettable elements may be affected when a `form` element is being reset.

* `input`
* `output`
* `select`
* `textarea`
* Form-associated custom elements

#### Autocapitalize-Inheriting Elements

Autocapitalize-inheriting elements inherit the `autocapitalize` attribute from their form owner.

* `button`
* `fieldset`
* `input`
* `output`
* `select`
* `textarea`

#### Script-Supporting Elements

Script-supporting elements do not represent anything by themselves, but provide functionality.

* `script`
* `template`

## Attributes

Memorize all attributes, to be aware of their existence and to develop a sense for what options HTML provides out of the box. (“HTML elements” refers to any element in the “http://www.w3.org/1999/xhtml” namespace—including, as per the specification, XML documents.)

| Attributes | Elements |
| --- | --- |
| `abbr` | `th` |
| `accept` | `input` |
| `accept-charset` | `form` |
| `accesskey` | all HTML elements |
| `action` | `form` |
| `allow` | `iframe` |
| `allowfullscreen` | `iframe` |
| `alt` | `area`, `img`, `input` |
| `as` | `link` |
| `async` | `script` |
| `autocapitalize` | all HTML elements |
| `autocomplete` | `form`, `input`, `select`, `textarea` |
| `autofocus` | all HTML elements |
| `autoplay` | `audio`, `video` |
| `blocking` | `link`, `script`, `style` |
| `charset` | `meta` |
| `checked` | `input` |
| `cite` | `blockquote`, `del`, `ins`, `q` |
| `class` | all HTML elements |
| `color` | `link` |
| `cols` | `textarea` |
| `colspan` | `td`, `th` |
| `content` | `meta` |
| `contenteditable` | all HTML elements |
| `controls` | `audio`, `video` |
| `coords` | `area` |
| `crossorigin` | `audio`, `img`, `link`, `script`, `video` |
| `data` | `object` |
| `datetime` | `del`, `ins`, `time` |
| `decoding` | `img` |
| `default` | `track` |
| `defer` | `script` |
| `dir` | all HTML elements |
| `dirname` | `input`, `textarea` |
| `disabled` | `button`, `fieldset`, `input`, `link`, `optgroup`, `option`, `select`, `textarea`, form-associated custom elements |
| `download` | `a`, `area` |
| `draggable` | all HTML elements |
| `enctype` | `form` |
| `enterkeyhint` | all HTML elements |
| `fetchpriority` | `img`, `link`, `script` |
| `for` | `label`, `output` |
| `form` | `button`, `fieldset`, `input`, `object`, `output`, `select`, `textarea`, form-associated custom elements |
| `formaction` | `button`, `input` |
| `formenctype` | `button`, `input` |
| `formmethod` | `button`, `input` |
| `formnovalidate` | `button`, `input` |
| `formtarget` | `button`, `input` |
| `headers` | `td`, `th` |
| `height` | `canvas`, `embed`, `iframe`, `img`, `input`, `object`, `source` (`picture`), `video` |
| `hidden` | all HTML elements |
| `high` | `meter` |
| `href` | `a`, `area`, `base`, `link` |
| `hreflang` | `a`, `link` |
| `http-equiv` | `meta` |
| `id` | all HTML elements |
| `imagesizes` | `link` |
| `imagesrcset` | `link` |
| `inert` | all HTML elements |
| `inputmode` | all HTML elements |
| `integrity` | `link`, `script` |
| `is` | all HTML elements |
| `ismap` | `img` |
| `itemid` | all HTML elements |
| `itemprop` | all HTML elements |
| `itemref` | all HTML elements |
| `itemscope` | all HTML elements |
| `itemtype` | all HTML elements |
| `kind` | `track` |
| `label` | `optgroup`, `option`, `track` |
| `lang` | all HTML elements |
| `list` | `input` |
| `loading` | `iframe`, `img` |
| `loop` | `audio`, `video` |
| `low` | `meter` |
| `max` | `input`, `meter`, `progress` |
| `maxlength` | `input`, `textarea` |
| `media` | `link`, `meta`, `source`, `style` |
| `method` | `form` |
| `min` | `input`, `meter` |
| `minlength` | `input`, `textarea` |
| `multiple` | `input`, `select` |
| `muted` | `audio`, `video` |
| `name` | `button`, `details`, `fieldset`, `form`, `iframe`, `input`, `map`, `meta`, `object`, `output`, `select`, `slot`, `textarea`, form-associated custom elements |
| `nomodule` | `script` |
| `nonce` | all HTML elements |
| `novalidate` | `form` |
| `onafterprint` | `body` |
| `onauxclick` | all HTML elements |
| `onbeforeinput` | all HTML elements |
| `onbeforematch` | all HTML elements |
| `onbeforeprint` | `body` |
| `onbeforeunload` | `body` |
| `onbeforetoggle` | all HTML elements |
| `onblur` | all HTML elements |
| `oncancel` | all HTML elements |
| `oncanplay` | all HTML elements |
| `oncanplaythrough` | all HTML elements |
| `onchange` | all HTML elements |
| `onclick` | all HTML elements |
| `onclose` | all HTML elements |
| `oncontextlost` | all HTML elements |
| `oncontextmenu` | all HTML elements |
| `oncontextrestored` | all HTML elements |
| `oncopy` | all HTML elements |
| `oncuechange` | all HTML elements |
| `oncut` | all HTML elements |
| `ondblclick` | all HTML elements |
| `ondrag` | all HTML elements |
| `ondragend` | all HTML elements |
| `ondragenter` | all HTML elements |
| `ondragleave` | all HTML elements |
| `ondragover` | all HTML elements |
| `ondragstart` | all HTML elements |
| `ondrop` | all HTML elements |
| `ondurationchange` | all HTML elements |
| `onemptied` | all HTML elements |
| `onended` | all HTML elements |
| `onerror` | all HTML elements |
| `onfocus` | all HTML elements |
| `onformdata` | all HTML elements |
| `onhashchange` | `body` |
| `oninput` | all HTML elements |
| `oninvalid` | all HTML elements |
| `onkeydown` | all HTML elements |
| `onkeypress` | all HTML elements |
| `onkeyup` | all HTML elements |
| `onlanguagechange` | `body` |
| `onload` | all HTML elements |
| `onloadeddata` | all HTML elements |
| `onloadedmetadata` | all HTML elements |
| `onloadstart` | all HTML elements |
| `onmessage` | `body` |
| `onmessageerror` | `body` |
| `onmousedown` | all HTML elements |
| `onmouseenter` | all HTML elements |
| `onmouseleave` | all HTML elements |
| `onmousemove` | all HTML elements |
| `onmouseout` | all HTML elements |
| `onmouseover` | all HTML elements |
| `onmouseup` | all HTML elements |
| `onoffline` | `body` |
| `ononline` | `body` |
| `onpagehide` | `body` |
| `onpagereveal` | `body` |
| `onpageshow` | `body` |
| `onpageswap` | `body` |
| `onpaste` | all HTML elements |
| `onpause` | all HTML elements |
| `onplay` | all HTML elements |
| `onplaying` | all HTML elements |
| `onpopstate` | `body` |
| `onprogress` | all HTML elements |
| `onratechange` | all HTML elements |
| `onreset` | all HTML elements |
| `onresize` | all HTML elements |
| `onrejectionhandled` | `body` |
| `onscroll` | all HTML elements |
| `onscrollend` | all HTML elements |
| `onsecuritypolicy violation` | all HTML elements |
| `onseeked` | all HTML elements |
| `onseeking` | all HTML elements |
| `onselect` | all HTML elements |
| `onslotchange` | all HTML elements |
| `onstalled` | all HTML elements |
| `onstorage` | `body` |
| `onsubmit` | all HTML elements |
| `onsuspend` | all HTML elements |
| `ontimeupdate` | all HTML elements |
| `ontoggle` | all HTML elements |
| `onunhandledrejection` | `body` |
| `onunload` | `body` |
| `onvolumechange` | all HTML elements |
| `onwaiting` | all HTML elements |
| `onwheel` | all HTML elements |
| `open` | `details`, `dialog` |
| `optimum` | `meter` |
| `pattern` | `input` |
| `ping` | `a`, `area` |
| `placeholder` | `input`, `textarea` |
| `playsinline` | `video` |
| `popover` | all HTML elements |
| `popovertarget` | `button`, `input` |
| `popovertargetaction` | `button`, `input` |
| `poster` | `video` |
| `preload` | `audio`, `video` |
| `readonly` | `input`, `textarea`, form-associated custom elements |
| `referrerpolicy` | `a`, `area`, `iframe`, `img`, `link`, `script` |
| `rel` | `a`, `area`, `link` |
| `required` | `input`, `select`, `textarea` |
| `reversed` | `ol` |
| `rows` | `textarea` |
| `rowspan` | `td`, `th` |
| `sandbox` | `iframe` |
| `scope` | `th` |
| `selected` | `option` |
| `shadowrootclonable` | `template` |
| `shadowroot delegatesfocus` | `template` |
| `shadowrootmode` | `template` |
| `shadowroot serializable` | `template` |
| `shape` | `area` |
| `size` | `input`, `select` |
| `sizes` | `img`, `link`, `source` |
| `slot` | all HTML elements |
| `span` | `col`, `colgroup` |
| `spellcheck` | all HTML elements |
| `src` | `audio`, `embed`, `iframe`, `img`, `input`, `script`, `source` (`audio` and `video`), `track`, `video` |
| `srcdoc` | `iframe` |
| `srclang` | `track` |
| `srcset` | `img`, `source` |
| `start` | `ol` |
| `step` | `input` |
| `style` | all HTML elements |
| `tabindex` | all HTML elements |
| `target` | `a`, `area`, `base`, `form` |
| `title` | all HTML elements |
| `translate` | all HTML elements |
| `type` | `a`, `button`, `embed`, `input`, `link`, `object`, `ol`, `script`, `source` |
| `usemap` | `img` |
| `value` | `button`, `data`, `input`, `li`, `meter`, `option`, `progress` |
| `width` | `canvas`, `embed`, `iframe`, `img`, `input`, `object`, `source` (`picture`), `video` |
| `wrap` | `textarea` |
| `writingsuggestions` | all HTML elements |

### Global Attributes

#### …Excluding Event Handler Attributes

Memorize the attributes that can be used on all HTML elements (not including event handler attributes), to know what attributes you can use anywhere.

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

#### …Including Event Handler Attributes

Memorize the attributes that can be used on all HTML elements, including event handler attributes. <!-- 98: the 25 “main” ones as per https://html.spec.whatwg.org/multipage/dom.html#global-attributes, the 3 attributes `class`, `id`, and `slot`, and 70 event handler attributes -->

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
* `onauxclick`
* `onbeforeinput`
* `onbeforematch`
* `onbeforetoggle`
* `onblur`
* `oncancel`
* `oncanplay`
* `oncanplaythrough`
* `onchange`
* `onclick`
* `onclose`
* `oncontextlost`
* `oncontextmenu`
* `oncontextrestored`
* `oncopy`
* `oncuechange`
* `oncut`
* `ondblclick`
* `ondrag`
* `ondragend`
* `ondragenter`
* `ondragleave`
* `ondragover`
* `ondragstart`
* `ondrop`
* `ondurationchange`
* `onemptied`
* `onended`
* `onerror`
* `onfocus`
* `onformdata`
* `oninput`
* `oninvalid`
* `onkeydown`
* `onkeypress`
* `onkeyup`
* `onload`
* `onloadeddata`
* `onloadedmetadata`
* `onloadstart`
* `onmousedown`
* `onmouseenter`
* `onmouseleave`
* `onmousemove`
* `onmouseout`
* `onmouseover`
* `onmouseup`
* `onpaste`
* `onpause`
* `onplay`
* `onplaying`
* `onprogress`
* `onratechange`
* `onreset`
* `onresize`
* `onscroll`
* `onscrollend`
* `onsecuritypolicyviolation`
* `onseeked`
* `onseeking`
* `onselect`
* `onslotchange`
* `onstalled`
* `onsubmit`
* `onsuspend`
* `ontimeupdate`
* `ontoggle`
* `onvolumechange`
* `onwaiting`
* `onwheel`
* `popover`
* `slot`
* `spellcheck`
* `style`
* `tabindex`
* `title`
* `translate`
* `writingsuggestions`

## Elements With Their Attributes

Go over all elements and their attributes, to extend your understanding of HTML semantics and features. Global attributes are mentioned, but not listed individually.

| Elements | Attributes |
| --- | --- |
| `a` | `download`, `href`, `hreflang`, `ping`, `referrerpolicy`, `rel`, `target`, `type`, global attributes |
| `abbr` | global attributes |
| `address` | global attributes |
| `area` | `alt`, `coords`, `download`, `href`, `ping`, `referrerpolicy`, `rel`, `shape`, `target`, global attributes |
| `article` | global attributes |
| `aside` | global attributes |
| `audio` | `autoplay`, `controls`, `crossorigin`, `loop`, `muted`, `preload`, `src`, global attributes |
| `b` | global attributes |
| `base` | `href`, `target`, global attributes |
| `bdi` | global attributes |
| `bdo` | global attributes |
| `blockquote` | `cite`, global attributes |
| `body` | `onafterprint`, `onbeforeprint`, `onbeforeunload`, `onhashchange`, `onlanguagechange`, `onmessage`, `onmessageerror`, `onoffline`, `ononline`, `onpagehide`, `onpagereveal`, `onpageshow`, `onpageswap`, `onpopstate`, `onrejectionhandled`, `onstorage`, `onunhandledrejection`, `onunload`, global attributes |
| `br` | global attributes |
| `button` | `disabled`, `form`, `formaction`, `formenctype`, `formmethod`, `formnovalidate`, `formtarget`, `name`, `popovertarget`, `popovertargetaction`, `type`, `value`, global attributes |
| `canvas` | `height`, `width`, global attributes |
| `caption` | global attributes |
| `cite` | global attributes |
| `code` | global attributes |
| `col` | `span`, global attributes |
| `colgroup` | `span`, global attributes |
| `data` | `value`, global attributes |
| `datalist` | global attributes |
| `dd` | global attributes |
| `del` | `cite`, `datetime`, global attributes |
| `details` | `name`, `open`, global attributes |
| `dfn` | global attributes |
| `dialog` | `open`, global attributes |
| `div` | global attributes |
| `dl` | global attributes |
| `dt` | global attributes |
| `em` | global attributes |
| `embed` | `height`, `src`, `type`, `width`, global attributes |
| `fieldset` | `disabled`, `form`, `name`, global attributes |
| `figcaption` | global attributes |
| `figure` | global attributes |
| `footer` | global attributes |
| `form` | `accept-charset`, `action`, `autocomplete`, `enctype`, `method`, `name`, `novalidate`, `rel`, `target`, global attributes |
| `h1` | global attributes |
| `h2` | global attributes |
| `h3` | global attributes |
| `h4` | global attributes |
| `h5` | global attributes |
| `h6` | global attributes |
| `head` | global attributes |
| `header` | global attributes |
| `hgroup` | global attributes |
| `hr` | global attributes |
| `html` | `manifest`, global attributes |
| `i` | global attributes |
| `iframe` | `allow`, `allowfullscreen`, `height`, `loading`, `name`, `referrerpolicy`, `sandbox`, `src`, `srcdoc`, `width`, global attributes |
| `img` | `alt`, `crossorigin`, `decoding`, `fetchpriority`, `height`, `ismap`, `loading`, `referrerpolicy`, `src`, `srcset`, `sizes`, `usemap`, `width`, global attributes |
| `input` | `accept`, `alt`, `autocomplete`, `checked`, `dirname`, `disabled`, `form`, `formaction`, `formenctype`, `formmethod`, `formnovalidate`, `formtarget`, `height`, `list`, `max`, `maxlength`, `min`, `minlength`, `multiple`, `name`, `pattern`, `placeholder`, `popovertarget`, `popovertargetaction`, `readonly`, `required`, `size`, `src`, `step`, `type`, `value`, `width`, global attributes |
| `ins` | `cite`, `datetime`, global attributes |
| `kbd` | global attributes |
| `label` | `for`, global attributes |
| `legend` | global attributes |
| `li` | `value`, global attributes |
| `link` | `as`, `blocking`, `color`, `crossorigin`, `disabled`, `fetchpriority`, `href`, `hreflang`, `imagesizes`, `imagesrcset`, `integrity`, `media`, `referrerpolicy`, `rel`, `sizes`, `type`, global attributes |
| `main` | global attributes |
| `map` | `name`, global attributes |
| `mark` | global attributes |
| `math` | defined by [MathML](https://www.w3.org/TR/mathml-core/) |
| `menu` | global attributes |
| `meta` | `charset`, `content`, `http-equiv`, `media`, `name`, global attributes |
| `meter` | `high`, `low`, `max`, `min`, `optimum`, `value`, global attributes |
| `nav` | global attributes |
| `noscript` | global attributes |
| `object` | `data`, `form`, `height`, `name`, `type`, `width`, global attributes |
| `ol` | `reversed`, `start`, `type`, global attributes |
| `optgroup` | `disabled`, `label`, global attributes |
| `option` | `disabled`, `label`, `selected`, `value`, global attributes |
| `output` | `for`, `form`, `name`, global attributes |
| `p` | global attributes |
| `picture` | global attributes |
| `pre` | global attributes |
| `progress` | `max`, `value`, global attributes |
| `q` | `cite`, global attributes |
| `rp` | global attributes |
| `rt` | global attributes |
| `ruby` | global attributes |
| `s` | global attributes |
| `samp` | global attributes |
| `script` | `async`, `blocking`, `defer`, `crossorigin`, `fetchpriority`, `integrity`, `nomodule`, `referrerpolicy`, `src`, `type`, global attributes |
| `search` | global attributes |
| `section` | global attributes |
| `select` | `autocomplete`, `disabled`, `form`, `multiple`, `name`, `required`, `size`, global attributes |
| `slot` | `name`, global attributes |
| `small` | global attributes |
| `source` | `height`, `media`, `sizes`, `src`, `srcset`, `type`, `width`, global attributes |
| `span` | global attributes |
| `strong` | global attributes |
| `style` | `blocking`, `media`, global attributes |
| `sub` | global attributes |
| `summary` | global attributes |
| `sup` | global attributes |
| `svg` | defined by [SVG](https://www.w3.org/TR/SVG/) |
| `table` | global attributes |
| `tbody` | global attributes |
| `td` | `colspan`, `headers`, `rowspan`, global attributes |
| `template` | `shadowrootclonable`, `shadowrootdelegatesfocus`, `shadowrootmode`, `shadowrootserializable`, global attributes |
| `textarea` | `autocomplete`, `cols`, `dirname`, `disabled`, `form`, `maxlength`, `minlength`, `name`, `placeholder`, `readonly`, `required`, `rows`, `wrap`, global attributes |
| `tfoot` | global attributes |
| `th` | `abbr`, `colspan`, `headers`, `rowspan`, `scope`, global attributes |
| `thead` | global attributes |
| `time` | `datetime`, global attributes |
| `title` | global attributes |
| `tr` | global attributes |
| `track` | `default`, `kind`, `label`, `src`, `srclang`, global attributes |
| `u` | global attributes |
| `ul` | global attributes |
| `var` | global attributes |
| `video` | `autoplay`, `controls`, `crossorigin`, `height`, `loop`, `muted`, `playsinline`, `poster`, `preload`, `src`, `width`, global attributes |
| `wbr` | global attributes |
| autonomous custom elements | global attributes |

I> Whenever you have a question related to HTML, remember to always consult [the HTML specification](https://html.spec.whatwg.org/multipage/) first.