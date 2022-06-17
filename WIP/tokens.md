# Models for Design Token Setups

There are many ways to set tokens up (= create, use and maintain), some are easier than others depending on context. Furthermore, Usage drives structure drives naming, all of it is very difficult to change after the fact. Hence the need for shared understanding and array of solutions before starting to set things in code, aka in stone.

This doc provides vocabulary for discussion, and inventories patterns (ie solutions) and provides decision criteria to pick one (ie context).

For a refresher of what tokens are or why they're profitable: see reading notes or `Vocabulary.md`.

## Levels of Abstraction

various possible token abstraction levels

Define against variables too?

## Relationships

- tiering (formalized categories)
- aliasing (unformalized)

formalized = programmatically testable/enforceable

tiers can be virtualized

## Possible Setups/Combinations

each with authoritative examples (nb setup != tiering; eg Material, Spectrum and birse all have different approaches to 3-tiering)

recommended setup (2 tiered)

depict the whole thing so that allocation is clear and quantitative comparison easy (== several example, dev change costs reified and quantified, compared to flexibility costs)

## Decision Criteria

go further than ~descriptions with guidance for discussion/decision.

E.g. what "checkable against" criteria, f(context): big org, small org, partnerships, mono code base, 1 or several techs, 1 or several product lines/brands, pace of change etc. Each tier is more flexibility but more complexity thus cost for everyone (eng, design, product), beware of gold plating
