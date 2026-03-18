# Notes on B2B Design

<!--BREAK-->

## Overview

<!-- Boo! Better titles/outline -->
<!-- streamline and define terminology, esp “enterprise design products”, end-users vs employees vs individuals etc -->

<!-- Frame better as: factors *directly* affecting the design org -->

<!-- card sort the whole thing for chunking/actionability
+send to @D? -->

<!-- sweep for:
- enteprise vs b2b
- customer vs buyer
- users vs end-users -->

B2B design is the design practice at companies that serve other companies rather than individual customers.
It’s for example the business of Dassault, IBM, Oracle, Salesforce, SAP, ServiceNow etc.

<!-- also known as enterprise design -->

B2B design has different goals, business models, metrics, roles, audiences, tools, engagement, culture and practices than consumer product design.

This document is an early mind sweep.
It can be helpful for designers curious about the B2B design space, as training material, interview framework or conversation support.

This first version has been simplified to large SaaS companies with thousands of employees, including dozens of designers.

<!--
Futher definition:

- buyer (the person, a decision maker as opposed to an employee) vs customer (the company) super-vs the end-user vs vendor
- distinction against service design or UXA vs SuiteX
- could also be “institutional” or “organizational” design, to account for gov work, NGOs, associations etc
- NB different from “productivity”. Some productivity is B2C eg office vs google docs vs iwork, or self accounting software, or Trello etc
- technically could be on prem, hybrid native etc
- (technically could be small orgs) some B2B apps have a very small scale (eg medical tools) some B2C products have a very large scale (eg social networks)
- Scale comes with its own set of considerations “eg at scale, all edge cases are frequent” *heh, not germane*
- “the product”
-->
<!-- **Constant consideration for scalability**

*From Loren Mack*

What would be a nice and easy design for consumers often needs to change to accommodate oceans of data. Search primary models. Limiting server calls and their payload size.
The need for bulk data manipulation and update. The need for large data set analytics, assessments, and diagnostics.
Being able to pre-test or rollback large transactions before deciding to ‘keep them’, AKA Impact Analysis. Stuff like that. -->

Summary:

<!-- actual links when Marked 3 doesnt break them during PDF export -->
<!-- update when complete -->

- The customer isn’t the user
- Expert users
- Controlled environment
- Configured products and services
- Complex deployment and adoption
- Weaker relationship with end-users
- Difficult changes
- Enduring tech stacks
- Lesser design culture/outcomes
- Different business success metrics
- Enforced regulations
- Different to “no” branding
- Backstage opportunities

## Notes

<!-- What a messy outline. Structure better. Causes-consequences? Topics? eg the space vs the work vs releasing vs… -->

**The customer isn’t the user**

<!-- The single biggest difference between consumer product design and enterprise design is its foundational definition: the fact that the customer isn’t the user. -->

Enterprise design products are selected at the executive level (e.g. by the CIO[^cio] or CTO[^cto]), then used by the rest of the company.

Whereas employees may care about speed, ease of access, ease of use or personalization, enterprise buyers will rather first look at  TCO[^tco], security, scalability, compatibility or compliance. They will consult with their internal legal, brand or technical representatives, further pushing away individual considerations.

[^cio]: Chief Information Officer
[^cto]: Chief Technology Officer
[^tco]: Total Cost of Ownership

**Expert users**

The users of enterprise design products are likely to be a professional audience, experts in their field with deep knowledge and strong opinions.
This audience is often segmented into user groups of very different cultures, motivations and responsibilities; each interfacing with the product at different points.

This domain expertise doesn’t necessarily translate product expertise, or to being tech-savvy overall.
E.g. just because a surgeon has great medical proficiency doesn’t mean they know all of Excel’s shortcuts.

**Controlled environment**

Devices and apps are company-provided and controlled.

Personal devices may not be able to be brought in the workplace, for example nurses or retail staff leaving their smartphones in the locker.
Desktop or countertop hardware can be locked down: tin cast into ports, computers physically bound to furniture.

Software outside of a very restrictive allowlist may not be installed.
Many sites, apps or services may not be allowed on a monitored network.
In extreme cases, devices can be air-gapped into LANs[^lan] without Internet connection.

End-users identity is controlled too (e.g. through SSO[^sso]), making it inconvenient or downright impossible to access new services.

The *controlled environment* affects *deployment and adoption*, but can also hinder/hamper/impede prototyping and testing, and even performance (e.g. as CDNs[cdn] are blocked).

