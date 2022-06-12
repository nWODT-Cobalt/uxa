# Communication Guidelines

<br>

>Writing gets real when it is read. Before that, it is a dream in letters. Writing to get read makes you careful, responsible, and considerate.

— [Oliver Reichenstein](https://ia.net/topics/take-the-power-back/)

>The way you communicate a thing creates the thing. The thing does not exist apart from its own communication.

— [Matt LeMay](https://twitter.com/mattlemay/status/1389961793175310344)

<!--BREAK-->

## Introduction

Communication is integral, not additive, to architecture — because it clarifies thinking, enables collaboration and supports scale.

This document encourages UXA practitioners to communicate — by providing guidelines for efficient, consistent and memorable material.
<!-- quick and easy for the author, consistent and memorable for the reader -->

It's relevant for reference material, like best practices, and pedagogical material, like trainings. It's not relevant for pitching, marketing nor UI copywriting.
<!-- in presentation decks, folioed documents, wiki pages, or printed posters -->

<!--BREAK-->

## 1 Structure

### 1.1 Content

Always provide local context (scope, assumptions, environment etc); invisible meta on *everything*

Content Order: Overview/abstract/general before details/concrete/specific.

Start with good practices
Don't cover bad practices, unless some recurring misconception needs active correction.

<!-- DOs/DONTs vs only DOs vs good/better/best? -->

Expose the intention > explain the behaviour > describe the properties
Illustrate with tokens: tool for spec & governance > capture design decision > json kvp

split between long form and quicker tips/conventions

+notion of it has to be simplified, caricatural, true enough to not suspend disbelief etc; in writing or illustrating

### 1.2 Morphology

could it be a list, a comparison table, a data table, a diagram, a reference ppt? *Make a super clear, super big decision tree for "how to shape your content/here's a boilerplate" depending on the deliverable. Eg best practices page: start from a must/could/should bullet list, etc.*

If text:

Each notion should be one paragraph and one only.
<!-- So it's actually one section -->

Each paragraph should be structured in the same way: first the notion <!-- result/guidance --> expressed in a few words. Then its rationale (optional), best practices (optional) and alternatives (optional). <!-- Further reading (connection to other concepts, perspectives, controversies, details etc.) -->  
everything but the idea is optional since in a lot of cases, the instruction standalone can be acted upon immediately, even if somewhat less effectively, while explanations can be added later. Thus trading depth for breadth allows for a quicker "initial overview".
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

Avoid synonyms, especially in domain-specific matters, as well as fuzzy terms and everything-buckets.

Replace or clarify terms that could be interpreted in different ways. E.g. it is not clear if an “alert” is about an error message, a business rule, a push notification or an exception indicator.

Avoid fuzzy spelling, e.g. “dropdown” vs “drop-down” vs “drop down”.

When referring to existing content, such as a UI or a diagram, spell commands, labels or messaging exactly as they appear in situ.

Everything-buckets are ill-defined terms that don’t really describe anything, such as “framework”. Their looseness often provide the appearance of agreement, to the detriment of actionability. Spot them and replace them with clearer explanations.

### 2.3 Tone & Voice

For descriptions, use the present tense and the active form (“Selecting a value triggers validation”).
For instructions, use the second person imperative (“Remove test set”).

Prefer positive wording, and direct statements to what's true rather than what's false.  
It's quicker to check what's true rather than what's false.  
Use negative wording for prohibition or to correct misconceptions.

In any case be assertive, impersonal and use the [singular *they*](https://en.wikipedia.org/wiki/Singular_they) form.

<!-- Faire porter les énoncés sur ce qui est vrai plutôt que sur ce qui est faux (dans les tâches de vérification). Raison: on est plus rapide à vérifier ce qui est vrai que ce qui est faux. -->

### 2.2 Attribution

dont reinvent the wheel for nothing ; check for prior data
authoritative / verified / quality (in data, in presentation) sourcing
<!-- Heh == prefer authoritative data -->
<!-- Sourcing is a whole other topic -->

Always give proper attribution: inline, in footnotes, or in a dedicated section. In the format that's demanded in the readme or license.

format for inline (text or pic) or reference attribution

verify authorized usage

### 2.4. Formatting

<!-- Heh pas terrible, c'est plutôt "conventions et finitions" -->

#### 2.4.1 Style Conventions

Use **strong** styling for keywords. *expand with dod material*

If typographic emphasis is used, it shall be boldface type.

title case for headings

avoid parentheses. use commas or rephrase.

<!-- Un titre d’activité ne contient pas de verbe d’action afin de ne pas le confondre avec une étape. -->

explicitly declare normative vs non-normative sections

Preferred date/time format, numbers format etc

Ponctuer les éléments de liste. D’un point s’il s’agit d’une phrase complète, ou de plusieurs phrases. De virgules le cas échéant. L’avant-dernier élément sera complété par “et” ou “ou”, et le dernier élément terminé par un point.

Numbers representing quantities of 10 or more shall be expressed in numerals ; those representing quantities less than 10 shall be expressed in words. If a number is the first word in a sentence, it shall be expressed in words.

#### 2.4.2 Typographic Signs

Be mindful about typographic signs.

Use proper apostrophes and quote marks ([smart-quotes-plus package](https://atom.io/packages/smart-quotes-plus)), multiplication signs, etc.

- [Glyphy](https://www.glyphy.io/) (e.g. ·, ↪, ⚠)
- [Subscripts and superscripts](https://en.wikipedia.org/wiki/Unicode_subscripts_and_superscripts) (e.g. ⁿᵈ, ⁴)

Conventions:

- e.g.
- etc.
- i.e.

#### 2.4.3 Foreign Words

Italics, translation right after in parentheses.

<!--BREAK-->

## 3 Illustrating

### 3.1 Usage

When/what to illustrate: covers/back covers for style, caricatured examples for trainings, charts-instead-of-text, etc.

Illustrate profusely. At least an illustration every 3-4 slides. They help keep reader interest.

Always associate illustrations directly to the content they support, e.g. floated right.

Make sure full-page illustrations are commented in *presenter's notes* (see xxx) as otherwise they lack the context required to be useful.

Don't illustrate bad practices. In the rare case a bad practice has to be depicted, always depict the corresponding good practice immediately next to it.

### 3.2 Style

Consistent pictorial style. All comparable figures in a document shall be prepared in the same style, for example, all line drawings, or all photographs.

[moodboard](https://www.pinterest.ca/nwodtcobalt/uxa/)

### 3.3 Format

Force bg

preferred layouts/grids (explain grid logic + show grid templates)

preferred sizes & form factors (incl scales and common multiples of 8 and 10)

export @2x

### 3.3 Examples

*florilège annoté*

<!--BREAK-->

## 4 Deckset & Marked Minutiae

`<!--BREAK-->` right after the h1 for Marked document covers

<!-- Major divisions of the document should begin on right hand-pages. Right-hand pages shall be odd-numbered pages, and left hand pages shall be even-numbered pages. -->

<!-- A user document shall have a table of contents unless it has fewer than three divisions or fewer than six pages. A table of contents shall include: (a) at least two levels of the headings and subheadings of the document, (b) appendixes if they exist, (d) list of exhibits, illustrations, figures and tables if they exist, and (e) the original page number of each item listed. The table of contents shall begin on a right-hand page. -->

format deckset presenters notes (they render formatted on deckset and on github

People can’t remember more than 3 points from a speech. (KK)

<!--BREAK-->

## 5 Naming Convention & File Organization

<!-- Split into different document ? -->

Naming schemes ? esp for artboards

Names: case sensitive, no spaces (within a project, not between projects)

<!--BREAK-->

## 9 Credits/bibliographie

- Règles rédaction de Foulon
- HFDS 2003
- IND6408
- [Swift API Design Guidelines](https://swift.org/documentation/api-design-guidelines/)

<!--BREAK-->

# Under Consideration

Check out:

- Handbook / IND6408
- <https://www.smashingmagazine.com/2021/10/resources-tools-turbocharge-copywriting-skills/>
- <https://polaris.shopify.com/content/grammar-and-mechanics#basics>

TBD:

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
