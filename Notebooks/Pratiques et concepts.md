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

# Élicitations et rédaction de principes

## Exemples

*En sus de ceux inclus dans les design systems:*

- [La charte des « Décodeurs »](http://www.lemonde.fr/les-decodeurs/article/2014/03/10/la-charte-des-decodeurs_4365106_4355770.html)
- [Gravity](https://medium.com/buildit/introducing-buildits-gravity-design-system-44c3fe7a1d26) (Inclusive , Lean, Robust, Considered , Progressive)
- [Linear Method](https://linear.app/linear-method)
- Lyft
	1. Nail the basics (Clear choice & context)
	2. Build confidence (Consistent & transparent)
	3. Be unique (Ownable & delightful)
- [Paste](https://paste.twilio.design/principles)

## Fredrik Matheson

<https://twitter.com/movito/status/1028548828931272705>
<!--date d'ajout : 19/08/2018-->

“A principle isn’t a principle unless it costs you something” — Bill Bernbach

*En commentant un tweet de Jared Spool :*

Values worth sticking with are only meaningful when they are hard to execute. If they are always convenient and easy, they aren’t values. They are just good practice. Values are the things we do when the wrong thing is easier and more lucrative.

## Creating Great Design Principles: 6 Counter-intuitive Tests

<https://articles.uie.com/creating-design-principles/>
<!--date d'ajout : 23/06/2018-->

It’s easy to separate a good design from bad designs. A great principle helps you distinguish a great design from the good designs.

- Test 1: Does It Come Directly From Research?
- Test 2: Does it Help You Say ‘No’ Most of the Time?
- Test 3: Does it Distinguish Your Design From Your Competitors’?
- Test 4: Is it Something You Might Reverse in a Future Release?
- Test 5: Have You Evaluated it for This Project?
- Test 6: Is its Meaning Constantly Tested?

*Easy to use* is not something that will ever set a competitor apart. However, *Focus on polish before new features* could set your design apart from a competitor trying to win the hearts and minds of customers through new features, even though their existing platform is buggy and convoluted.

## Web App Masters: Design Principles

<http://www.lukew.com/ff/entry.asp?1364>

How do we tell if our designs are getting better? We need way to evaluate them. Design principles embody a design philosophy and help teams get to better design decisions.

Design principles provide abstract guidance about how to make decisions. Dieter Rams was one of the first to apply design principles to his work.

Google and Facebook have very similar high-level design principles (useful, fast, simple, human) but these principles are so broad that they are almost useless.

Companies use generic principles because they are the only things people can agree upon. Who would argue that “fast” and “universal” are not good principles? As a result, these generic principles show up a lot.

The problem with really long lists of principles is that no team can keep them all in mind as they go through the design process.

Good design principles are specific and not overly extensive.

Design principles should not be common. They need to be specific to what you are trying to accomplish.

There are six questions that you can use to evaluate your design principles.

- Does the design principle come directly from research? What kind of research finds principles like “clean” and “universal”? None. Knowing the observations that led to principles is makes them actionable.
- Does this principle allow you to say “no” most of the time? We need to get rid of good designs. We need to get to great designs.
- Does the design principle distinguish your design from your competitor’s designs?
- Have you evaluated the design principle for this project?
- Is this design principle something you might want to reverse in a future release? If we can imagine effective designs that don’t meet our principle. That’s how we get to great deigns from good designs.
- Is the design principle’s meaning constantly being tested?

## What makes a good design principle?

<https://matthewstrom.com/writing/principles>
<!--date d'ajout : 03/01/2018-->

- Good design principles are memorable
- Good design principles help you say no
- Good design principles aren’t truisms (a good test of truism is the reversibility test)
- Good design principles are applicable

A shortcut to good principles: "Even Over" statements

*Réminiscent du « pour savoir si un terme est vide de sens, il faut chercher son contraire. Personne ne voudrait par exemple s’appeler A l’arrêt », dans  [Pourquoi les partis politiques se prennent de passion pour le point d’exclamation](https://www.lopinion.fr/politique/pourquoi-les-partis-politiques-se-prennent-de-passion-pour-le-point-dexclamation).*

## A Matter of Principle

<https://medium.com/the-year-of-the-looking-glass/a-matter-of-principle-4f5e6ad076bb#.crmh0x42x>

*Principles can answer stakeholders or devs more efficiently than factual points thrown at each and every question they have.*

A good set of design principles, on the other hand, does the following:

1. Helps resolve practical and real-world questions around specific design decisions.
2. Applies to an entire class of design decisions, both things we can think of today, as well as questions that will pop up in the future.
3. Imparts a human-oriented sense of “why?” that is easy for everybody — including non-designers — to understand.
4. Has a point of view and a sense of prioritization that a rational person could disagree with.
5. Is generally paired with illustrative examples that show how the principle applies to specific decisions.

Instead of relying on gatekeepers to keep a high quality bar, better instead that everyone gets to agreement on a smaller set of guiding values, so that the best decisions get made in a consistent manner, scaling across many decisions, and even many designers.
