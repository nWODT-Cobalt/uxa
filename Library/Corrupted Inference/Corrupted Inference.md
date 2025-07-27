# Corrupted Inference

^
A really short activity to illustrate a notion that’s otherwise annoying to put in words: how incomplete context can lead to misunderstanding.

---

![](assets/engines-status.pdf)

^
As the captain of this plane, do you notice anything?  
“Engine 4 is down!”, right? Now what if I tell you that engine 4 works fine, exactly like the other engines; it’s just not hooked up to the display. We almost went for an emergency landing there, woops!  
If several entities share the same “status” (in this example all engines at 80% forward thrust) but only some of them expose their status, then end-users are going to assume that entities not exposing their status are in a “bad” status.  
Users aren’t going to guess that the status indication is missing, they’re just going to assume that the entity is “broken”, in error state.  
It works the other way around too: if some errors are flagged but not all of them, users are just going to assume that entities without error badges are fine, when they aren’t.  
In any case users are making bad assumptions, because inconsistent encoding has  corrupted their inference.  
Takeaway: flag/badge/status-indicate  **all** entities in a given context, in the same way for the same thing.
