# Notes on enterprise design

<!--BREAK-->

---

## Context

<!-- Boo! Better titles/outline -->

Who/What's this doc for? A quick reference for B2C people interested in working in B2B. or as a fwk for evaluating ppl during hiring, or as an outline for training etc.
For new designers, or otherwise experienced designers or design managers looking to work in the field.

<!-- Define B2B vs enterprise design vs UXA vs SuiteX vs... -->

<!-- NB different from "productivity". Some productivity is B2C eg office vs google docs vs iwork, or self accounting software, or Trello etc -->

change the goals, role, engagement, value-add and ultimately practice of the B2B designer vs B2C designer

only describes ecological context; doesnt offer a practice to solve for it

"Enterprise design" defined by "the customer isn't the user". Typically JIRA (vs Trello). IBM/SAP?

With great points from [7 Insights for Navigating B2B Design](https://www.unknownarts.co/p/7-insights-for-navigating-b2b-design)

We'll make broad assumptions in this first version:

- Everything has been simplified
- SaaS/cloud/RWA (technically could be on prem, native etc)
- Made by large teams (10+ designers) in large companies (1000+ ees)
    - (technically could be small orgs) some B2B apps have a very small scale (eg medical tools) some B2C products have a very large scale (eg social networks)
    - Scale comes with its own set of considerations "eg at scale, all edge cases are frequent" *heh, not germane*
- Professional, expert audience

## Remarkable attributes

<!-- sort as causes vs consequences and/or in themes legal vs technical vs financial -->
<!-- in any case, eventually derive actions (if not a process) for designers -->

- Managing multi-persona dynamics/the customer isnt the user
    - The distinction between buyer and user is a big one. For me, that meant designing mostly for the security engineer (the user) but delivering enough value to the Chief InfoSec Officer (the buyer) for them to see it was worth spending hundreds of thousands or millions of dollars per year on our product. In some cases, other third-party employees could torpedo the sales process too (like if a CTO or Chief Architect decided they didn't want to accommodate our architecture).
- The user devices, apps, networks etc can be company-provided and/or controlled
- Products are configured
    - super important. business rules, business workflows, business processes, automation, administration etc
    - By companies/sys admins
    - Last, if at all, by employees
    - feature flags / feature toggle
    - RBAC/user access management/security
    - launch darkly

[The parameters potentially affecting what end-users have access to. Each a subset of the previous one.]
| Name          | Description                                                                                | Owner              |
| ------------- | ------------------------------------------------------------------------------------------ | ------------------ |
| SKU           | Product mix subscriptions, modules purchased. <br> Legal agreements and restrictions.      | CIO, COO           |
| Configuration | Customer-wide setup: what is enabled, disabled, deployed, created or customized; for whom  | Admins, IT         |
| Tenant        | Configuration at a local level, for a particular org, business unit, geography or location | Manager, directors |
| Preferences   | Personal, work or convenience settings                                                     | End-users          |
| Context       | Day-to-day, business- or task-specific factors                                             | N/A                |

- Lower emphasis on design overall
    - At least on interaction design/visual design as understood nowadays; or for clouds/apps applications
    - Because there could be a lot of HFE work by public (powerplants in Europe) or private sector (eg Bell, CAE)

- High-stakes design changes
    - The stakes of making changes were very high. If we made a poor design decision that resulted in a major error it could take down our customer’s systems (and the other businesses that depended on that company’s services). This meant we needed to “measure a hundred times to cut once” and be very deliberate in our prototyping and rollout process.
    - Change management
- Higher value on reliability/~"stability over time"
    - Since users *rely* on the service, for doing their job or running their business, as opposed to consuming it for entertainment or as their optional volition
    - Often captured in contracts/SLAs; contractual agreements, levels of service, levels of uptime, legal liability
- Other legal frameworks
    - Some specific to industries, eg MILSTD or aviation standards; sometimes not de jure but de facto industry standards
    - Some "generic" but actually enforced, or possible enough to be enforced (eg WCAG, localization, GDPR)
- Testing is "managed"
    - No live A/B testing etc
    - But beta programs in partnership with customers
- Different "voice of the customer"
    - Design wasn’t the sole “voice of the customer.” We had entire teams in professional services and customer success who were in constant contact with users and whose job it was to represent their needs. This shifted my focus to be more on leaning into those relationships, interpreting the constant flow of feedback, and synthesizing it into smarter design choices.
    - dedicated research roles/team
    - customers only partially convey needs of users
    - the issue you’ve identified goes beyond product design and product experience into feature prioritization
- high barrier to entry
    - Another reason why good design is less found in  large enterprise software is because the barrier of entry to building something useful for B2B is a lot higher than B2C. You usually need a certain amount of industry knowledge and experience to create any semblance of a useful / usable product. Also B2B often needs a lot more features to be “sellable,” plus a sales engine. This already weeds out a lot of potential founders, willing investors, and thus good options in the market.

- The business metrics are different (eg PEPM, net dollar retention, retention, churn)

- Implementation costs are huge for the customers, in money, time, expertise, trust
    - As a result, so are switching costs
    - As a result, stickiness
    - As a result, reputation is key
    - Much higher cost of error / favors "nobody gets fired for buying IBM" / low risk-taking (on both sides)

- Real, human support
    - Support/expert communities

- Active sales process, sales teams
    - VS "just" online marketing, word of mouth, virality etc
    - Long standing relationships
- some features/product can be built for a single customer, if big enough
    - much more customer-driven, vs ~gut/vision driven innovation

- Concurrent/Backwards compatibility
- Brandability, Themeability, customization, White-labeling
    - some customers will have deep customization/deviance, and will tend to produce more content/transactions then B2C products, where user input is minimal or heavily controlled
- 3rd party integration, 3rd party support

- Frontstage vs. Backstage Customer opportunities
    - design can be at another level than "the app"

- design org not well considered/involved

---

UXA stock, à voir :

Relevant signals

• Deliverables
    • Flowcharts (a lot of them), decision trees, state charts
    • Entity-relationship diagrams, domain models
    • Tables & matrixes of all kinds, rich lists
    • Templates of all kinds (Figma, wiki, plain text, YAML, JSON, md)
    • Reference material of all kinds (ditto)
• Activities (and proof thereof, e.g. through the deliverables above)
    • Pitching to leadership, training to contributors, advocacy to all
    • Governance, guidance, office hours
• Keywords
    • Modular, composable, interface, interplay
    • Parameters, attributes, properties, configuration
    • Services, frameworks, platforms, orchestration
    • Patterns, emergent behaviors, rules & relationships
    • Terminology, ontology, taxonomy
• All of it packaged
    • As living artefacts
    • Geared towards a product-design-dev audience, not just a dev one
    • With clear delineation of responsibilities (what's owned by "the platform", what's opened to or expected from "partners")
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

• Keywords like information architecture, card sorting, visual hierarchy, design systems, patterns
    • Those are table stakes, and not indicative of an architectural practice
    • Especially when design systems are "tokens and components" rather than patterns, frameworks, screen flows, utilities, usage guidelines etc.
    • Especially when patterns are "big components" rather than "abstraction of a solution"
• Mentions of "strategy", "scalability", "consistency", "reuse" without further details
- Layout
- Responsiveness
- Style
- Perceived quality
- Perceived novelty

(They are still there, but their relative importance is lower)
