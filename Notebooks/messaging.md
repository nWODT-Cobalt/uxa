# a taxonomy of messaging

## context

inbox systems for complex products

1. Not all "communication to user" is "notifications"
2. Notifications = timely + out-of-view
3. Notifications aren't "the thing", they aren't even 1:1 to "the thing"
4. "mail client patterns" aren't notification tools; they are action and audit/historical records tools. The OS/platform is the notifications tool.

## taxonomy

what are notifications compared to other forms of messaging

Notifications are: preview + shortcuts
subtypes:
Activity: action required (preview + shortcuts)
Alerts: read-only, for awareness (just preview)

A
Timely
(or ~mandatory)
(or ~action/awareness required)

B
Not Timely
(or ~optional)
(or ~action/awareness not required)

C
Out of View
(not necessarily out of product,
more like out of view or domain)

D
In View

AC notification
AD feedback
BC announcement, activity/news feed
BD instruction, nudge

Notifications != Objects != mail client content (regardless of the proxy level)
!= mail client content because nots are n:1 to objects, not all nots will go to mail client (cf props below) etc
workflow objects (or event?)
the notification is really only tied to its change of status, not its nature/existence

## properties

*eg for creation and weighting of business rules; themselves for bundling, priority, silent delivery etc*

### Properties of the territory entity

Object/data OR action
~immanent to the business

Synchronous (timely?)
timely, .g. TALK p2p chat, or feedback, e.g. confirmation that a command has gone through)
asynchronous (no due date or far-out deadline, e.q. availability of tax slips)

Time sensitive
requests or actions with a due date

Actionable
informational, for awareness, read-only (.g. "your time-off request has been accepted" or "geofenced punched-in")
doesnt mean "not important"
actionable, for decisionm follow-up expected (e.g.To-do task, or timecard review)

Critical
not (e.g. baby announcement, neither frequent nor important)
(e.g. legally binding or mandatory, like an attestation or benefits enrollment)
criticality = frequency × importance

"frequency"

Priority

Expectancy

legality

Meaningful origin
system thing
request from manager or colleague in the same team

Preferences
Employee convenience, eg authorize emails but not texts
company configuration (e.g right to disconnect laws)

Initiator
(e.g. en employee asking to swap shifts may see all the steps the request is going through)
observer or approver (.q. the manager approving the shift may only see key steps of the request)

Persistent
ephemeral (no need to keep track, e.g.a p2p communication)
persistent: keeping the record is important for audit purposes, e.g.a compliance training)

Habitat (same as persistence?)
no place, at least no canonical one, where the object exists outside of Inbox (eg Request Period?)
Object are stand-alone/embedded (eg TOR?)

~Dynamic/status
static eg like a punch record (immutable time/location/job/employee)
dynamic eg lifecycle, like a request, with different content and actions at every step
Maps to Pro's To Do/Waiting/Done

### Properties of the map component/notification (on top of the entity ones)

Notification/ping/signal
Notifications are O-n:1 to objects
(Eg several possible reminders, on several possible channels)
~decided by the design

In-product vs out-of-product

Interaction
not blocking
blocking

Dismissisable
auto dismissed, user dismissed
not dismissable

Actionable
informational
actionable
The degree of actionability and the required context to do so is the single biggest decision criteria.
How much can be done at the ping level, depending on how big the ping is, vs at the canonical/origin level

Properties of the map component/notification (on top of the entity ones)
Notification/ping/signal
Notifications are O-n:1 to objects
(Eg several possible reminders, on several possible channels)
~decided by the design
In-product
s out-of-product
Interaction
not blocking
blocking
Dismissisable
auto dismissed, user dismissed
not dismissable
Actionable Prime
informational
actionable
The degree of actionability and the required context to do so is the single biggest decision criteria.
How much can be done at the ping level, depending on how big the ping is, vs at the canonical/origin level
