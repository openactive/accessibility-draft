---
description: What is actually being modelled?
---

# Accessible Places vs Accessible Opportunities

One of the first questions that needs to be answered when describing accessibility provision is what it is that is actually being made accessible. Typically this will have one of two answers:

* the _place_ where an activity is being held
* the _activity_ itself

For example, a gym or leisure centre may be provided with disabled parking, accessible toilets and changing rooms, etc. These are available to all users of the building regardless of the particular class or facility they're attending. Accordingly, these should be considered accessibility features of the _place_ in which the activity is held. In terms of the Opportunity specification, details about this should be included in the `Event.location` field, which takes a `schema:Place` as its value.

On the other hand, many classes are tailored for people with a particular accessibility need – for example, gym sessions with reduced sensory stimulus for people on the autistic spectrum.  In this case, the accessibility features are associated with a specific time-slot, not the gym as a whole. It accordingly makes sense to model them on the `Event` itself, rather than its location.

To learn more about conveying accessibility information concerning physical locations, see [Modelling Places](modelling-places/overview.md) and the [Accessible Leisure Centre](worked-examples/accessible-leisure-centre.md) worked example. To find out more about describing accessible Opportunities, see the sections on [Opportunity top-level attributes](top-level-attributes/overview.md), on  [accessibilitySupport](accessibility-support/overview.md) attributes, and the [Chair Yoga](worked-examples/chair-yoga.md)  example.

