# Communication Guidelines

<br>

>Writing gets real when it is read. Before that, it is a dream in letters. Writing to get read makes you careful, responsible, and considerate.

— [Oliver Reichenstein](https://ia.net/topics/take-the-power-back/)

>The way you communicate a thing creates the thing. The thing does not exist apart from its own communication.

— [Matt LeMay](https://twitter.com/mattlemay/status/1389961793175310344)

<!--BREAK-->

## Introduction

Communication is integral, not additive, to architecture — because it clarifies thinking, enables collaboration and supports scale.

This document encourages UXA practitioners to communicate — by providing guidelines for efficient, consistent and memorable material. Practitioners are expected to be familiar with UX concepts, that are only explained here when then have a specialized meaning in architecture. This document is thus a reference handbook: it inventories UXA conventions and parameters, but doesn’t explain nor justify them.

<!-- quick and easy for the author, consistent and memorable for the reader -->

This document is relevant for reference material, like best practices, and pedagogical material, like trainings. It’s not relevant for pitching, marketing nor UI copywriting.
<!-- in presentation decks, folioed documents, wiki pages, or printed posters -->

### Conventions

Some terms used throughout this document have a particular meaning in the UXA context:

- Document (Marked; for reading or reference) vs presentation (Deckset, for presentation or reference).
- Inline vs full-screen
- Figures (illustration, diagram, chart, photograph, gif, screenshot) vs images vs tables

<!--BREAK-->

## 1 Structure

### 1.1 Content

Always provide local context (scope, assumptions, environment etc); invisible meta on *everything*

Explicitly declare normative vs non-normative sections.

Content Order: Overview/abstract/general before details/concrete/specific.

Start with good practices
Don’t cover bad practices, unless some recurring misconception needs active correction.

<!-- DOs/DONTs vs only DOs vs good/better/best? -->

Expose the intention > explain the behaviour > describe the properties
Illustrate with tokens: tool for spec & governance > capture design decision > json kvp

split between long form and quicker tips/conventions

+notion of it has to be simplified, caricatural, true enough to not suspend disbelief etc; in writing or illustrating

### 1.2 Morphology

could it be a list, a comparison table, a data table, a diagram, a reference ppt? *Make a super clear, super big decision tree for “how to shape your content/here’s a boilerplate” depending on the deliverable. Eg best practices page: start from a must/could/should bullet list, etc.*

If text:

Each notion should be one paragraph and one only.
<!-- So it’s actually one section -->

Each paragraph should be structured in the same way: first the notion <!-- result/guidance --> expressed in a few words. Then its rationale (optional), best practices (optional) and alternatives (optional). <!-- Further reading (connection to other concepts, perspectives, controversies, details etc.) -->  
everything but the idea is optional since in a lot of cases, the instruction standalone can be acted upon immediately, even if somewhat less effectively, while explanations can be added later. Thus trading depth for breadth allows for a quicker “initial overview”.
No paragraph should be longer than 10-15 lines.

![](assets/communication,writing-guidelines,structure@2x.png)

Alineas (line breaks) can be used within a paragraph to add structure.

- The preferred length of paragraphs is three or four sentences, but five or six are acceptable.
- The preferred average sentence is 17 words or less, but up to 20 is acceptable.

<!--BREAK-->

## 2. Writing

### 2.0 Syntax

Apply a [parallel structure](https://owl.purdue.edu/owl/general_writing/mechanics/parallel_structure.html) whenever possible.

Apply a *must/could/should* structure whenever possible. <https://www.rfc-editor.org/rfc/rfc2119>

### 2.1 Vocabulary

Be very mindful of vocabulary.

Prefer generic terms over terms of art. Terms of art (words or phrases that have a precise, specialized meaning within a particular field or profession) are an essential communication tool, but should only be used to capture crucial meaning that would otherwise be lost. The only reason to use a technical term rather than a more common word is that it precisely expresses something that would otherwise be ambiguous or unclear.

Define technical terms, uncommon words and common words that are used in an unusual or special way. Define them immediately following their first occurrence in the text.

Avoid abbreviations.

When several (about 10) new terms or abbreviations are used, provide a glossary or list of acronyms.
Include it in the document, or contribute and link to the **Vocabulary** (to be published).

Avoid synonyms, especially in domain-specific matters, as well as fuzzy terms and everything-buckets. Aim to reuse the same, simple words as much as possible.

Replace or clarify terms that could be interpreted in different ways. E.g. it is not clear if an “alert” is about an error message, a business rule, a push notification or an exception indicator.

Avoid fuzzy spelling, e.g. “dropdown” vs “drop-down” vs “drop down”.

When referring to existing content, such as a UI or a diagram, spell commands, labels or messaging exactly as they appear in situ.

Everything-buckets are ill-defined terms that don’t really describe anything, such as “framework”. Their looseness often provide the appearance of agreement, to the detriment of actionability. Spot them and replace them with clearer explanations.

### 2.3 Spelling

Use American spelling. When in doubt, check the [Merriam-Webster dictionary](https://www.merriam-webster.com/) for the preferred spelling of specific terms.

### 2.3 Tone & Voice

For descriptions, use the present tense and the active form (“Selecting a value triggers validation”).
For instructions, use the second person imperative (“Remove test set”).

Prefer positive wording, and statements directed to what’s true rather than what’s false; it’s quicker to check.  
Use negative wording for prohibition or to correct misconceptions.

In any case be assertive, impersonal and use the [singular *they*](https://en.wikipedia.org/wiki/Singular_they) form.

<!-- Faire porter les énoncés sur ce qui est vrai plutôt que sur ce qui est faux (dans les tâches de vérification). Raison: on est plus rapide à vérifier ce qui est vrai que ce qui est faux. -->

<!-- use the passive voice if the object (thing being done) is more important than the subject (person doing the thing) -->

### 2.2 Sourcing

Make sure content, in particular fonts or images from Internet, are explicitly allowed to be used. This can be achieved through various means, like an open-source license or the purchase of a commercial license.

<!-- authoritative / verified / quality (in data, in presentation) sourcing -->
<!-- Heh == prefer authoritative data -->
<!-- authoritative sourcing != legal sourcing -->

### 2.3. Attribution

Most documents or presentations are built upon on other people’s ideas, data or work. It’s important to only ever use authorized material, and credit it properly.

Provide attribution for other people’s material.  
Inline attribution, located directly where the material is, is the preferred way of doing attribution. It works well for most quotes, tables or figures.
Reference attribution, separate from the material and gathered at the end of the document, is possible when inline attribution isn’t appropriate for aesthetic or technical reasons. It’s mostly for full-slide images.

If the author asks for a specific an attribution format, use it. If not, use the following:

- Inline: `<work title>, <author name>, <work year>`
- Reference: `<page/slide number>: <work title>, <author name>, <work year>`

Do not use footnotes for attribution.

<!-- provide examples: default, talk within a conference, figure within a document, etc. -->
<!-- the point is to be fair and useful (provide context), not be dogmatic nor academic -->

<!-- citation, attribution, sources, references, credits, further resources -->
<!-- [How to Cite Your Sources](https://gouldguides.carleton.edu/citation/attribution) -->
<!-- APA -->
<!-- titre *exact* de la section d'attribution? credits, bibliographie, sources, etc. -->

### 2.4. Formatting

<!-- Heh pas terrible, c’est plutôt “conventions et finitions” -->

#### 2.4.1 Style Conventions

Use title case for headings.

If typographic emphasis is used, it shall be boldface type.
Use **strong** styling for keywords.

*expand with dod material*

Punctuate list items: with a period if it’s a complete sentence, or sentences. Otherwise with commas. The last item is punctuated with a period.

Avoid parentheses. Use commas or rephrase.

<!-- Don’t use ampersands (&). They attract attention to the least important part of the sentence. Spell out the word “and.” -->

<!-- Un titre d’activité ne contient pas de verbe d’action afin de ne pas le confondre avec une étape. -->

Use apostrophes to form possessives:

- Singular nouns: add ’s, even if they end in s (merchant’s, bus’s)
- Plural nouns that don’t end in s: add ’s (women’s, men’s)
- Plural nouns that end in s: add an apostrophe (boxes’, customers’)

Oxford Comma Y/N?

#### 2.4.2 Number and Dates

Numbers representing quantities of 10 or more shall be expressed in numerals ; those representing quantities less than 10 shall be expressed in words. If a number is the first word in a sentence, it shall be expressed in words.

*Preferred date/time format, units formats and spaces etc*

These guidelines are for American English, which is the language we use as a base before translating to other languages. However, dates, numbers, and measurements may be formatted differently in other languages.

When possible, use the month’s full name, for example, October. If there are space constraints, use 3-letter abbreviations, for example, Oct. Don’t write dates numerically, for example, 07-02-14.

Don’t use ordinal indicators, which are words representing position or rank in a sequential order (1st, 2nd, 3rd, and so on).

Use commas for numbers with four or more digits. Whenever possible, don’t truncate numbers

Use an en dash without a space on either side for number ranges:

In all cases, include a space between the number and the unit.

When listing out multiple measurements in a row, put the unit of measurement at the end instead of after each number (and include a space).

#### 2.4.2 Typographic Signs

Be mindful about typographic signs. In particular:

- Abbreviations: e.g., etc., i.e. with periods,
- Apostrophes and quote marks: curly instead of straight; run the [smart-quotes-plus](https://atom.io/packages/smart-quotes-plus) package,
- Fractions: real fractions like ¼ instead of fake ones like 1/4; supported by Inter and iA Writer Quattro,
- Multiplication signs: × instead of the letter x.

Refer to [Glyphy](https://www.glyphy.io/) to grab rarer signs like ⅓, ↪ or ⚠.

#### 2.4.3 Foreign Words

Foreign words should be italicized, and immediately followed by their translation in parentheses.

<!--BREAK-->

## 3 Illustrating

### 3.1 Usage

When/what to illustrate: covers/back covers for style, caricatured examples for trainings, charts-instead-of-text, etc.

Illustrate profusely. At least an illustration every 2-3 slides. They help keep reader interest.

Always associate illustrations directly to the content they support, e.g. floated right.

Make sure full-page illustrations are commented in *presenter’s notes* (see xxx) as otherwise they lack the context required to be useful.

Don’t illustrate bad practices. In the rare case a bad practice has to be depicted, always depict the corresponding good practice immediately next to it.

### 3.2 Style

Use a consistent pictorial style for all comparable figures in a document, for example, all line drawings, or all photographs. Follow the style provided by the [moodboard](https://www.pinterest.ca/nwodtcobalt/uxa/).

Photographs or screenshots can be used as examples or explanations, but should not be used for editorial purposes. Prefer illustrations.

### 3.3 Grid

This guidance is most relevant for heavily templated tools like Deckset or Marked, that offer little control over the size, position or treatment of images. Manually laid out documents may go past the conventions covered here.

Units can be expressed as pixels (px), points (pt) or dips (dp) depending on the OS. They are hereafter noted as pixels for clarity.

<!-- A **unit** is the smallest measure a vertex can be positioned at accurately. It depends on the physical and logical resolution of the device, and can be expressed as pixels (px), points (pt), dips (dp). Units are hereafter noted as pixels for clarity. -->

#### 3.3.1 Parameters

The UXA grid is set to an 8 px module.

<!--
| Parameter     | Value         | Definition                                               |
| ------------- | ------------- | -------------------------------------------------------- |
| Module        | 8 px          | The recurring measure vertices are anchored at           |
| Aspect ratio  | 16:9          | The relative size of the width to the height of an image |
| Artboard size | 1600 × 900 px | The absolute size of an image                            |
 -->

![Grid Parameters](assets/grid-parameters@2x.png)

#### 3.3.2 Form Factors/Layout

While the canonical 1600 × 900 px artboard size is well-suited to full-screen rendering, it can be unwieldy to use alongside text. Derived artboard sizes are available:

![Artboards Form Factors](assets/artboard-form-factors@2x.png)

| Type         |  Size (px) | Usage                                                       |
| ------------ | ----------:| ----------------------------------------------------------- |
| 1 artboard   | 1600 × 900 | Full-screen in presentation  (or stand-alone, or in poster) |
| 1/2 artboard |  800 × 900 | Inline in presentation (e.g. next to bullet points)         |
| 1/4 artboard |  800 × 450 | Inline in document (e.g. between two paragraphs)            |

Artboards contain various guides helping to lay out content quickly and consistently:

1. Artboard: export frame of the figure
2. Measurement origin: virtual border from which all content should be measured and aligned. Set so that content can be laid out on a 8 px grid within the larger 1600 × 900 px artboard, that doesn’t support it by default.
3. Visual clearance: 40 px for docs, 40/80 px for slides (against canvas edge, not safe area edge. Exceptionally 10px, eg screenshot (and most dont qualify to begin with). full bleed only for impact, on bg stuff.
4. Content keylines: optional preferred positions for content

![Layout Templates](assets/layout-templates@2x.png)

Inline doc: shave vertically as much as possible (to not disrupt reading flow).
Can be vertically shortened (only at export time, so that it’s easy to get back to nominal).
try and catch a preferred size.

![Inline illustration shortening](assets/inline-illo-shortening@2x.png)

#### 3.3.3 Preferred Sizes

Specific values along the 8 px grid are preferred when working on editorial layouts.

While an 8 px module is appropriate for fine work like UI design, it’s too granular for illustrations or pages layout, where elements are sized and positioned at a much bigger scale. Thus specific, bigger values are picked out of all the possible multiples of 8.

The preferred values are multiples of 8 (the UXA grid module) and 10 (another frequent grid module), ensuring scale and compatibility. Multiples of 4 (half UXA grid module) and 10 are also possible, as a second choice. Straight multiples of 8 are the last resort.

<!-- scales, series, stop points? major, minor, module? preferred, possible, fallback? -->
<!-- the half module series are identical: n(4 × 10) = n(8 × 5) -->

[Preferred Sizes]
| Priority | Rythm (px) | Sample values (px)                                    |
| -------- | ---------- | ----------------------------------------------------- |
| 1        | 8 × 10     | 80, 160, 240, 420, 400, 480, 560, 640, 720, 800, etc. |
| 2        | 4 × 10     | 40, 80, 120, 160, 200, 240, 280, 320, 360, 400, etc.  |
| 3        | 8 × 1      | 8, 16, 24, 32, 40, 48, 56, 64, 72, 80, etc.           |

Note that these preferred values are just a starting point, merely minimizing accidental divergences. Better layouts would require further refinement, like [harmonic scales](https://type-scale.com/) or [Renard series](https://en.wikipedia.org/wiki/Renard_series).

### 3.4 Export

<!-- svg > pdf > png > jpg -->

Export to SVG by default.  
SVG files are scalable, interoperable, programmatically manipulable and lightweight.
Some specific use cases may require other formats:

| Priority | Format | Scaling | Usage                                            |
| -------- | ------ | ------- | ------------------------------------------------ |
| 1        | SVG    | 1x      | Vector figures without text (e.g. illustrations) |
| 2        | PDF    | 1x      | Vector figures with text (e.g. diagrams)         |
| 3        | PNG    | 2x      | Screenshots, UI mockups                          |
| 4        | JPG    | 2x      | Photos, scanned documents                        |

Set an illustration background color, `Gris 0106 Béton Clair` by default.
<!-- Marked-only? -->

Illustration assets can be rendered in a variety of contexts such as a high-contrast Markdown client, a dark-mode browser or a hand-off, inspection or version control tool. Their background color is unknown, and some of them could make the illustration foreground illegible.

Moreover, some photos may not have a 16:9 aspect ratio meaning the document background will bleed through. Depending on the photo color, the `Gris 0106 Béton Clair` background may not work well. In this case, it’s possible to select the closest-matching UXA color (e.g. `Noir 1571 Jais`), or to sample an appropriate color from the photo.
<!-- Heh that’s actually slide bg , not illo bg + 90% scaling-->

Do not pick an arbitrary background color for editorial purposes, like calling for attention.
<!-- divider entre recommendations marked et recommendations deckset ? peu d’overlap au final -->

![Background Color](assets/background-color@2x.png)

### 3.5 Examples

*florilège annoté*

<!--BREAK-->

## 4 Deckset & Marked Minutiae

### 4.1 Marked

Finalize document:

- Insert a `<!--BREAK-->` tag immediately after the top H1, to yield a clean cover page

Configure Marked:

- Enable `Export`/`Prevent orphaned headlines`
- Enable `Export`/`Add page breaks before/Footnotes`

Export with Marked:

- Set the theme to [UXASF1](https://github.com/nWODT-Cobalt/markown-utilities)
- Select `Export As`/`Save PDF (Paginated)`

<!-- Major divisions of the document should begin on right hand-pages. Right-hand pages shall be odd-numbered pages, and left hand pages shall be even-numbered pages. -->

<!-- A user document shall have a table of contents unless it has fewer than three divisions or fewer than six pages. A table of contents shall include: (a) at least two levels of the headings and subheadings of the document, (b) appendixes if they exist, (d) list of exhibits, illustrations, figures and tables if they exist, and (e) the original page number of each item listed. The table of contents shall begin on a right-hand page. -->

### 4.2 Deckset

Present or export Deckset presentations with the [UXASF1](/Resources/Deckset) theme.

<!-- Keep it focused, keep it small. 5 slides or less is perfectly fine. People can’t remember more than 3 points from a speech. (KK) -->
<!-- Actually: make small, focused documents all the time -->

Do not hesitate to format Deckset presenter’s notes; they will render so on Deckset and on Github.

<!--BREAK-->

## 5 Naming Convention & File Organization

<!-- Split into different document ? -->

Naming schemes ? esp for artboards

Names: case sensitive, no spaces (within a project, not between projects)

<!--BREAK-->

## 9 Sources

- Règles rédaction, JM Foulon, 2007
- HFDS 2003
- IND6408
- [Grammar and mechanics — Shopify Polaris](https://polaris.shopify.com/foundations/content/grammar-and-mechanics), Shopify, 2022
- [Swift API Design Guidelines](https://swift.org/documentation/api-design-guidelines/), Apple, 2020

<!--BREAK-->

# Under Consideration

TBD:

- Handbook / IND6408
- UXA·ID?
- Page numbers?
- Titles on individual slides?
- Highlight sparsely (e.g. command names, symbol names)?
- TOC, recap?
- Qualités: Validité, Clarté/Transparence, Granularité, Uniformité, Cohérence, Complétude, Disponibilité, Accessibilité, Utilisabilité
- Highlight words Style to indicate to the reader that they refer to entities in our own design system, rather than generic notions.
- Pour chaque action significative ou groupe d’actions significatives reliées, on inclut une ou des vérifications afin de s’assurer que leur exécution a apporté les résultats attendus.
- Embrace precedent. Don’t optimize terms for the total beginner at the expense of conformance to existing culture.
- Keep annotations terse. Economy of concepts and terms is a primary goal.
- style guide TLDR: noir jais pour premier plan, gris béton clair pour arrière plan, bleu xxx pour emphase, gris xxx pour déemphase.


boilerplate f(type of document):

Eg for ~collaboration reference, esp when ppl come from different trades, orgs, etc.

- Any prerequisite or context, including definition of terms of art
- Overall goals and scope
- Principles, expressed in a decision-supportive way (see SADMEME). Basically clarifying how will decisions be taken. Typically statements like “xx over yy over zz” or “xx is a goal, yy is a byproduct”
- Technical guidance, expressed in a conformative way.  Eg must/could/should format, do/don’t format, controlled list of values, etc.
- Some thoughts about governance. Who does what, who’s checking what, who says things are good to go etc. What’s the contribution model past the initial effort, etc.
- Ideally structured after the process, rather than the tool or the assets; acknowledging that the audience is proficient or debutant.
