# Notes on enterprise design

<!-- A tentative look at the specificities of enterprise design -->

<!--BREAK-->


**Managing multi-persona dynamics/the customer isnt the user**

The distinction between buyer and user is a big one. For me, that meant designing mostly for the security engineer (the user) but delivering enough value to the Chief InfoSec Officer (the buyer) for them to see it was worth spending hundreds of thousands or millions of dollars per year on our product. In some cases, other third-party employees could torpedo the sales process too (like if a CTO or Chief Architect decided they didn't want to accommodate our architecture).

**Not prescriptive of scale**

Scale comes with its own set of considerations "eg at scale, all edge cases are frequent".
some B2B apps have a very small scale (eg medical tools) some B2C products have a very large scale (eg social networks)

**Different "voice of the customer"**

Design wasn’t the sole “voice of the customer.” We had entire teams in professional services and customer success who were in constant contact with users and whose job it was to represent their needs. This shifted my focus to be more on leaning into those relationships, interpreting the constant flow of feedback, and synthesizing it into smarter design choices.

**High-stakes design changes**

The stakes of making changes were very high. If we made a poor design decision that resulted in a major error it could take down our customer’s systems (and the other businesses that depended on that company’s services). This meant we needed to “measure a hundred times to cut once” and be very deliberate in our prototyping and rollout process.

Change management

contractual agreements, levels of service, levels of uptime, legal liability

---

a quick intro at/quick considerations about enterprise design

realities to take into account, that change the goals, role, engagement, value-add and ultimately practice of the B2B designer vs B2C designer

*look for "B2B" design lit*

NB: B2B != enterprise design != ? "internal tools". B2B can be "for experts by experts" eg medical imagery, flight sims etc





<!--
Knowing that the ecological context is different since:
- The buyers aren't the users, the users aren't the buyers
- The user devices, apps, networks etc can be company-provided and/or controlled -->

<https://www.betterbydesign.cc/p/7-insights-for-navigating-b2b-design>

---

Whatever it is, “enterprise design” is different from consumer, e-commerce, product, social, community, blogging, news, etc design.
Here’s a tentative list of practice/outcomes/considerations which are important in “enterprise design”, compared to other fields of UX design:

<!-- B2B RWA -->
<!-- tactical level -->
<!-- For new designers, or otherwise experienced designers or design managers looking to work in the field. -->

- Accessibility
- Brand
- Compliance (whether to internal guidelines, or external ones like legal or industry standards)
- Frameworks
- Internationalization
- Interplay
- Platforms
- Scalability
- White-labeling
- 3rd party integration
- 3rd party support

<!-- Framework (fwk): a black-box genie’s lamp lol service deterministically prescribing a holistic design solution (where, how, when, who; not what) who/what/where/when/how  for cross-suite features fed a complex use case.
They’re partially or completely automated;  through templating, governance and programmation. They’re owned and operated by suitex designers. -->

This can be achieved through:

- Business processes
- Composability
- Configurability (wide and deep, from component props to full-on admin areas)
- Interfacing
- Modularity
- Multi-channeling
- Orchestration
- Platforms
- Portability
- Themeability
- RBAC

<!-- incl. branding, etc; some customers will have deep customization/deviance, and will tend to produce more content/transactions then B2C products, where user input is minimal or heavily controlled) -->

<!--
As opposed to:

- Layout
- Responsiveness
- Style
- Perceived quality
- Perceived novelty

(They are still there, but their relative importance is lower)
-->

<!--
At a higher level:

- Co-strategy
- Governance
- Partnerships
-->

[The parameters potentially affecting what end-users have access to. Each a subset of the previous one.]
| Name          | Description                                                                                | Owner              |
| ------------- | ------------------------------------------------------------------------------------------ | ------------------ |
| SKU           | Product mix subscriptions, modules purchased. <br> Legal agreements and restrictions.      | CIO, COO           |
| Configuration | Customer-wide setup: what is enabled, disabled, deployed, created or customized; for whom  | Admins, IT         |
| Tenant        | Configuration at a local level, for a particular org, business unit, geography or location | Manager, directors |
| Preferences   | Personal, work or convenience settings                                                     | End-users          |
| Context       | Day-to-day, business- or task-specific factors                                             | N/A                |


also: feature flags / feature toggle
RBAC/user access management/security
launch darkly
Backwards compatibility
