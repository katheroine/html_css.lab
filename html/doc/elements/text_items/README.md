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

### Attributes

Authors can use the `class` attribute on the `i` element to identify *why* the element is being used, so that if the style of a particular use (e.g. dream sequences as opposed to taxonomic terms) is to be changed at a later date, the author doesn't have to go through the entire document (or series of related documents) annotating each use.

Terms in languages different from the main text should be annotated with `lang` attributes (or, in XML, `lang` attributes in the XML namespace).

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

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

### Attributes

Authors can use the `class` attribute on the `b` element to identify why the element is being used, so that if the style of a particular use is to be changed at a later date, the author doesn't have to go through annotating each use.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

#### Use cases

* *Keywords* in a summary
* *Product names* in a review
* Other spans of text whose typical presentation would be boldfaced (but not including any special importance)

#### History

Historically, the `b` element was meant to make text boldface. Styling information has been deprecated since HTML4, so the meaning of the `b` element has been changed.

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

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

#### Use cases

* Annotating spelling errors
* A proper name mark to denote proper names in Chinese text
* Other forms of annotation

#### History

Along with other pure styling elements, the original HTML Underline `u` element was deprecated in HTML 4. However, `u` was restored in HTML 5 with a new, semantic, meaning: to mark text as having some form of non-textual annotation applied.

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

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Use cases

* *Importance*: the `strong` element can be used in a heading, caption, or paragraph to distinguish the part that really matters from other parts that might be more detailed, more jovial, or merely boilerplate. (This is distinct from marking up subheadings, for which the `hgroup` element is appropriate.)
* *Seriousness*: the `strong` element can be used to mark up a warning or caution notice. Accepted use for `strong` is to denote the labels of paragraphs which represent notes or warnings within the text of a page.
* *Urgency*: the `strong` element can be used to denote contents that the user needs to see sooner than other parts of the document.

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

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Use cases

* When used in a quotation (`q`) or block quote (`blockquote`), it generally indicates text which is of special interest but is not marked in the original source material, or material which needs special scrutiny even though the original author didn't think it was of particular importance. Think of this like using a highlighter pen in a book to mark passages that you find of interest.
* Otherwise, `mark` indicates a portion of the document's content which is likely to be relevant to the user's current activity. This might be used, for example, to indicate the words that matched a search operation.

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

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

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

### Examples

```html
That was the citation from the <cite>Vulgata</cite>.
```

**Samples**:
* [Basic](../../../samples/elements/cite/cite.html)

### Related elements

