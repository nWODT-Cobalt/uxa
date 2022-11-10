# Reading notes on design principles

<!--BREAK-->

*Most design principles tend to be consensual statements of good intentions, read once and instantly forgotten as they’re of no use day-to-day.*
*This document tracks best practices for eliciting and writing useful principles.*

## Zack

<!--date d’ajout : 18/06/2022-->

The purpose and consumers of the contents need to be clarified first. How far you would like the principles to impact your internal orgs? Is it for [UX-internal] educating or align stakeholder expectations? Establish a common language in the whole company?

Product Design [can be] a supporting org/subset of Prod Dev, so PM and Dev are involved in signing-off. The principles need to be widely-relatable/educable so that they actually accelerate the buy-in process. Something to watch out for to manage stakeholder expectations.

## Fredrik Matheson

<https://twitter.com/movito/status/1028548828931272705>
<!--date d’ajout : 19/08/2018-->

Bill Bernbach:

>A principle isn’t a principle unless it costs you something

Jared Spool:

>Values worth sticking with are only meaningful when they are hard to execute. If they are always convenient and easy, they aren’t values. They are just good practice. Values are the things we do when the wrong thing is easier and more lucrative.

## Creating Great Design Principles: 6 Counter-intuitive Tests

<https://articles.uie.com/creating-design-principles/>
<!--date d’ajout : 23/06/2018-->

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
<!--date d’ajout : 03/01/2018-->

- Good design principles are memorable
- Good design principles help you say no
- Good design principles aren’t truisms (a good test of truism is the reversibility test)
- Good design principles are applicable

A shortcut to good principles: “Even Over” statements.

*Reminiscent of « pour savoir si un terme est vide de sens, il faut chercher son contraire. Personne ne voudrait par exemple s’appeler A l’arrêt », from [Pourquoi les partis politiques se prennent de passion pour le point d’exclamation](https://www.lopinion.fr/politique/pourquoi-les-partis-politiques-se-prennent-de-passion-pour-le-point-dexclamation) (FR).*

## A Matter of Principle

<https://medium.com/the-year-of-the-looking-glass/a-matter-of-principle-4f5e6ad076bb#.crmh0x42x>

A good set of design principles, on the other hand, does the following:

1. Helps resolve practical and real-world questions around specific design decisions.
2. Applies to an entire class of design decisions, both things we can think of today, as well as questions that will pop up in the future.
3. Imparts a human-oriented sense of “why?” that is easy for everybody — including non-designers — to understand.
4. Has a point of view and a sense of prioritization that a rational person could disagree with.
5. Is generally paired with illustrative examples that show how the principle applies to specific decisions.

Instead of relying on gatekeepers to keep a high quality bar, better instead that everyone gets to agreement on a smaller set of guiding values, so that the best decisions get made in a consistent manner, scaling across many decisions, and even many designers.

## Personal Notes

*An attempt at consolidating the above into an actionable framework.*

Principles are “a fundamental truth that serves as the fondation for a system of belief or a chain of reasoning” ([Julie Zhuo](https://medium.com/the-year-of-the-looking-glass/a-matter-of-principle-4f5e6ad076bb#.crmh0x42x), 2015).

Their point is to support alignment and decision-making, and to a lesser extent creativity.
They can come from external factors (business strategy, market constraints, technical limitations) or internal choices (e.g. brand, personal preferences).

Principles are relevant in several areas of an organization: strategy, gouvernance, marketing etc.
In UX, they can informe entire strategies, new products, big redesigns or specific journeys.
On smaller efforts, they’re not as useful as more straightforward guidelines.

Good design principles are MEMOSPADE:

**Memorable**

Clear, concise and impactful so that they can be internalized, thus generative, rather than referred to, thus conformative.
Use short, unambiguous, and well-illustrated statements. Quantify them when possible.

For example, Android’s “make important things fast”.

**Evolving**

Reasonably iterated upon, to remain relevant as the product grows.
Adjust their substance and scope, especially in the earlier phases when things are still in flux.

For example, Gravity replaced “be universal” with “inclusive”.

**Meaningful**

Impart a human-oriented sense of why, so that they’re memorable and motivating.
Make the rationale interesting to the reader (designers or non-designers) rather than true to the system.

For example, “small things matter, good and bad” from Windows UX.

**Outbound**

Expressed in terms of end-user benefits rather than internal benefits.
Don’t mention tools, technical capabilities or other similar internal properties.

For example, replace “use push notifications” with “keep the user apprised timely”.

**Specific**

Not a truism, indistinguishable from competitors, that doesn’t help making decisions. Replace “always true” statements with opinionated visual preferences, focused guidelines or business idiosyncrasies.

For example, “clarity above all” rather than “easy to use”.

**Prioritized**

Ranked against one another, so as to provide a path to resolution for difficult use cases. Write principles as “x over y over z”, or make an explicit different between must have and nice to have.

For example, as per Salesforce: “clarity > efficiency > consistency > beauty”.

**Applicable**

Can be easily connected to designs, and acted upon. If a statement isn’t actionable it’s a goal, not a principle; principles must support design activities.
Make sure principles aren’t completely abstract, demanding a lot of thinking to be applied to the product. Provide an high-level “how”.

For example, “use shape to communicate actionability” rather than “make controls obvious”.

**Determinative**

Allow to say no, to fairly pick between options. Otherwise the effort devolves into lowest common denominator without style nor conceptual integrity.
Break down big statements into smaller, unambiguous ones. Write down explicitly their known consequences, positive or negative. Quantify if possible.

For example, “single meaning over several meanings” rather than “meaningful icons”.

**Encompassing**

Apply to entire classes of problems, now and in the future; otherwise they’re a pass/fail criteria, not a principle.
Don’t be too detailed, e.g. principles covering one use case each.

For example, “start with smart defaults” rather than “placeholder text in fields”.

<!-- Having more than an handful principles is overwhelming; curate actively. Likewise, not all principles will have to be perfectly MEMOSPADE to be useful. -->

## Examples

Aggregators:

- [Design Principles](https://principles.adactio.com/)
- [Design Principles FTW](https://www.designprinciplesftw.com/)

Misc:

- [La charte des « Décodeurs »](http://www.lemonde.fr/les-decodeurs/article/2014/03/10/la-charte-des-decodeurs_4365106_4355770.html) (FR)
- [Gravity](https://medium.com/buildit/introducing-buildits-gravity-design-system-44c3fe7a1d26), with interesting iterations based on experience
- [Hey Elon: Let Me Help You Speed Run The Content Moderation Learning Curve](https://www.techdirt.com/2022/11/02/hey-elon-let-me-help-you-speed-run-the-content-moderation-learning-curve/), an orthogonal but convincing depiction of iterating on principles
- [Linear Method](https://linear.app/linear-method)
- [Paste](https://paste.twilio.design/principles)
