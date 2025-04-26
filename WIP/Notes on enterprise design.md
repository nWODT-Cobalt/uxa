# Notes on enterprise design

<!--BREAK-->

## Overview

<!-- Boo! Better titles/outline -->
<!-- streamline and define terminology, esp “enterprise design products”, end-users vs employees vs individuals etc -->

“Enterprise design” is a design practice targeted at enterprise rather than individuals customers.
It’s for example the business of Dassault, IBM, Oracle, Salesforce, SAP, ServiceNow etc.

Enterprise design has different goals, business models, metrics, roles, audiences, tools, engagement, culture, practices etc than consumer product design.

This document is an early mind sweep, that may eventually grow into proper reference material.
For now it can be helpful for designers curious about the enterprise design space, as training material, interview framework or conversation support.

<!-- more complete, nuanced definition: -->
<!-- could also be “institutional” or “organizational” design, to account for gov work, NGOs, associations etc -->
<!-- Define B2B vs enterprise design vs UXA vs SuiteX vs B2B vs B2C vs… -->
<!-- “the customer isn’t the user” -->
<!-- NB different from “productivity”. Some productivity is B2C eg office vs google docs vs iwork, or self accounting software, or Trello etc -->

<!-- only describes ecological context; doesn’t offer a practice to solve for it -->

This first version has been generally simplified to large SaaS companies with thousands of employees, including dozens of designers.

<!-- - technically could be on prem, hybrid native etc -->
<!-- - (technically could be small orgs) some B2B apps have a very small scale (eg medical tools) some B2C products have a very large scale (eg social networks) -->
<!-- - Scale comes with its own set of considerations “eg at scale, all edge cases are frequent” *heh, not germane* -->

## Notes

<!-- What a messy outline. Structure better. Causes-consequences? Topics? -->
<!-- in any case, eventually derive actions (if not a process) for designers -->
<!-- TOC as a TL:DR? -->

**The customer isn’t the user**

<!-- The single biggest difference between consumer product design and enterprise design is it’s foundational definition: the fact that the customer isn’t the user. -->

Enterprise design products are selected at the executive level (e.g. by the CIO[^cio] or CTO[^cto]), then used by the rest of the company. In other words, they are

Whereas employees may care about speed, ease of access, ease of use or personalization, enterprise buyers will rather look at  TCO[^tco], security, scalability, compatibility or compliance. They will consult with legal, brand or technical experts, pushing further away personal considerations.

<!-- Managing multi-persona dynamics

For me, that meant designing mostly for the security engineer (the user) but delivering enough value to the Chief InfoSec Officer (the buyer) for them to see it was worth spending hundreds of thousands or millions of dollars per year on our product. In some cases, other third-party employees could torpedo the sales process too (like if a CTO or Chief Architect decided they didn’t want to accommodate our architecture). -->

[^cio]: Chief Information Officer
[^cto]: Chief Technology Officer
[^tco]: Total cost of ownership

**Users are experts**

The users of enterprise design products are likely to be a professional audience, experts in their field.

Deep knowledge, strong opinions. Designing for them means internalizing a lot of domain knowledge.

This isn’t necessarily the same as being tech-savvy or computing experts. E.g. just because a surgeon has great medical proficiency doesn’t mean that they know all of Excel’s shortcuts.

**The ecological environment is controlled**

Devices and apps are company-provided and controlled.

Personal devices may not be able to be brought in the workplace (e.g. nurses or retail staff leaving smartphones and smartwatches in the locker). Software outside of a very restrictive allowlist may not be installed. Many sites, apps or services may not be allowed on a monitored network.

<!-- Identity too (SSO) -->

In extreme cases, devices can be air-gapped into LANs[^lan] without Internet connection. Hardware too can be locked down: tin cast into ports, computer physically bound to furniture or wall.

<!-- huge impact on MFA, CDN, releases etc -->

[^lan]: Local area network

