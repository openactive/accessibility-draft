---
description: Representing information drawn from the Active Places Data Platform
---

# Mapping from Active Places

One of the richest sources of information about accessibility provision in the physical-activity sector across England is the [Active Places Data Platform](https://dataplatform.activeplacespower.com/). 

Active Places records accessibility information in a number of fields, as itemised below.

### DisabilityAccess

This value should be left unrepresented \(that is to say, can be discarded\) in mapping to OpenActive accessibility attributes.

### DisabilityParams

DisabilityParams followed by an 'N' \(for 'No'\) should be discarded. Those followed by a 'Y' \(for 'Yes'\) should be mapped as an `amenityFeature` with:

* a `type`  of "LocationFeatureSpecification"
* a `name` consisting of the Active Places term, prefixed by the word "Accessible"
* a `value` of `True`

For example, an ActivePlaces DisabilityParams value of 

`Parking,Y,Finding and reaching the entrance,N,Reception area,N,Doorways,N, Changing Facilities,Y,Activity Areas,N,Toilets,Y,Social Areas,N,Spectator Areas,N,Emergency Exits,Y`

would be represented in OpenActive data as

```text
"amenityFeature": [
    {"@type": "LocationFeatureSpecification",
     "name": "Accessible Parking",
     "value": true },
    {"@type": "LocationFeatureSpecification",
     "name": "Accessible Changing Facilities",
     "value": true },
    {"@type": "LocationFeatureSpecification",
     "name": "Accessible Toilets",
     "value": true },
    {"@type": "LocationFeatureSpecification",
     "name": "Accessible Emergency Exits",
     "value": true }
]
```

### DisabilityNotes

Each Active Places DisabilityNote should be mapped to an `accessibilitySupport` object with a `name` of "Disability Notes" and a `description` field holding the content of the field.

### DisabilityChangingPlaces

In cases where the value of `DisabilityChangingPlaces` in Active Places is a 0 \('No'\) or 2 \('Don't Know'\), the information should be discarded and not mapped to OpenActive. In cases where it is 1 \('Yes'\), it should be represented as an `amenityFeature` with the `name Disability Changing Places`, and a value of `true`.

```text
"amenityFeature": [
    {"@type": "LocationFeatureSpecification",
     "name": "Disability Changing Places",
     "value": true}
]
```

