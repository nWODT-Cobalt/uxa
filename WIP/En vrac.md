# En vrac

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

[Formal grammar](https://en.wikipedia.org/wiki/Formal_grammar)

Insertion non linéaire

commutativity, associativity, and distributivity

Conceptual Integrity:

- As few concepts as possible (in words or pictos)
- Explicitely mentioned/depicted (no silent nor black box notions)
- Single representation thereof
- As few exceptions as possible

*Example comparing rows of toggle vs a silly implementation with radios, checkboxes, dropdowns, labels on the left or on the right, etc. Or something not UI related?*.

# Pratiques et concepts

*Applicables au-delà des design systems, mais pas fonctionnel unitairement.*

## The \#1 architectural mistake

<https://twitter.com/kimgoodwin/status/1249802017301598208>
<!--date d'ajout : 19/04/2020-->

I think the \#1 architectural mistake I see on software teams is failure to articulate the conceptual data model before building things. What are the meaningful objects, how do they relate, and what can users do with them? It’s a small investment for huge dividends.

## What I have learned at Google as a designer

<https://medium.com/google-design/what-i-learned-at-google-as-a-designer-7e3a12b7a82e>
<!--date d'ajout : 16/05/2018-->

Learn to articulate ideas using vocabulary of abstraction and system design. By describing your approach in a different terminology, you can help people think about reusability and repeatability of patterns and solutions. You can help them construct a mental model that can be re-applied to different situations and not just remain limited to solving the individual problem at hand. A large part of systems thinking is coming up with these reusable mental models that help reduce maintenance overhead.

## GitLab Values

<https://about.gitlab.com/handbook/values/>
<!--date d'ajout : 05/04/2018-->

Boring solutions: Use the most simple and boring solution for a problem. You can always make it more complex later if that is needed. The speed of innovation for our organization and product is constrained by the total complexity we have added so far, so every little reduction in complexity helps. Don't pick an interesting technology just to make your work more fun, using code that is popular will ensure many bugs are already solved and its familiarity makes it easier for others to contribute.

## Should it be a pattern decision tree

<https://coggle.it/diagram/V0hkiP976OIbGpy8>
<!--date d'ajout : 18/03/2018-->

## Coding with Clarity

<https://alistapart.com/article/coding-with-clarity>
<!--date d'ajout : 10/12/2017-->

Working code isn’t necessarily good code. Your code also needs to be easy to read, understand, and modify. It needs clarity, and to achieve that, it has to be organized well, with careful planning and proper separation of ideas taking place before you even open your code editor. Coding for clarity is something that separates the great developers from the merely good, and there are a few basic principles that can set you on that path.

**The single responsibility principle**

The single responsibility principle states that a block of code should do one thing, and do it well. If you’re describing what a function does and you have to use the word “and,” that function is probably too complex.

**Command-query separation**

Functions fall into one of two categories: *commands*, which perform an action, and *queries*, which answer a question.

A good rule of thumb is that if your function answers a question, it should return a value and *not* alter the state of the data. Conversely, if your function does something, it should alter the state of the data and *not* return a value.

**Loose coupling**

*Coupling* is a measure of how much one program unit relies on others. Too much coupling (or tight coupling) is rigid and should be avoided. That’s the jigsaw puzzle. We want our code to be flexible, like Lego blocks. That’s loose coupling, and it generally results in much greater clarity.

Classes that interact with each other can also be culprits of tight coupling. You shouldn’t have to modify a class because another class changes. Constructor parameters can be passed as an object with the receiving object having fallback default values, which loosens coupling and means code won’t break when you add new parameters.

**High cohesion**

*Cohesion* is a measure of how much the various different program units belong together. A high level of cohesion is good and adds clarity to code blocks; a low level of cohesion is bad and leads to much confusion.

Repeated code is a sure sign of low cohesion. Similar lines of code should be broken into functions, and similar functions should be broken into classes.

## Keep a Changelog

<http://keepachangelog.com/en/1.0.0/>
<!--date d'ajout : 18/03/2018-->

*Et [Semver](https://semver.org/) et <https://speakerdeck.com/apistrat/api-versioning-at-stripe>.*

## How To Be More Organized While Designing UI

<https://medium.com/@tristanminor/how-to-be-more-organized-while-designing-ui-90d2d69cfb4f#.tx5dev9u3>
<!--date d'ajout : 23/04/2016-->

*Brouillon mais a le mérite de fournir des illustrations intéressantes.*

- Clear Overview Of Variables
- Grouping Of Styles
- Pairings of Variables
- Everything Is An Object
- Properties for Everything
- Inheritance Of Properties

Imagine a node based editor (something like Mindnode) in which you can see and maintain the visual relationships of your projects. It would be able to read SCSS files and connect to Sketch to update your shared styles.

## OOUX: A Foundation for Interaction Design

<http://alistapart.com/article/ooux-a-foundation-for-interaction-design>
<!--date d'ajout : 20/04/2016-->

*Très intéressant, mais a priori plus pour les systèmes complets et "nouveaux". Voir comment faire le lien au mieux avec les flux de tâche/scenarii utilisateur.*

>The “metaphor,” once found, is a perfectly definite thing: a collection of objects, actions on objects, and relationships between objects.

>–Dave Collins, Designing Object-Oriented User Interfaces (1995)

In retrospect, I feel like I was doing my job backwards for the first two-thirds of my career, putting interaction flows before building an object-oriented framework. Now, I would figure out the system of chefs, recipes, and ingredients before worrying about the chef onboarding process or how exactly a chef posts a recipe. How do the objects relate to one another? What content elements comprise each object? Which objects make up my MVP and which objects can I fold in later? Finally, what actions does a user take on each object?

*Bon point. Un des buts serait de parvenir à designer les gabarits/composants avant les pages, plutôt que de les inférer depuis celles-ci.*

![](http://alistapart.com/d/ooux-foundation-for-interaction-design/BridgeDiagram221-07.jpg)

By using the object framework, I might uncover functionality I wouldn’t otherwise have considered if my brainstorming was too broad and unconstrained; structure gives creative thinking more support than amorphous product goals and squishy user objectives.

You can user-test your system of objects and the actions a user might take on them before spending long hours on interaction design. Create a prototype that simply lets users navigate from one object to another, exploring the framework (which is a significant user goal in itself). Through observation and interviews, see if your system resonates with their mental model. Do you have the right objects and do their relationships make sense? And are the right “buttons” on those objects?

Armed with a simple prototype of your interconnected objects and their associated CTAs, you now have a platform to discuss functionality with users—without all the hard work of prototyping the actual interactions. In a nutshell: talk to your users about the button before designing what happens when they click it.

![](http://alistapart.com/d/ooux-foundation-for-interaction-design/after_object_map_vertical2x.jpg)

*De son [article précédent](http://alistapart.com/article/object-oriented-ux) :*

Newsflash! This is how your backend engineers work. In the ’80s, the software engineering community began to transition from procedural languages to object-oriented languages, which have benefits like code reuse, data encapsulation, and easier software maintenance. Most programmers bring your designs to life using object-oriented languages like Java, Ruby, Python, C++ or C#.

Engineers start their process by mapping out the objects that make up the problem domain—something UXers should be doing from day one. When they look at your wireframes or prototypes, they first reverse-engineer your design to parse out the objects. They think, “How will object X talk to object Y? Will object A be made up of lots of object Bs? Which attributes will each object have? Will this class of objects inherit from that class of objects?”

On the web, we develop object-orientedly, but still design procedurally, focusing on drill-down hierarchy or linear task flows.

Content modeling. To extract the objects, we basically highlight the nouns [from the brief]. Recognizing nouns is first-grade simple, but extracting objects does require some subtle art *(et explication)*.

## Work Smarter: Object-Oriented User Experience Design

<!--date d'ajout : 22/02/2015-->

Think about how computer programs are written. Years ago, all computer programs were written into a flat file. They combined data, interface calls, and processing all in one long program.

After a while, programmers realized that this was very inefficient. There was no opportunity for re-use. Eventually, they moved into object-oriented coding. They began to write pieces of code which could work in different situations. They defined data and functions which could be used repeatedly, under different circumstances. This is much better than re-writing everything specific for each program. By separating out the subroutines, they became more capable of maintaining the code with greater ease.

This was an enormous change in the software field. There is nobody who would ever think about going back.

Decades later, we're looking at doing the same exact thing in the UX field. We have the exact equivalent of writing flat file code. For many of us, when we do a project, what comes out is a document or slide deck. At the end of the day, everything that we know and learn is jumbled up inside these documents. If you want to work in this design space, a lot of time is spent looking through the documents and pulling out everything we might know about a user type, scenario, or environment. It's a jumbled mess.

If we change the way we work from thinking about our output as just a single document and instead break that output into its components, then we can stop re-doing those objects over and over again. We can make it easy for people to find and work with them, and create much more efficiency.

Now, the first time you do this it's not going to be any faster. But, once you've done it for a while, you end up having an environment of shared models. You end up with shared standards, project content, customer models, scenarios, ecosystems, and so on. That allows us to do our work in a faster, better, and cheaper way.

Object-oriented UX is about working smarter. It's about working in a way which is in fact faster, cheaper, and better. I think, in the future, we'll find that all UX professionals will work, not based on ad hoc memories they have from different projects, but from a shared, documented, tool-based environment that allows them to manage these objects.