* In some cases, the [**`b`**](#bold) element might be appropriate for names; e.g. in a gossip article where the names of famous people are keywords rendered with a different style to draw attention to them. In other cases, if an element is really needed, the span element can be used.)
* A citation is not a quote, for which the [**`q`**](#quotation) element is appropriate.

## Definition

### Documentation

|Website  |URL                                                                             |
|---------|--------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-dfn-element|
|W3CSchool|https://www.w3schools.com/tags/tag_dfn.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/dfn        |

### Tag

```html
<dfn></dfn>
```

### Description

The defining instance of a term.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `dfn` element represents the defining instance of a term, and it specifies a term that is going to be defined within the content.

The `dfn` element should be used in a complete definition statement, where the full definition of the term can be one of the following:

* The ancestor ***paragraph*** (a block of text, sometimes marked by a `p` element)
* The ***description list group*** (a `dt`/`dd` pairing),
* The nearest ***section*** ancestor of the `dfn` element,

So, the nearest ancestor of the `dfn` element must also contain the definition(s) for the term given by the `dfn` element.

### Attributes

#### `title`

**Value**: Text

**Description**: Specifies the term being defined

**Example**:

```html
<dfn title="Some Term"></dfn>
```

If the `title` attribute of the dfn element is present, then it must contain only the term being defined.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Use cases

The term inside the `dfn` tag can be any of the following:

* Just as the content of the `dfn` element:

```html
<p><dfn>HTML</dfn> is the standard markup language for creating web pages.</p>
```

* Or, with the title attribute added:

```html
<p><dfn title="HyperText Markup Language">HTML</dfn> is the standard markup language for creating web pages.</p>
```

* Or, with an `abbr` tag inside the `dfn` element:

```html
<p><dfn><abbr title="HyperText Markup Language">HTML</abbr></dfn> is the standard markup language for creating web pages.</p>
```

* Or, with the id attribute added. Then, whenever a term is used, it can refer back to the definition with an `a` tag:

```html
<p><dfn id="html-def">HTML</dfn> is the standard markup language for creating web pages.</p>

<p>This is some text...</p>
<p>This is some text...</p>
<p>Learn <a href="#html-def">HTML</a> now.</p>
```

**Specifying the term being defined**

The term being defined is identified following these rules:

* If the `dfn` element has a `title` attribute, the value of the `title` attribute is considered to be the term being defined. The element must still have text within it, but that text may be an abbreviation (perhaps using `abbr`) or another form of the term.
* If the `dfn` contains a single child element and does not have any text content of its own, and the child element is an `abbr` element with a `title` attribute itself, then the exact value of the `abbr` element's title is the term being defined.
* Otherwise, the text content of the `dfn` element is the term being defined.
* If the `dfn` element has a `title` attribute, it must contain the term being defined and no other text.

**Links to `dfn` elements**

If you include an `id` attribute on the `dfn` element, you can then link to it using `a` elements. Such links should be uses of the term, with the intent being that the reader can quickly navigate to the term's definition if they're not already aware of it, by clicking on the term's link.

### Examples

* Basic identification of a term

This example uses a plain `dfn` element to identify the location of a term within the definition.

```html
<p>
  The <strong>HTML Definition element (<dfn>&lt;dfn&gt;</dfn>)</strong> is used
  to indicate the term being defined within the context of a definition phrase
  or sentence.
</p>
```

Since the `dfn` element has no `title`, the text contents of the `dfn` element itself are used as the term being defined.

* Links to definitions

To add links to the definitions, you create the link the same way you always do, with the `a` element.

```html
<p>
  The <strong>HTML Definition element (<dfn id="definition-dfn">&lt;dfn&gt;</dfn>)</strong>
  is used to indicate the term being defined within the context of a definition
  phrase or sentence.
</p>

<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Graece donan, Latine
  voluptatem vocant. Confecta res esset. Duo Reges: constructio interrete.
  Scrupulum, inquam, abeunti;
</p>

<p>
  Because of all of that, we decided to use the
  <code><a href="#definition-dfn">&lt;dfn&gt;</a></code> element for this project.
</p>
```

Here we see the definition — now with an `id` attribute, "definition-dfn", which can be used as the target of a link. Later on, a link is created using `a` with the `href` attribute set to "#definition-dfn" to set up the link back to the definition.

* Using abbreviations and definitions together

In some cases, you may wish to use an abbreviation for a term when defining it. This can be done by using the `dfn` and `abbr` elements in tandem, like this:

```html
<p>
  The <dfn><abbr title="Hubble Space Telescope">HST</abbr></dfn> is among the
  most productive scientific instruments ever constructed. It has been in orbit
  for over 20 years, scanning the sky and returning data and photographs of
  unprecedented quality and detail.
</p>

<p>
  Indeed, the <abbr title="Hubble Space Telescope">HST</abbr> has arguably done
  more to advance science than any device ever built.
</p>
```

Note the `abbr` element nested inside the `dfn`. The former establishes that the term is an abbreviation ("HST") and specifies the full term ("Hubble Space Telescope") in its title attribute. The latter indicates that the abbreviated term represents a term being defined.

**Samples**:
* [Basic](../../../samples/elements/dfn/dfn.html)
* [With `title` attribute](../../../samples/elements/dfn/dfn.attribute_title.html)
* [With `abbr` element](../../../samples/elements/dfn/dfn.element_abbr.html)
* [With `id` attribute and `a` element](../../../samples/elements/dfn/dfn.attribute_id_element_a.html)
* [With `dt` element](../../../samples/elements/dfn/dfn.element_dt.html)

### Relative elements

* The full definition of the term can be in the ancestor [**`p`**](#paragraph) element.
* The full definition of the term can be in the [**`dd`**](#dd) element.
* The full definition of the term can be in the narest ancestor [**`section`**](#section) element.
* The `dfn` element can be nested by the [**`dt`**](#dt) element.
* The `dfn` element can nest the [**`abbr`**](#abbreviation) element.
* The [**`a`**](#anchor) element can lead to the `dfn` element.

## Abbreviation

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-abbr-element|
|W3CSchool|https://www.w3schools.com/tags/tag_abbr.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/abbr        |

### Tag

```html
<abbr></abbr>
```

### Description

An abbreviation or acronym.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `abbr` element represents an abbreviation or acronym, optionally with its expansion. The `abbr` tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".

### Use cases

Abbreviations do not have to be marked up using this element. It is expected to be useful in the following cases:

* *Abbreviations for which the author wants to give expansions*, where using the `abbr` element with a `title` attribute is an alternative to including the expansion inline (e.g. in parentheses).
* *Abbreviations that provide an expansion or definition outside the flow of the document's content*, for which `abbr` is used with an appropriate `title` attribute.
* *Abbreviations that are likely to be unfamiliar to the document's readers*, for which authors are encouraged to either mark up the abbreviation using an `abbr` element with a `title` attribute or include the expansion inline in the text the first time the abbreviation is used.
* *Abbreviations whose presence needs to be semantically annotated*, e.g. so that they can be identified from a style sheet and given specific styles, for which the `abbr` element can be used without a `title` attribute.

It's certainly not required that all abbreviations be marked up using `abbr`. There are, though, a few cases where it's helpful to do so:

* When an abbreviation's presence in the text needs to be semantically noted, the `abbr` element is useful. This can be used, in turn, for styling or scripting purposes.
* You can use `abbr` in concert with `dfn` to establish definitions for terms which are abbreviations or acronyms.
* When including an abbreviation or acronym, provide a full expansion of the term in plain text on *first use*, along with the `abbr` to mark up the abbreviation.

**Grammar considerations**

In languages with grammatical number (that is, languages where the number of items affects the grammar of a sentence), use the same grammatical number in your title attribute as inside your `abbr` element. This is especially important in languages with more than two numbers, such as Arabic, but is also relevant in English.

### Default styling

The purpose of this element is purely for the convenience of the author and all browsers display it inline (display: inline) by default, though its default styling varies from one browser to another.

Some browsers add a dotted underline to the content of the element. Others add a dotted underline while converting the contents to small caps. Others may not style it differently than a `span` element. To control this styling, use text-decoration and font-variant.

### Accessibility

Spelling out the acronym or abbreviation in full the first time it is used on a page is beneficial for helping people understand it, especially if the content is technical or industry jargon.

Only include a `title` if expanding the abbreviation or acronym in the text is not possible. Having a difference between the announced word or phrase and what is displayed on the screen, especially if it's technical jargon the reader may not be familiar with, can be jarring.

```html
<p>
  JavaScript Object Notation (<abbr>JSON</abbr>) is a lightweight data-interchange format.
</p>
```

This is especially helpful for people who are unfamiliar with the terminology or concepts discussed in the content, people who are new to the language, and people with cognitive concerns.

### Attributes

#### `title`

**Value**: Text

**Description**: Specifies the term being defined

**Example**:

```html
<Abbr title="Some Term"></abbr>
```

The `title` attribute may be used to provide an expansion of the abbreviation. The attribute, if specified, must contain an expansion of the abbreviation, and nothing else. Use the global `title` attribute to show the description for the abbreviation/acronym when you mouse over the element. This text is often presented by browsers as a tooltip when the mouse cursor is hovered over the element.

The `title` attribute has a specific semantic meaning when used with the `abbr` element. It must contain a full human-readable description or expansion of the abbreviation.

Providing an expansion in a `title` attribute once will not necessarily cause other `abbr` elements in the same document with the same contents but without a `title` attribute to behave as if they had the same expansion. Every `abbr` element is independent.

Include a `title` attribute only when the inline expansion or definition is not available.

Each `abbr` element you use is independent of all others, providing a title for one does not automatically attach the same expansion text to others with the same content text.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
We used to structure the text with the <abbr title="Hypertext Markup Language">HTML</abbr> as a commonly recognized standard.
```

**Samples**:
* [Basic](../../../samples/elements/abbr/abbr.html)
* [With `title` attribute](../../../samples/elements/abbr/abbr.attribute_abbr.html)
* [With **`dfn`** element](../../../samples/elements/abbr/abbr.element_dfn.html)

### Related elements

* Use `abbr` in concert with [**`dfn`**](#definition) to establish definitions for terms which are abbreviations or acronyms

## Variable

### Documentation

|Website  |URL                                                                             |
|---------|--------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-var-element|
|W3CSchool|https://www.w3schools.com/tags/tag_var.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/var        |

### Tag

```html
<var></var>
```

### Description

A variable.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `var` element represents a variable. This could be an actual variable in a mathematical expression or programming context, an identifier representing a constant, a symbol identifying a physical quantity, a function parameter, or just be a term used as a placeholder in prose.

For mathematics, in particular for anything beyond the simplest of expressions, **MathML** is more appropriate. However, the var element can still be used to refer to specific variables that are then mentioned in MathML expressions.

### Default style

It's typically presented using an italicized version of the current typeface, although that behavior is browser-dependent.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
In physics, <var>a</var> means the acceleration.
```

**Samples**:
* [Basic](../../../samples/elements/var/var.html)

### Related elements

* Use the [**`code`**](#code) element for the computer language.
* Use the [**`kbd`**](#keyboard) element for the he keyboard input.
* Use the [**`samp`**](#sample) element for the sample output.
* Use the [**`span`**](#span) element for the styling purposes.

## Code

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-code-element|
|W3CSchool|https://www.w3schools.com/tags/tag_code.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/code        |

### Tag

```html
<code></code>
```

### Description

A code fragment.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `code` element represents a fragment of computer code. This could be an XML element name, a filename, a computer program, or any other string that a computer would recognize.

The `code` element by itself only represents a single phrase of code or line of code.

There is no formal way to indicate the language of computer code being marked up. Authors who wish to mark code elements with the language used, e.g. so that syntax highlighting scripts can use the right rules, can use the class attribute, e.g. by adding a class prefixed with "language-" to the element.

The content inside is displayed in the browser's default monospace font.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
The short example of the code could be <code>print("Hello, world!");</code> simply displaying a given text.
```

**Samples**:
* [Basic](../../../samples/elements/code/code.html)
* [With **`pre`** element](../../../samples/elements/code/code.element_pre.html)

### Related elements

* To represent multiple lines of code, wrap the `code` element within a [**`pre`**](#preformatted) element.

## Keyboard

### Documentation

|Website  |URL                                                                             |
|---------|--------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-kbd-element|
|W3CSchool|https://www.w3schools.com/tags/tag_kbd.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/kbd        |

### Tag

```html
<kbd></kbd>
```

### Description

A code fragment.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `kbd` element represents user input (typically keyboard input, although it may also be used to represent other input, such as voice commands).

When the `kbd` element is nested inside a `samp` element, it represents the input as it was echoed by the system.

When the `kbd` element contains a `samp` element, it represents input based on system output, for example invoking a menu item.

When the `kbd` element is nested inside another `kbd` element, it represents an actual key or other single unit of input as appropriate for the input mechanism.

The content inside is displayed in the browser's default monospace font.

**Representing keystrokes within an input**

To describe an input comprised of multiple keystrokes, you can nest multiple `kbd` elements, with an outer `kbd` element representing the overall input and each individual keystroke or component of the input enclosed within its own `kbd`.

```html
<p>
  You can also create a new document using the
  <kbd><kbd>Ctrl</kbd>+<kbd>N</kbd></kbd> keyboard shortcut.
</p>
```

This wraps the entire key sequence in an outer `kbd` element, then each individual key within its own, in order to denote the components of the sequence.

You don't need to do all this wrapping. You can choose to simplify it by leaving out the external `kbd` element. In other words, simplifying this to just `<kbd>Ctrl</kbd>+<kbd>N</kbd>` would be perfectly valid.

Depending on your style sheet, though, you may find it useful to do this kind of nesting.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
To list all files from the current working directory with some additional information run a command <kbd>ls -l</kbd>.
```

**Samples**:
* [Basic](../../../samples/elements/kbd/kbd.html)
* [With **`samp`** element](../../../samples/elements/kbd/kbd.element_samp.html)

### Related elements

* Nesting a `kbd` element inside a [**`samp`**](#sample) element represents input that has been echoed back to the user by the system.
* Nesting a [**`samp`**](#sample) element inside a `kbd` element, on the other hand, represents input which is based on text presented by the system, such as the names of menus and menu items, or the names of buttons displayed on the screen.

## Sample

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-samp-element|
|W3CSchool|https://www.w3schools.com/tags/tag_samp.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/samp        |

### Tag

```html
<samp></samp>
```

### Description

A sample or quoted output.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `samp` element represents sample or quoted output from another program or computing system.

**Sample output including user input**

You can nest the `kbd` element within a `samp` block to present an example that includes text entered by the user.

The content inside is displayed in the browser's default monospace font.

### Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
If the address is wrong you will see a message like <samp>404 Page not found</samp>.
```

**Samples**:
* [Basic](../../../samples/elements/samp/samp.html)
* [With **`kbd`** element](../../../samples/elements/samp/samp.element_kbd.html)

### Related elements

* Nesting a `kbd` element inside a [**`samp`**](#sample) element represents input that has been echoed back to the user by the system.
* Nesting a [**`samp`**](#sample) element inside a `kbd` element, on the other hand, represents input which is based on text presented by the system, such as the names of menus and menu items, or the names of buttons displayed on the screen.

## Data

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-data-element|
|W3CSchool|https://www.w3schools.com/tags/tag_data.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/data        |

### Tag

```html
<data></data>
```

### Description

A machine-readable form of contents.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `data` element represents its contents, along with a machine-readable form of those contents in the `value` attribute. The element is used to add a machine-readable translation of a given content.

The element can be used for several purposes.

When combined with microformats or the microdata attributes, the element serves to provide both a machine-readable value for the purposes of data processors, and a human-readable value for the purposes of rendering in a web browser. In this case, the format to be used in the value attribute is determined by the microformats or microdata vocabulary in use.

The element can also, however, be used in conjunction with scripts in the page, for when a script has a literal value to store alongside a human-readable value. In such cases, the format to be used depends only on the needs of the script. (The data-* attributes can also be useful in such situations.)

Sorting JavaScript library can provide a sorting mechanism on each list item or table row used values of the `value` attribute of the `data` element.

When the `value` is date- or time-related, the more specific `time` element can be used instead.

### Attributes

#### `value`

**Value**: Number

**Description**: Represents the element's contents in a machine-readable format.

**Example**:

```html
<data value="1234"></data>
```

The `value` attribute must be present. Its value must be a representation of the element's contents in a machine-readable format.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
Mathematicans ofter use the <data class="number" value="3.14">&#x3C0;</data>.
```

**Samples**:
* [Basic](../../../samples/elements/data/data.html)
* [With **`li`** element](../../../samples/elements/data/data.element_li.html)
* [With **`td`** element](../../../samples/elements/data/data.element_td.html)

### Related elements

* Often used with [**`li`**](#li) element.
* Often used with [**`td`**](#td) element.

## Time

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-time-element|
|W3CSchool|https://www.w3schools.com/tags/tag_time.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/time        |

### Tag

```html
<time></time>
```

### Description

A machine-readable form of date and/or time.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `time` element represents its contents, along with a machine-readable form of those contents in the datetime attribute. The kind of content is limited to various kinds of dates, times, time-zone offsets, and durations, as described below. For example, this can help a user agent offer to add an event to a user's calendar.

The `datetime` attribute may be present. A time element that does not have a `datetime` content attribute must not have any element descendants.

The datetime value of a time element is the value of the element's datetime content attribute, if it has one, otherwise the child text content of the time element.

The datetime value of a time element must match one of the following syntaxes.

[Full list of the valid datetime formats](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/time#valid_datetime_values).

## Attributes

#### `datetime`

**Value**: Date and/or time in the one of the acceptable formats.

**Description**: Represents the date/time in a machine-readable format.

**Example**:

```html
<data datetime="31.10.2025"></data>
```

If `datetime` attribute is present, its value must be a representation of the element's contents in a machine-readable format.

The `datetime` attribute of this element is used translate the time into a machine-readable format so that browsers can offer to add date reminders through the user's calendar, and search engines can produce smarter search results.

It may represent one of the following:

* A time on a 24-hour clock.
* A precise date in the Gregorian calendar (with optional time and timezone information).
* A valid time duration.

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
The conference will be held on <time datetime="10-12-2025">December 10, 2025</time>.
```

**Samples**:
* [Basic](../../../samples/elements/time/time.html)

## Superscript

### Documentation

|Website  |URL                                                                                      |
|---------|-----------------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-sub-and-sup-elements|
|W3CSchool|https://www.w3schools.com/tags/tag_sup.asp                                               |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/sup                 |

### Tag

```html
<sup></sup>
```

### Description

A superscript text.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `sup` element represents a superscript.

The `sup` element should only be used for typographical reasons - that is, to change the position of the text to comply with typographical conventions or standards, rather than solely for presentation or appearance purposes.

The `sup` tag defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes.

This element must be used only to mark up typographical conventions with specific meanings, not for typographical presentation for presentation's sake. For example, it would be inappropriate for the `sup` element to be used in the name of the LaTeX document preparation system. In general, authors should use this element only if the absence of this element would change the meaning of the content.

In certain languages, superscripts are part of the typographical conventions for some abbreviations.

Superscripts are usually rendered with a raised baseline using smaller text.

### Use cases

Appropriate use cases for `sup` include (but aren't necessarily limited to):

* *Displaying exponents*, such as "x3". It may be worth considering the use of MathML for these, especially in more complex cases.
* *Displaying superior lettering*, which is used in some languages when rendering certain abbreviations. For example, in French, the word "mademoiselle" can be abbreviated "Mlle"; this is an acceptable use case.
* Representing ordinal numbers, such as "4th" instead of "fourth."

For example, to style the wordmark of a business or product which uses a raised baseline should be done using CSS (most likely vertical-align) rather than `sup`.

## Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
In mathematics, the exponential function is described by the f(x) = e<sup>x</sup> formula.
```

**Samples**:
* [Basic](../../../samples/elements/sup/sup.html)

## Subscript

### Documentation

|Website  |URL                                                                                      |
|---------|-----------------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-sub-and-sup-elements|
|W3CSchool|https://www.w3schools.com/tags/tag_sub.asp                                               |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/sub                 |

### Tag

```html
<sub></sub>
```

### Description

A subscript text.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: Phrasing content

The `sub` element represents a subscript.

The `sub` element should be used only for typographical reasons - that is, to change the position of the text to comply with typographical conventions or standards, rather than solely for presentation or appearance purposes.

The `sub` tag defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas.

This element must be used only to mark up typographical conventions with specific meanings, not for typographical presentation for presentation's sake. For example, it would be inappropriate for the `sub` element to be used in the name of the LaTeX document preparation system. In general, authors should use this element only if the absence of this element would change the meaning of the content. Using `sub` to style the name of a company which uses altered baselines in their wordmark would not be appropriate; instead, CSS should be used.

The `sub` element can be used inside a `var` element, for variables that have subscripts.

Subscripts are typically rendered with a lowered baseline using smaller text.

### Use cases

Appropriate use cases for `sub` include (but aren't necessarily limited to):

* *Marking up footnote numbers*.
* *Marking up the subscript in mathematical variable numbers* (although you may also consider using a MathML formula for this).
* *Denoting the number of atoms of a given element within a chemical formula*.

## Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
Developer's best friend, C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>, otherwise known as "caffeine".
```

**Samples**:
* [Basic](../../../samples/elements/sub/sub.html)

## Ruby

### Documentation

|Website  |URL                                                                              |
|---------|---------------------------------------------------------------------------------|
|WHATWG   |https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-ruby-element|
|W3CSchool|https://www.w3schools.com/tags/tag_ruby.asp                                      |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/ruby        |

### Tag

```html
<ruby></ruby>
```

### Description

A ruby annotation.

**Type**: Inline

**Categories**:
* Flow content
* Phrasing content
* Palpable content

**Contexts in which this element can be used**:
* Where phrasing content is expected

**Content model**: See prose

The `ruby` element allows one or more spans of phrasing content to be marked with ruby annotations.

**Ruby annotations** are short runs of text presented alongside base text - rendered above, below, or next to base text, primarily used in East Asian typography as a guide for pronunciation or meaning of the corresponding characters or to include other annotations. In Japanese, this form of typography is also known as furigana and is often used in Japanese publications.

It can also be used for annotating other kinds of text, but this usage is less common.

The term ***ruby*** originated as a unit of measurement used by typesetters, representing the smallest size that text can be printed on newsprint while remaining legible.

The content model of ruby elements consists of one or more of the following sequences:

* One or the other of the following:

    * Phrasing content, but with no `ruby` elements and with no `ruby` element descendants
    * A single `ruby` element that itself has no `ruby` element descendants

* One or the other of the following:

    * One or more `rt` elements
    * An `rp` element followed by one or more `rt` elements, each of which is itself followed by an `rp` element


The `ruby` and `rt` elements can be used for a variety of kinds of annotations.

## Attributes

|Attributes support|   |
|------------------|---|
|Global attributes |YES|
|Event attributes  |YES|

### Examples

```html
<ruby>
  漢 <rp>(</rp><rt>Kan</rt><rp>)</rp> 字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>
```

**Samples**:
* [Basic](../../../samples/elements/ruby/ruby.html)

### Related elements

* Use `ruby` together with [**`rt`**](#rt) element that gives that information;
* And an optional [**`rp`**](#rp) element that defines what to show for browsers that do not support ruby annotations.
