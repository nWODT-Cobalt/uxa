# Taxonomy for component states

<!-- components’? components? -->
<!-- bi-directional link with `Reading notes on design systems, components & tokens.md` -->

<!--BREAK-->

## Overview

“States” are visual feedback for a component’s temporary condition.
Users rely on their cues to understand and manipulate the UI.
Well-designed states support accessibility, improve usability, and contribute to brand expression and delight.

<!-- (not only visual but that’s the starting line for 99%) -->

<!-- commented figure eg I know that tab 1 is active and that Im ushovering tab 2 -->

This document is a quick reference to inventory and label common states, in order to:

- Discuss within a design team and its technical partners
- Scope the work
- Design in a consistent, complete and effective manner
- Structure Figma assets

<!-- At this time this document is a quick reference, rather than proper training material. -->

<!-- <jump to recap table> -->

## Methodology

### Scope

“States” is a broad notion. This document covers user-visible, user-triggered component’s states.

This excludes application states, that are driven by data status, business logic, system services or back-end calls.
It also excludes states that could be displayed on components, but aren’t in response to direct user manipulation.

For example, the “Unread” indicator of a “Messages” tab isn’t in scope. While the "Unread" status does exist, it characterizes a data attribute (read vs unread) rather than a component feedback (idle vs pressed down).

<!-- ditto for filtered, locked, unsaved etc -->
<!-- Notability Feedback Normal Notable xxx -->

Component states are also different from components properties such as size, emphasis, theme etc. Those properties are set at design time and don’t change at runtime.

<!-- not different but a subset -->

User-triggered states are transient: they cycle in quick succession. Thus a good rule of thumb to tell them apart from other attributes is whether they reset on page (re)load. If yes, they are likely components’ states, as covered in this document.

### Conventions

States are organized into "state categories". Each state name is unique.

### References

- [All the user-facing states](https://ericwbailey.website/published/all-the-user-facing-states/)
- [W3C](https://www.w3.org/TR/WCAG21/#dfn-states)
- Major vendors component libraries and guidelines

## Taxonomy

<!-- Have 1 example per “states group” (define that too) + 1 recap table-->
<!-- show how examples fill or not the general matrix -->

**Pointer Feedback**

`Idle`, `Hovered`, `Pressed Down`, `Disabled`, `Loading`

"Pressed down" is preferred to "Active", as per WCAG.

**Selection Feedback**

`Unselected`, `Selected`, `Indeterminate`

**Focus Feedback**

`Unfocused`, `Focused`

**Input Feedback**

`Empty`,  `In progress`, `Filled`

Note that “Empty” means “empty of user input”, not “empty of any content”. There may still be a placeholder, as a component property.

**Validation Feedback**

`No validation`, `Instructions`, `Error`, `Success`

Note that "Instructions" means "explanations in reaction to user input", not persistent help text. There may still be persistent help text, independently from instructions, as a component property.

**Others**

The states listed above are the most common. Further states should be considered on a case-by-case basis, such as "visited" for links or "dragged" for draggable elements.

<!--
States for complex composed elements like data grids *like what?*
States for non-form components like video player or map browser *like what?*
-->

## How-To

Here's how to use the provided taxonomy to support design activities.

### Scope

For each component, assess which states from the taxonomy do apply.
Not all components have all states: for example, a button has no notion of being "selected" or not. A radio button can be selected, but can't have an "indeterminate" state.

State categories are multiplicative rather than additive.
A tab control gets "Pointer Feedback" (4 applicable states) and "Selection feedback" (2 applicable states). That's 4 × 2 = 8 states, not 4 + 2 = 6 states.

<!-- show several composed examples at once eg `Idle, Unselected, Unfocused` vs `Hover, Selected, Unfocused` // E.g. a text field can be filled, in error , hovered and focused all at once -->

Note that that this step isn’t about “adding” states. Rather, it is about making sure existing states are accounted for, so that design decisions can be made with proper context.

### Design

Just because a state exists doesn’t mean it needs a unique design.
Some states can be very similar or downright identical in appearance.

<!-- similar: idle unselected vs idle selected, only 1 icon difference
identical: segmented control hover vs active -->

States don't have to be encoded with color only: icons, text, position shift etc. can also be very effective.

Finally, consider the whole component when styling states, like text labels associated to atomic controls.

<!-- eg a colored label for an active input field -->

### Figma

Name properties or variants with the state categories and states from the taxonomy.
This improves consistency for the builder and for the user, in turn improving maintainability and understandability.
It is ok to omit the word "feedback" from state category names.

Expose states as variants rather than booleans.

<!-- show pics of bad figma props then the better version -->

<!-- Figma props aren’t the exact same as conceptual component props; confusing -->

<!-- eg `Focused: Yes/No` -> `Focus Feedback Unfocused Focused` -->
