---
description: Representing information drawn from the Active Places Data Platform
---

# Mapping to and from Active Places

One of the richest sources of information about accessibility provision in the physical-activity sector across England is the [Active Places Data Platform](https://dataplatform.activeplacespower.com/). 

Active Places records accessibility information in a number of fields, as itemised below.

### DisabilityAccess

This value should be left unrepresented \(that is to say, can be discarded\) in mapping to  OpenActive accessibility attributes.

### DisabilityParams

DisabilityParams followed by an 'N' \(for 'No'\) should be discarded. Those followed by a 'Y' \(for 'Yes'\) should be mapped as an `amenityFeature` with:

* a `type`  consisting of the Active Places term, prefixed by the word "Accessible"
* a `name` consisting of the Active Places term, prefixed by the word "Accessible"
* a `value` of `True`

For example, an ActivePlaces DisabilityParams value of 

`Parking,Y,Finding and reaching the entrance,N,Reception area,N,Doorways,N, Changing Facilities,Y,Activity Areas,N,Toilets,Y,Social Areas,N,Spectator Areas,N,Emergency Exits,Y`

would be represented in OpenActive data as

```text
"amenityFeature": [
    {"type": "Accessible Parking",
     "name": "Accessible Parking",
     "value": "True"},
    {"type": "Accessible Changing Facilities",
     "name": "Accessible Changing Facilities",
     "value": "True"},
    {"type": "Accessible Toilets",
     "name": "Accessible Toilets",
     "value": "True"},
    {"type": "Accessible Emergency Exits",
     "name": "Accessible Emergency Exits",
     "value": "True"}
]
```

### DisabilityNotes

Each Active Places DisabilityNote should be mapped to an `accessibilitySupport` object with a `name` of "Disability Notes" and a `description` field holding the content of the field.

### DisabilityChangingPlaces

