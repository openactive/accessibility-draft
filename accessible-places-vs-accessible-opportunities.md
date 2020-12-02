---
description: What is actually being modelled?
---

# Accessible Places vs Accessible Opportunities

One of the first questions that needs to be answered when describing accessibility provision is what it is that is actually being made accessible. Typically this will have one of two answers:

* the _place_ where an activity is being held
* the _event_ itself \(referred to formally in the OpenActive context as an 'opportunity' or an 'event'\). 

For example, a gym or leisure centre may be provided with disabled parking, accessible toilets and changing rooms, etc. These are available to all users of the building regardless of the particular class or facility they're attending. Accordingly, these should be considered accessibility features of the _place_ in which the activity is held. In terms of the Opportunity specification, details about this should be included in the `Event.location` field, which takes a `schema:Place` as its value.

On the other hand, many classes are tailored for people with a particular accessibility need – for example, gym sessions with reduced sensory stimuli for people on the autistic spectrum.  In this case, the accessibility features are associated with a specific time-slot, not the gym as a whole. It accordingly makes sense to model them on the event itself, rather than its location.

For the most part, the properties used to model accessibility information about places and about opportunities are the same; even if they can be attached to different kinds of entities. The only exceptions are [`amenityFeature`](top-level-attributes/amenityfeature.md)and [`transportNote`](top-level-attributes/transportnote.md)\(both applicable to places, but not opportunities\) and [`accessibilitySupportLevel`](top-level-attributes/accessibilitysupportlevel.md) \(applicable to opportunities, but not places\).

If in doubt about whether to relate a particular property to a place or to an opportunity, ask yourself the question 'is this feature available to everyone in all classes held in a facility, or is it limited only to some of these?' If the former, the information almost certainly relates to the relevant place; if the latter, it should be attached to individual opportunities. 

For a concrete illustration of the different approaches used for modelling accessibility in relation to places and opportunities, see the [Accessible Leisure Centre](worked-examples/accessible-leisure-centre.md) and [Chair Yoga](worked-examples/chair-yoga.md) worked examples.