**Enterprise products are configured**

Enterprise products are usually highly configurable in order to support business processes, regulations, topologies etc.

<!-- For a product to be configured, it needs be configurable. A huge area of design on its own -->
<!-- == no two instances will be the same, design and deliverables for modularity etc -->

System admins will work hand-in-hand with the vendor to initially deploy the product, and will then maintain and extend it on their own. User access, security, business rules etc will drive who can access what, and how.
End-users may still be able to set their own preferences. If they exist, they will be downstream of layers of company-driven decisions.

[The parameters potentially affecting what end-users have access to. Each a subset of the previous one.]
| Name          | Description                                                                                | Owner              |
| ------------- | ------------------------------------------------------------------------------------------ | ------------------ |
| SKU           | Product mix subscriptions, modules purchased. <br> Legal agreements and restrictions.      | CIO, COO           |
| Configuration | Customer-wide setup: what is enabled, disabled, deployed, created or customized; for whom  | Admins, IT         |
| Tenant        | Configuration at a local level, for a particular org, business unit, geography or location | Manager, directors |
| Preferences   | Personal, work or convenience settings                                                     | End-users          |
| Context       | Day-to-day, business- or task-specific factors                                             | N/A                |

<!-- Move to a/the “configuration in enterprise” note -->

**Acquisition/implementation is difficult**

- Implementation costs are huge for the customers, in money, time, expertise, trust
    - As a result, so are switching costs
    - As a result, stickiness
    - As a result, reputation is key
    - Much higher cost of error / favors “nobody gets fired for buying IBM” / low risk-taking (on both sides)
- high barrier to entry
    - Another reason why good design is less found in large enterprise software is because the barrier of entry to building something useful for B2B is a lot higher than B2C. You usually need a certain amount of industry knowledge and experience to create any semblance of a useful / usable product. Also B2B often needs a lot more features to be “sellable,” plus a sales engine. This already weeds out a lot of potential founders, willing investors, and thus good options in the market.

- Active sales process, sales teams
    - VS “just” online marketing, word of mouth, virality etc
    - Long standing relationships
- some features/product can be built for a single customer, if big enough
    - much more customer-driven, vs ~gut/vision driven innovation

**Different “voice of the customer” (to/from)**

- Design wasn’t the sole “voice of the customer.” We had entire teams in professional services and customer success who were in constant contact with users and whose job it was to represent their needs. This shifted my focus to be more on leaning into those relationships, interpreting the constant flow of feedback, and synthesizing it into smarter design choices.
- dedicated research roles/team
- customers only partially convey needs of users
- the issue you’ve identified goes beyond product design and product experience into feature prioritization
- Real, human support
- Support/expert communities

**Change is difficult**

- High-stakes design changes
    - The stakes of making changes were very high. If we made a poor design decision that resulted in a major error it could take down our customer’s systems (and the other businesses that depended on that company’s services). This meant we needed to “measure a hundred times to cut once” and be very deliberate in our prototyping and rollout process.
    - Change management
- Higher value on reliability/~“stability over time”
    - Since users *rely* on the service, for doing their job or running their business, as opposed to consuming it for entertainment or as their optional volition
    - Often captured in contracts/SLAs; contractual agreements, levels of service, levels of uptime, legal liability
- Testing is “managed”
    - No live A/B testing etc
    - But beta programs in partnership with customers
    - feature flags / feature toggle
    - launching darkly
- difficult to know what to change, difficult to actually proceed with the change, to iterate
- the org may not be set up for or interested in agile follow-up anyway

**Older, mature, sticky tech stacks**

- Concurrent/Backwards compatibility
- Low key a hindrance to progress
- Eg COBOL for banks or secure languages for rigs or the military
- But really, the same characterization for all aspects of the org

**Lesser design culture/outcomes**

