# HTML elements: Text content

## Paragraph

### Documentation

|Website  |URL                                                                       |
|---------|--------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/grouping-content.html#the-p-element|
|W3CSchool|https://www.w3schools.com/tags/tag_p.asp                                  |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/p    |

### Tag

```html
<p></p>
```

### Description

Text paragraph.

**Type**: Block

**Categories**:
* Flow content
* Palpable content

**Contexts in which this element can be used**:
* Where flow content is expected

**Content model**: Phrasing content

Paragraphs are usually represented in visual media as blocks of text separated from adjacent blocks by blank lines and/or first-line indentation, but HTML paragraphs can be any structural grouping of related content, such as images or form fields.

Browsers automatically add a single blank line before and after each paragraph element.

A paragraph, in HTML terms, is not a *logical* concept, but a *structural* one. That's why, the paragraph cannot create nested hierarchies i.e. cannot contain other elements.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
<p>Some paragraph.</p>
```

### Related elements

* The [**`ul`**](#unordered_list), [**`ol`**](#ordered_list) elements cannot be children of **`p`** elements.

**Samples**:
* [Basic](../../../samples/elements/p/p.html)

## Block quotation

### Documentation

|Website  |URL                                                                                |
|---------|-----------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/grouping-content.html#the-blockquote-element|
|W3CSchool|https://www.w3schools.com/tags/tag_blockquote.asp                                  |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/blockquote    |

### Tag

```html
<blockquote></blockquote>
```

### Description

A block quotation from another source.

**Type**: Block

**Categories**:
* Flow content
* Palpable content

**Contexts in which this element can be used**:
* Where flow content is expected

**Content model**: Flow content

The block quotation element indicates that the enclosed text is an extended quotation. Usually, this is rendered visually by indentation (see Notes for how to change it).

Browsers usually indent `blockquote` elements.

The content of a block quotation may be abbreviated or may have context added in the conventional manner for the text's language.

### Attributes

#### `cite`

**Value**: URL (relative or absolute)

**Description**: Specifies the source of the quotation

**Example**:

```html
<blockquote cite="URL"></blockquote>
```

Content inside a block quotation must be quoted from another source, whose address, if it has one, may be cited in the `cite` attribute.

If the `cite` attribute is present, it must be a valid URL potentially surrounded by spaces. To obtain the corresponding citation link, the value of the attribute must be parsed relative to the element's node document. User agents may allow users to follow such citation links, but they are primarily intended for private use (e.g., by server-side scripts collecting statistics about a site's use of quotations), not for readers.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
<blockquote cite="https://github.com/katheroine">I'm Katheroine and this is my code.</blockquote>
```

**Samples**:
* [Basic](../../../samples/elements/blockquote/blockquote.html)
* [With `cite` attribute](../../../samples/elements/blockquote/blockquote.attribute_cite.html)
* [With **`cite`** element](../../../samples/elements/blockquote/blockquote.element_cite.html)
* [With several **`p`** elements](../../../samples/elements/blockquote/blockquote.elements_p.html)
* [With figure **`figure`** and **`figcaption`** elements](../../../samples/elements/blockquote/blockquote.elements_figure_figcaption.html)

### Related elements

* A [**`p`**](#paragraph) elements can be nested inside the blockquote element to organise text and split it into graphically separated blocks.
* An [**`quote`**](#quotation) element can be used for inline (short) quotations.
* A URL for the source of the quotation may be given using the `cite` attribute, while a text representation of the source can be given using the [**`cite`**](#citation) element.
* A `blockquote` element is used in conjunction with a [**`figure`**](#figure) element and its [**`figcaption`**](#figure_caption) to clearly relate a quote to its attribution.
