# HTML elements: Text items

## Italic

### Documentation

|Website  |URL                                                                           |
|---------|------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-i-element|
|W3CSchool|https://www.w3schools.com/tags/tag_i.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/i        |

### Tag

```html
<i></i>
```

### Description

Voice or mood, text of different quality than normal prose.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `i` element represents a span of text in an *alternate voice or mood*, or otherwise offset from the normal prose in a manner indicating a different quality of text for readability reasons. This would be a range of text with different semantic meaning than the surrounding text.

The content inside is typically displayed in italic.

#### Use cases

* *Alternative voice or mood*
* *Taxonomic designations* (such as the genus and species "Homo sapiens")
* *Idiomatic terms from another language* (such as "et cetera"); these should include the lang attribute to identify the language
* *Technical terms*
* *Transliterations*
* *Thoughts* (such as "She wondered, What is this writer talking about, anyway?")
* *Ship or vessel names* in Western writing systems (such as "They searched the docks for the Empress of the Galaxy, the ship to which they were assigned.")

#### History

In earlier versions of the HTML specification, the `i` element was merely a presentational element used to display text in italics, much like the `b` element was used to display text in bold letters. This is no longer true, as these tags now define semantics rather than typographic appearance. A browser will typically still display the contents of the `i` element in italic type, but is, by definition, no longer required to do so.

### Attributes

Authors can use the `class` attribute on the `i` element to identify *why* the element is being used, so that if the style of a particular use (e.g. dream sequences as opposed to taxonomic terms) is to be changed at a later date, the author doesn't have to go through the entire document (or series of related documents) annotating each use.

Terms in languages different from the main text should be annotated with `lang` attributes (or, in XML, `lang` attributes in the XML namespace).

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
Using the right <i>tone of the voice</i> is important in the communication process.
```

**Samples**:
* [Basic](../../../samples/elements/i/i.html)

### Related elements

* Use [**`em`**](#emphasis) to indicate stress emphasis.
* Use [**`strong`**](#strong) to indicate importance, seriousness, or urgency.
* Use [**`mark`**](#mark) to indicate relevance.
* Use [**`cite`**](#citation) to mark up the name of a work, such as a book, play, or song.
* Use [**`dfn`**](#definition) to mark up the defining instance of a term.

## Bold

### Documentation

|Website  |URL                                                                           |
|---------|------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-b-element|
|W3CSchool|https://www.w3schools.com/tags/tag_b.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/b        |

### Tag

```html
<b></b>
```

### Description

Text to which attention is being drawn without any extra importance.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `b` element represents a span of text used to draw the reader's attention to the element's contents, which are not otherwise granted special importance and with no implication of an alternate voice or mood, such as *key words* in a document abstract, *product names* in a review, *actionable words* in interactive text-driven software, or an article lede.

The `b` element should be used as a last resort when no other element is more appropriate.

You should not use `b` for styling text or granting importance. If you wish to create boldface text, you should use the CSS `font-weight` property.

#### Use cases

* *Keywords* in a summary
* *Product names* in a review
* Other spans of text whose typical presentation would be boldfaced (but not including any special importance)

#### History

Historically, the `b` element was meant to make text boldface. Styling information has been deprecated since HTML4, so the meaning of the `b` element has been changed.

### Attributes

Authors can use the `class` attribute on the `b` element to identify why the element is being used, so that if the style of a particular use is to be changed at a later date, the author doesn't have to go through annotating each use.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
<b>HTML</b> is a hypertext markup language.
```

**Samples**:
* [Basic](../../../samples/elements/b/b.html)

### Related elements

