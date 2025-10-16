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

* Use the [**`em`**](#emphasis) element to denote stress emphasis.
* Use the [**`b`**](#bold) element to draw attention to text.
* Use the [**`mark`**](#mark) element to mark key words or phrases.
* Use the [**`strong`**](#strong) element to indicate that text has strong importance.
* Use the [**`cite`**](#citation) element to mark the titles of books or other publications.
* Use the [**`i`**](#italic) element to denote technical terms, transliterations, thoughts, or names of vessels in Western texts.
* Use the [**`ruby`**](#ruby) element to provide textual annotations (as opposed to the non-textual annotations created with `u`).

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

**`em` vs. `strong`**

Adding to the confusion is the fact that while HTML 4 defined `strong` as indicating a stronger emphasis, HTML 5 defines `strong` as representing "strong importance for its contents." This is an important distinction to make.

While `em` is used to change the meaning of a sentence as spoken emphasis does ("I love carrots" vs. "*I love carrots*"), `strong` is used to give portions of a sentence added importance (e.g., "**Warning! This is very dangerous.**") Both `strong` and `em` can be nested to increase the relative degree of importance or stress emphasis, respectively.

## Strong

### Documentation

|Website  |URL                                                                                |
|---------|-----------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-strong-element|
|W3CSchool|https://www.w3schools.com/tags/tag_strong.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/strong        |

### Tag

```html
<strong></strong>
```

### Description

Strong importance, seriousness, or urgency.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `strong` element represents strong importance, seriousness, or urgency for its contents (such as warnings).

The `strong` element can be nested, with each level of nesting indicating a greater degree of importance.

Changing the importance of a piece of text with the strong element does not change the meaning of the sentence.

The content inside is typically displayed in bold.

### Use cases

* *Importance*: the `strong` element can be used in a heading, caption, or paragraph to distinguish the part that really matters from other parts that might be more detailed, more jovial, or merely boilerplate. (This is distinct from marking up subheadings, for which the `hgroup` element is appropriate.)
* *Seriousness*: the `strong` element can be used to mark up a warning or caution notice. Accepted use for `strong` is to denote the labels of paragraphs which represent notes or warnings within the text of a page.
* *Urgency*: the `strong` element can be used to denote contents that the user needs to see sooner than other parts of the document.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
<strong>Caution! Hot contents.</strong> Use the holder.
```

**Samples**:
* [Basic](../../../samples/elements/strong/strong.html)


### Related elements

* Use the [**`b`**](#bold) element to specify bold text without any extra importance.
* Use the [**`b`**](#bold) element to draw attention to certain text without indicating a higher level of importance.
* Use the [**`em`**](#emphasis) element to mark text that has stress emphasis.
* Use the [**`hgroup`**](#hgroup) element for marking up subheadings.

**`b` vs. `strong`**

It is often confusing to new developers why there are so many ways to express the same thing on a rendered website. `b` and `strong` are perhaps one of the most common sources of confusion.

The `strong` element is for *content that is of greater importance*, while the `b` element is used to *draw attention to text without indicating that it's more important*.

It may help to realize that both are valid and semantic elements in HTML and that it's a coincidence that they both have the same default styling (boldface) in most browsers (although some older browsers actually underline `strong`).

**`em` vs. `strong`**

Adding to the confusion is the fact that while HTML 4 defined `strong` as indicating a stronger emphasis, HTML 5 defines `strong` as representing "strong importance for its contents." This is an important distinction to make.

While `em` is used to change the meaning of a sentence as spoken emphasis does ("I love carrots" vs. "*I love carrots*"), `strong` is used to give portions of a sentence added importance (e.g., "**Warning! This is very dangerous.**") Both `strong` and `em` can be nested to increase the relative degree of importance or stress emphasis, respectively.

## Small

### Documentation

|Website  |URL                                                                               |
|---------|----------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-small-element|
|W3CSchool|https://www.w3schools.com/tags/tag_small.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/small        |

### Tag

```html
<small></small>
```

### Description

Side comments.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `small` element represents side comments such as small print.

Small print typically features *disclaimers*, *caveats*, *legal restrictions*, or *copyrights*. Small print is also sometimes used for *attribution*, or for *satisfying licensing requirements*, independent of its styled presentation.

The `small` element should not be used for extended spans of text, such as multiple paragraphs, lists, or sections of text. It is only intended for short runs of text.

By default, it renders text within it one font-size smaller, such as from small to x-small.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
GitHub is committed to shaping policies that promote programmers' interests and the future of software. <small>(According to github.com)</small>
```

**Samples**:
* [Basic](../../../samples/elements/small/small.html)

### Related elements

* The `small` element does not "de-emphasize" or lower the importance of text emphasized by the [**`em`**](#emphasis) element or marked as important with the [**`strong`**](#strong) element. To mark text as not emphasized or important, simply do not mark it up with the [**`em`**](#emphasis) or [**`strong`**](#strong) elements respectively.
* The small element must not be used for subheadings; for that purpose, use the [**`hgroup`**](#hgroup) element.

## Mark

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-mark-element|
|W3CSchool|https://www.w3schools.com/tags/tag_mark.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/mark        |

### Tag

```html
<mark></mark>
```

### Description

Text marked for reference purposes.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `mark` element represents a run of text in one document marked or highlighted for reference purposes, due to its relevance in another context. When used in a quotation or other block of text referred to from the prose, it indicates a highlight that was not originally present but which has been added to bring the reader's attention to a part of the text that might not have been considered important by the original author when the block was originally written, but which is now under previously unexpected scrutiny. When used in the main prose of a document, it indicates a part of the document that has been highlighted due to its likely relevance to the user's current activity.

### Use cases

* When used in a quotation (`q`) or block quote (`blockquote`), it generally indicates text which is of special interest but is not marked in the original source material, or material which needs special scrutiny even though the original author didn't think it was of particular importance. Think of this like using a highlighter pen in a book to mark passages that you find of interest.
* Otherwise, `mark` indicates a portion of the document's content which is likely to be relevant to the user's current activity. This might be used, for example, to indicate the words that matched a search operation.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Accessibility

The presence of the mark element is not announced by most screen reading technology in its default configuration. It can be made to be announced by using the CSS content property, along with the `::before` and `::after` pseudo-elements.

### Examples

```html
We work every working day for al least <mark>eight hours</mark>.
```

**Samples**:
* [Basic](../../../samples/elements/mark/mark.html)

### Related elements

* Don't use `mark` for syntax highlighting purposes; instead, use the [**`span`**](#span) element with appropriate CSS applied to it.
* Don't confuse `mark` with the [**`strong`**](#strong) element; `mark` is used to denote content which has a degree of relevance, while `strong` indicates spans of text of importance.

## Quotation

### Documentation

|Website  |URL                                                                           |
|---------|------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-q-element|
|W3CSchool|https://www.w3schools.com/tags/tag_q.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/q        |

### Tag

```html
<q></q>
```

### Description

Short quotation.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `q` element represents some phrasing content quoted from another source.

Quotation punctuation (such as quotation marks) that is quoting the contents of the element must not appear immediately before, after, or inside `q` elements; they will be inserted into the rendering by the user agent.

The `q` element must not be used in place of quotation marks that do not represent quotes; for example, it is inappropriate to use the `q` element for marking up sarcastic statements.

The use of `q` elements to mark up quotations is entirely optional; using explicit quotation punctuation without `q` elements is just as correct.

The `q` HTML element indicates that the enclosed text is a short inline quotation and  don't require paragraph breaks.

Browsers normally insert quotation marks around the quotation.

### Attributes

#### `cite`

**Value**: URL (relative or absolute)

**Description**: Specifies the source of the quotation

**Example**:

```html
<q cite="URL"></q>
```

### Attributes

Content inside a `q` element must be quoted from another source, whose address, if it has one, may be cited in the `cite` attribute. The value of this attribute is a URL that designates a source document or message for the information quoted. This attribute is intended to point to information explaining the context or the reference for the quote. The source may be fictional, as when quoting characters in a novel or screenplay.

If the `cite` attribute is present, it must be a valid URL potentially surrounded by spaces. To obtain the corresponding citation link, the value of the attribute must be parsed relative to the element's node document. User agents may allow users to follow such citation links, but they are primarily intended for private use (e.g., by server-side scripts collecting statistics about a site's use of quotations), not for readers.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
He used to say <q>Videmus nunc per speculum et in aenigmate</q>, what was the citation from the Vulgata.
```

**Samples**:
* [Basic](../../../samples/elements/q/q.html)
* [With `cite` attribute](../../../samples/elements/q/q.attribute_cite.html)

### Related elements

* Use [**`blockquote`**](#blockquote) for long quotations.

## Citation

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-cite-element|
|W3CSchool|https://www.w3schools.com/tags/tag_cite.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/cite        |

### Tag

```html
<cite></cite>
```

### Description

Short citation.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `cite` element represents the title of a creative work (e.g. a book, a paper, an essay, a poem, a score, a song, a script, a film, a TV show, a game, a sculpture, a painting, a theatre production, a play, an opera, a musical, an exhibition, a legal case report, a computer program, etc.). This can be a work that is being quoted or referenced in detail (i.e., a citation), or it can just be a work that is mentioned in passing.

A person's name is not the title of a work — even if people call that person a piece of work — and the element must therefore not be used to mark up people's names.

A citation is not a quote.

The text in the `cite` element usually renders in italic.

### Use cases

In the context of the `cite` element, a creative work could be, for example, one of the following:

* A book
* A research paper
* An essay
* A poem
* A musical score
* A song
* A play or film script
* A film
* A television show
* A game
* A sculpture
* A painting
* A theatrical production
* A play
* An opera
* A musical
* An exhibition
* A legal case report
* A computer program
* A website
* A web page
* A blog post or comment
* A forum post or comment
* A tweet
* A Facebook post
* A written or oral statement

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
That was the citation from the <cite>Vulgata</cite>.
```

**Samples**:
* [Basic](../../../samples/elements/cite/cite.html)

### Related elements

* In some cases, the [**`b`**](#bold) element might be appropriate for names; e.g. in a gossip article where the names of famous people are keywords rendered with a different style to draw attention to them. In other cases, if an element is really needed, the span element can be used.)
* A citation is not a quote, for which the [**`q`**](#quotation) element is appropriate.
