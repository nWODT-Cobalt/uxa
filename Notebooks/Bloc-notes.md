## En vrac

Prioritize learning over delivery
Every decision you make is a hypothesis

at scale, all edge cases are common

Design systems extension ideas: design IDE, bidirectional integration with dev IDE, visual & behavioral regression testing, self-service 3rd party integration (to be broken down), design APIs, theming (not just colors but scale factors, hardware factors, ui form factors etc), integrated telemetry, task patterns, etc.

Functionalism: design for function and it will be beautiful *(pwoooo risqué)*

Makers tend not to lead because they are busy making

Rather than being a dictionary of shapes, it’s a dictionary of methods

From the Wikipedia page on Composability:

>A highly composable system provides recombinant components that can be selected and assembled in various combinations to satisfy specific user requirements. In information systems, the essential features that make a component composable are that it be:

>- self-contained (modular): it can be deployed independently – note that it may cooperate with other components, but dependent components are replaceable
>- stateless: it treats each request as an independent transaction, unrelated to any previous request. Stateless is just one technique; managed state and transactional systems can also be composable, but with greater difficulty.

## Pour axiomes

Specialized understanding = gatekeeping

An easy-to-learn API features consistent naming conventions and patterns, economy of concepts, and predictability.

Each deliverable is a micro DSL

Reuse from the get-go, meaning *always* turn it into a deliverable. At least:

- Title (both decent file name, if not complete scheme, and on-pic title)
- Expand from an example to a rationale if possible
- Share/publish/version etc

Predictability, generativity/predictivity, decidability (hard pass/fail). repeatability, accuracy, efficience, opposite of inference ("expliciteness"), "lean fit"
functions not dictionnaries: <https://matthewstrom.com/writing/functions-in-design-systems>
thats what being systematic means, hence why it can't just be added afterwards

## Matériel pédagogique WIP

### Components

Investigate modes *(pour DoD de composant)* : Edition, data saving, failure, loading, initial state, empty state, etc. +min, max, reasonable/expected, recommended

base components should only accept enumerable parameters

### Writing and Maintaining Documentation

And remember — if it isn’t documented, it doesn’t exist.

Show structure before behavior, and behavior before layout.

The customer journey is a fluid mix of intentions, contexts, tasks and ever more dynamic screens. Documentation should capture and encourage working in terms of complete flows, not just successions of static screens. Given finite resources, it means starting from structure rather than layout.

Our best solution yet is to approach documentation with an editorial mindset, carefully composing a narrative for each page, curating what content to expose, and supporting it with purpose-made illustrations.

Allocate the most real estate and details for primary use cases.

Maintaining current pages is as important as adding new ones.

Content naturally becomes irrelevant over time; it’s our job to make sure that our colleagues find what they’re looking for nonetheless.

Quick fixes here and there, larger reorganizations when appropriate and sunsetting content from time to time ensure everyone remains on the same page.

Make sure only meaningful revisions are archived locally and on Mojo; get rid of the minimal or redundant iterations

### Publication Status & Change History

Enter any pertinent information in the prompt if you feel the changes are significant.

As such, it is preferable to expose pages only when their content is high quality. This way, it is possible to work on major new features or improvements in the backstage, without disrupting the experience of the reader.

Reviewing our content together builds consensus, allows for better solutions and keeps everyone in the loop. Conversely working in isolation often leads to inconsistency, rework, and poor communication inside and outside of the team. It’s thus preferred to discuss major changes before pushing them; see previous point to for how to work with Confluence drafts.

### Misc

Insertion non linéaire

commutativity, associativity, and distributivity

Conceptual Integrity:

- As few concepts as possible (in words or pictos)
- Explicitely mentioned/depicted (no silent nor black box notions)
- Single representation thereof
- As few exceptions as possible

*Example comparing rows of toggle vs a silly implementation with radios, checkboxes, dropdowns, labels on the left or on the right, etc. Or something not UI related?*.