- Lower emphasis on design overall
- At least on interaction design/visual design as understood nowadays; or for clouds/apps applications
- Because there could be a lot of HFE work by public (powerplants in Europe) or private sector (eg Bell, CAE)
- design org not well considered/involved
- np “design founder” here, possibly not even at the first 1-2 execs level

**Different success metrics**

- The business metrics are different (eg PEPM, net dollar retention, retention, churn)
- subs,  not ads

**Regulatory Compliance**

<!-- Legal Frameworks -->

Regulatory compliance is much more prominent in enterprise than in consumer design.

Because of the demanding audience, criticality of service, engagement with government or just sheer scale, regulations are either enforced or assessed as likely to be: localization in countries of operation, privacy laws such as GDPR, accessibility laws like WCAG, etc.

Most verticals add their own standards like ISO 9341, ISO 1347, ISO 16290, NF EN 1325, MILSTD, ICAO or IATA norms etc.
Sometimes not *de jure*, but nonetheless *de facto*.

**The best branding is no branding**

- Brandability, Themeability, customization, White-labeling
    - some customers will have deep customization/deviance, and will tend to produce more content/transactions then B2C products, where user input is minimal or heavily controlled
- 3rd party integration, 3rd party support (composing, being composed)
- the product isnt a brand of its own, rather it must support the customers brand (eg the exact opposite of Dropbox, Spotify or Steam)
- technicakky it has a brand, but there again it is geared towards its enterprise customers (being reliable, configurable, feature-rich, etc) rather than individuals/end-users (where it’d have to be enticing, easy to use, differentiated, etc).

**Frontstage vs. Backstage Customer opportunities**

design can be at another level than “the app”

a wider surface area

<!-- eg configuration, administration, multi-actor workflows/orchestration; any interface thereof -->

<!-- business workflows, business processes, automation, administration etc: missing a whole section on the “actual business” side of things!-->

---

*Some items from [7 Insights for Navigating B2B Design](https://www.unknownarts.co/p/7-insights-for-navigating-b2b-design).*

<!-- **subsequent practice**

UXA signals, à voir

Relevant signals

- Deliverables
    - Flowcharts (a lot of them), decision trees, state charts
    - Entity-relationship diagrams, domain models
    - Tables & matrixes of all kinds, rich lists
    - Templates of all kinds (Figma, wiki, plain text, YAML, JSON, md)
    - Reference material of all kinds (ditto)
- Activities (and proof thereof, e.g. through the deliverables above)
    - Pitching to leadership, training to contributors, advocacy to all
    - Governance, guidance, office hours
- Keywords
    - Modular, composable, interface, interplay
    - Parameters, attributes, properties, configuration
    - Services, frameworks, platforms, orchestration
    - Patterns, emergent behaviors, rules & relationships
    - Terminology, ontology, taxonomy
- All of it packaged
    - As living artefacts
    - Geared towards a product-design-dev audience, not just a dev one
    - With clear delineation of responsibilities (what’s owned by “the platform”, what’s opened to or expected from “partners”)
- Business processes
- Composability
- Configurability (wide and deep, from component props to full-on admin areas)
- Interfacing
- Modularity
- Multi-channeling
- Orchestration
- Platforms
- Portability
- RBAC
- Brand
- Frameworks
- Internationalization
- Interplay
- Platforms
- Scalability

At a higher level:

- Co-strategy
- Governance
- Partnerships

Irrelevant signals

- Keywords like information architecture, card sorting, visual hierarchy, design systems, patterns
    - Those are table stakes, and not indicative of an architectural practice
    - Especially when design systems are “tokens and components” rather than patterns, frameworks, screen flows, utilities, usage guidelines etc.
    - Especially when patterns are “big components” rather than “abstraction of a solution”
- Mentions of “strategy”, “scalability”, “consistency”, “reuse” without further details
- Layout
- Responsiveness
- Style
- Perceived quality
- Perceived novelty

(They are still there, but their relative importance is lower) -->