* Headings should use the [**`h1`**]() to [**`h6`**]() elements.
* Stress emphasis should use the [**`em`**](#emphasis) element.
* Importance should be denoted with the [**`strong`**](#strong) element.
* Text marked or highlighted should use the [**`mark`**](#mark) element.

## Unarticulated

### Documentation

|Website  |URL                                                                           |
|---------|------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-u-element|
|W3CSchool|https://www.w3schools.com/tags/tag_u.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/u        |

### Tag

```html
<u></u>
```

### Description

Unarticulated annotation.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `u` element represents a span of text with an unarticulatedand styled differently from normal text, such as misspelled words or proper names in Chinese text (a Chinese proper name mark), or labeling the text as being misspelt.

The content inside is typically displayed with an underline.

You should not use `u` to underline text for presentation purposes, or to denote titles of books.

Avoid using the `u` element where it could be confused for a hyperlink!

To apply an underlined appearance without any semantic meaning, use the text-decoration property's value underline.

#### Use cases

* Annotating spelling errors
* A proper name mark to denote proper names in Chinese text
* Other forms of annotation

#### History

Along with other pure styling elements, the original HTML Underline `u` element was deprecated in HTML 4. However, `u` was restored in HTML 5 with a new, semantic, meaning: to mark text as having some form of non-textual annotation applied.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
Watch out to not write it <u>envinorment</u>.
```

**Samples**:
* [Basic](../../../samples/elements/u/u.html)

### Related elements

* Use [**`em`**](#emphasis) to denote stress emphasis.
* Use [**`b`**](#bold) to draw attention to text.
* Use [**`mark`**](#mark) to mark key words or phrases.
* Use [**`strong`**](#strong) to indicate that text has strong importance.
* Use [**`cite`**](#citation) to mark the titles of books or other publications.
* Use [**`i`**](#italic) to denote technical terms, transliterations, thoughts, or names of vessels in Western texts.
* Use [**`ruby`**](#ruby) to provide textual annotations (as opposed to the non-textual annotations created with `u`).

## Strikethrough

### Documentation

|Website  |URL                                                                           |
|---------|------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-s-element|
|W3CSchool|https://www.w3schools.com/tags/tag_s.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/s        |

### Tag

```html
<s></s>
```

### Description

Contents that are no longer accurate or no longer relevant.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `s` element represents contents that are no longer correct, accurate or no longer relevant.

The `s` HTML element renders text with a strikethrough, or a line through it.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Accessibility

The presence of the s element is not announced by most screen reading technology in its default configuration. It can be made to be announced by using the CSS content property, along with the `::before` and `::after` pseudo-elements.

Some people who use screen readers deliberately disable announcing content that creates extra verbosity. Because of this, it is important to not abuse this technique and only apply it in situations where not knowing content has been struck out would adversely affect understanding.

### Examples

```html
The price is only <s>$3.99</s> $2.99!
```

**Samples**:
* [Basic](../../../samples/elements/s/s.html)

### Related elements

* Use [**`del`**](#del) and [**`ins`**](#ins) elements when indicating document edits.

## Emphasis

### Documentation

|Website  |URL                                                                            |
|---------|-------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-em-element|
|W3CSchool|https://www.w3schools.com/tags/tag_em.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/em        |

### Tag

```html
<em></em>
```

### Description

Stress emphasis.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `em` element represents stress emphasis of its contents. The `em` element is for words that have a stressed emphasis compared to surrounding text, which is often limited to a word or words of a sentence and affects the meaning of the sentence itself.

The `em` element can be nested, with each level of nesting indicating a greater degree of emphasis.

The placement of stress emphasis changes the meaning of the sentence. The element thus forms an integral part of the content. The precise way in which stress is used in this way depends on the language.

The `em` element isn't a generic "italics" element. Sometimes, text is intended to stand out from the rest of the paragraph, as if it was in a different mood or voice. For this, the i element is more appropriate.

The em element also isn't intended to convey importance; for that purpose, the strong element is more appropriate.

The content inside is typically displayed in italic.

It should not be used to apply italic styling; use the CSS font-style property for that purpose.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

# Accessibility

A screen reader will pronounce the words in `em` with an emphasis, using verbal stress.

### Examples

```html
I learnt it all <em>by myself</em>!
```

**Samples**:
* [Basic](../../../samples/elements/em/em.html)

### Related elements

* Use the [**`cite`**] element to mark the title of a work (book, play, song, etc.).
* Use the [**`i`**] element to mark text that is in an alternate tone or mood, which covers many common situations for italics such as scientific names or words in other languages.
* Use the [**`strong`**] element to mark text that has greater importance than surrounding text.

**`i` vs. `em`**

Some developers may be confused by how multiple elements seemingly produce similar visual results. `em` and `i` are a common example, since they both italicize text.

By default, the visual result is the same. However, the semantic meaning is different. The `em` element represents *stress emphasis of its contents*, while the `i` element represents *text that is set off from the normal prose*, such as a foreign word, fictional character thoughts, or when the text refers to the definition of a word instead of representing its semantic meaning.