[^sso]: Single Sign-On
[^lan]: Local Area Network
[^cdn]: Content Delivery Network

**Configured products and services**

Enterprise products are usually highly configurable in order to support business processes, regulations, org topologies etc.

Customers’ system admins will work hand-in-hand with the vendor to initially deploy the product, and may then maintain and extend it on their own. User access, security, business rules etc will drive who can access what, and how.

End-users may still be able to set their own preferences. If so, it will be downstream of layers of company-driven decisions.

Consequently, product instances can be significantly different from one tenant to another, or from one end-user to another within a tenant, requiring to design for and with *modularity*.

<!-- As opposed to B2C apps that are largely the same, at least morphologically, for their whole user base. Eg there’s only 1 whatspp Ui-->

Finally, the configuration surface (also known as “admin area” or similar) required for the above is a huge *backstage opportunity* of its own.

**Complex deployment and adoption**

The effort to implement or deploy an enterprise system can be huge for the customer, in money and time.
A successful deployment can take months. An unsuccessful one, years.

Adaption may be mandated but not realized on the field, as *expert users* may not be interested and have a lot of internal leverage.

<!-- And have very good reasons to feel so. -->

Special advocacy, training or compliance programs can be ran throughout the organization.

It’s very different from the B2C space where most users get products through app stores or the cloud, and are not interested or able to decline an app update.

**Difficult updates/Managed changes**

<!-- the customer will control the updates, not the vendor -->
<!-- How's that different from the previous one? Initial implementation vs subsequent updates? -->
<!-- Rewrite as "complex deployment and updates (incl change management)" because that's what's relevant through the design lens vs "complex adoption" -->
<!-- Different parallel delivery channels. The early adopter or privileged parterns or canary one is a good avenue for testing-->

A very high value is placed on reliability and stability, since users rely on the service for doing their job or running their business.
Especially more so since *deployment is complex*.

<!-- as opposed to consuming it for entertainment or as their optional volition -->

Those metrics are often explicitly laid out in contracts and SLAs[^sla], with quantified levels of uptime, quality of service and eventual penalties.

<!-- difficult to iterate
the org may not be set up for or interested in agile follow-up anyway -->

<!-- no continuous releases, esp with zero notes, heads-up of speedbumps like in the consumer world -->

[^sla]: Service Level Agreement

Thus updates are high stakes. Testing and releases are managed through formal programs, such as beta partnership with costumers or launching darkly with feature toggles, rather than live A/B testing and continuous releases. The deployment of a new version is contingent to explicit customer acceptance, and may be very slow or not happening at all.

<!-- If we made a poor design decision that resulted in a major error it could take down our customer’s systems (and the other businesses that depended on that company’s services). This meant we needed to “measure a hundred times to cut once” and be very deliberate in our prototyping and rollout process. -->

**Expensive mistakes**

Because of *Complex deployment and adoption* and *Difficult updates*

favoring a low risk-taking for both the vendor and the customer. “Nobody gets fired for buying ~~IBM~~ Atlassian.”

**Long lead-cycles**

with 3–5 years long contracts, and renewal negotiated quarters or years in advance.

**Weaker relationship with end-users**

The direct line of communication between designer and user may be weak.

On one hand, designers are less in touch with the audience.
Companies of a certain size will have dedicated research roles, rather than designers performing research tasks.
Likewise, there may be entire departments like sales, customer success, support or professional services who are much closer to the action, and whose insights are considered “the voice and the customer” and drive the conversation.

<!-- also not easy to find proxies, eg what do you do for test pilots -->
<!-- there may be ad-hoc Support/expert communities -->

On the other hand, the audience itself is different.
The primary contacts may be buyers rather than end-users; the former only partially conveying the need of the latter.

This issue goes beyond product discovery and design, and into feature prioritization.

**Enduring tech stacks**

<!-- Older, mature, sticky -->

The tech stack in enterprise design can trail the leading edge by years.

<!-- practice too -->

This isn’t just a function of big and mature organizations, but also a commercial interest or a contractual obligation to support older version of the product.
It’s compounded by the fact that *change is difficult*.

**Lesser design culture**

<!-- thus maturity, outcomes etc -->

Enterprise vendors have historically put less emphasis on user experience than their consumer counterparts. To this day, C-level design voices are very rare, and “design founders” virtually inexistant.

