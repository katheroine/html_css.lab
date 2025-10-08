# HTML elements: Text content

## Paragraph

### Documentation

|Website  |URL                                                                   |
|---------|----------------------------------------------------------------------|
|W3CSchool|https://www.w3schools.com/tags/tag_p.asp                              |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/p|

### Tag

```html
<p></p>
```

### Description

Text paragraph.

**Type**: Block

Paragraphs are usually represented in visual media as blocks of text separated from adjacent blocks by blank lines and/or first-line indentation, but HTML paragraphs can be any structural grouping of related content, such as images or form fields.

Browsers automatically add a single blank line before and after each paragraph element.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
<p>Some paragraph.</p>
```

**Samples**:
* [Basic](../../../samples/elements/p/p.html)

## Block quotation

### Documentation

|Website  |URL                                                                            |
|---------|-------------------------------------------------------------------------------|
|W3CSchool|https://www.w3schools.com/tags/tag_blockquote.asp                              |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/blockquote|

### Tag

```html
<blockquote></blockquote>
```

### Description

A block quotation from another source.

**Type**: Block

The block quotation element indicates that the enclosed text is an extended quotation. Usually, this is rendered visually by indentation (see Notes for how to change it).

Browsers usually indent block quote elements.

### Attributes

#### `cite`

**Value**: URL (relative or absolute)

**Description**: Specifies the source of the quotation

**Example**:

```html
<blockquote cite="URL"></blockquote>
```

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
* [With **`p`** element](../../../samples/elements/blockquote/blockquote.element_p.html)

### Relatives

* A [**p**](#paragraph) elements can be nested inside the blockquote element to organise text and split it into graphically separated blocks.
* An [**quote**](#quote) element can be used for inline (short) quotations.
* A URL for the source of the quotation may be given using the `cite` attribute, while a text representation of the source can be given using the [**citation**](#citation) element.
