*About components*
*On components*
*reading notes — components*

so as to remain differentiated from original content

## Component API

<https://github.com/mrmrs/component-api-talk>
<!--date d'ajout : 18/03/2018-->

*~N'exposer que les propriétés pertinentes et attendues pour chaque composant HTML (e.g. button) plutôt que de permettre d'écrire tout le CSS. Très bien argumenté.*

## Component QA

<https://github.com/viljamis/vue-design-system/wiki/Component-QA>
<!--date d'ajout : 18/03/2018-->

- Sufficient States & Variations
- Content Resilience
- Composability
- Etc.

## Components

<https://jxnblk.com/blog/components/>
<!--date d'ajout : 26/07/2017-->

From the Wikipedia page on Composability:

>A highly composable system provides recombinant components that can be selected and assembled in various combinations to satisfy specific user requirements. In information systems, the essential features that make a component composable are that it be:

>- self-contained (modular): it can be deployed independently – note that it may cooperate with other components, but dependent components are replaceable
>- stateless: it treats each request as an independent transaction, unrelated to any previous request. Stateless is just one technique; managed state and transactional systems can also be composable, but with greater difficulty.

A UI system that is made up of independent stateless components is extremely flexible. When individual pieces need to be swapped out or updated, those changes are isolated and don’t cause other parts of a system to break.

Naming things is hard, there’s no debate there, but when you start to categorize different parts of a UI into pages, views, flows, atoms, molecules, materials, or kittens, you’ve already started to undermine the concept of composability, and it probably takes more time and effort to get an entire team of people to “agree upon” your proposed naming conventions than it’s worth.

The point of this is to think about everything as an interoperable system. You can slice and dice components in any way you see fit, and these components are likely to change and be fine tuned as a system is developed. Premature optimization is a trap that’s easy to fall into. Embrace the chaos as you build. Patterns will emerge from the primordial goop of UI that is your product, and by consistently thinking about a composable system you’ll probably come up with something more flexible and more robust than if one person dictates a dogmatic framework to work within.

## Buttons in Design Systems

<https://medium.com/eightshapes-llc/buttons-in-design-systems-eac3acf7e23#.asm44ei4r>
<!--date d'ajout : 27/04/2016-->

*Décompose avec pédagogie les attributs et états possibles d'un bouton en apparence ordinaire.*