Note that in some industries, there can be a strong design function that’s not about UX design, but HFE[^hfe].

*reword*

[^hfe]: Human Factors Engineering

<!-- Another reason why good design is less found in large enterprise software is because the barrier of entry to building something useful for B2B is a lot higher than B2C. You usually need a certain amount of industry knowledge and experience to create any semblance of a useful / usable product. Also B2B often needs a lot more features to be “sellable,” plus a sales engine. This already weeds out a lot of potential founders, willing investors, and thus good options in the market. -->

**Different business success metrics**

<!-- thus different design success metrics too -->

The monetization is usually different: recurring subscription revenue expressed in PEPM[^pepm] dollars, rather than freemium or ad-supported.

[^pepm]: Per User Per Month

*B2B metrics are weak and rare, when marketing metrics exists thay dont make their way to us*

<!-- net dollar retention, retention, churn -->

**Enforced regulations**

<!-- Legal Frameworks -->

Regulatory compliance is much more prominent in enterprise than in consumer design.

Because of the demanding audience, criticality of service, engagement with government or just sheer scale, regulations are either enforced or assessed as likely to be: localization in countries of operation, privacy laws such as GDPR, accessibility laws like WCAG, etc.
If not *de jure*, at least *de facto*.

Most verticals add their own standards like MILSTD references or ICAO doc series.

<!-- HIPAA, GDPR -->

*HIPAA, ISO27001*

<!-- ISO 9341, 1347, 16290; NF EN 1325 -->

<!-- ISO 27001, ISO 27701 -->

<!-- SLAs and other contractual agreements vs no one caring about a EULA -->

**Different to no branding**

<!-- actually two-tiered branding -->

Enterprise branding will focus for what matters to its audience: reliability, configurability, feature-richness, etc over being enticing, easy to use, differentiated.

<!-- better connect to previous such enum -->

Moreover, customers company often theme the product to their own brand, because they offer it internally to their employees or bundle it as part of their products.
The initial brand collaterals may never reach end-users.

<!-- thats hiding the much bigger composability/integration practice -->

<!-- This message may never reach end-users because it’s not intended for them to begin with -->

<!-- Moreover, enterprise products very often have to be themable/white-labeled, . -->

<!-- Bonus: building such white-labeling theming capabilities is a typical enterprise design project! -->

<!-- Brandability, Themeability, customization, White-labeling, 3rd party integration -->

**Backstage opportunities**

Since enterprise design covers not just end-users but also the many areas enabling them, the surface for design and innovation is broader than in exclusively consumer products.

Configuration, administration, orchestration and the many intersections thereof are as many points where designers can intervene.

<!-- business workflows, business processes, automation, administration etc: missing a whole section on the “actual business” side of things!-->

<!-- front stage “opportunities” eg MFA -->

**Domain knowledge requirement**

The specificities and depth between domains (e.g. between finance and healthcare) or even between players within a domain (e.g.)
As opposed to say e-commerce where there’s a lot more commonalities between ~companies, and the issues are elsewhere.

Combined with *expert users* and *regulations*, it means internalizing a lot of domain knowledge in order to be able to contribute.

Some employers will only hire designers with prior experience in their vertical.

**Plan for modularity**

*thats practice not a factor*

in conceptualization (UXA!)

in deliverables

in collaboration (set expectations with counterparts, divide the work among design teams)

## Sources

- [7 Insights for Navigating B2B Design](https://www.unknownarts.co/p/7-insights-for-navigating-b2b-design)
- With contributions from Loren Mack and Étienne Viale. Thank you!

<!--
**High switching costs**

in turn making enterprise products very sticky and creating a high barrier to entry for competitors
thats actually for the buyer, but mention it somewhere else
-->

<!-- **Difficult cust acquisition**

- Active sales process, sales teams
    - VS “just” online marketing, word of mouth, virality etc
    - Long standing relationships
- some features/product can be built for a single customer, if big enough
    - much more customer-driven, vs ~gut/vision driven innovation
- lot more buyer power in some areas

thats true but is it a design issue? are some other points likewise not directly connected to design?
-->

<!--

**subsequent practice**

### Hiring B2B designers

sous la forme: “deliverables: information architecture -> Flowcharts”?

UXA signals, à voir

Relevant signals

- Deliverables
    - Flowcharts (a lot of them), decision trees, state charts
    - Entity-relationship diagrams, domain models, class diagrams
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
