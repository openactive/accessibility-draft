---
description: Getting to and from an event or place
---

# transportNote

Transport can present unusual challenges for individuals with accessibility needs. Not only are disabled people more likely than average to be reliant on public transport, they may be constrained to particular paths because of requiring e.g. step-free access or audio signals to approach a venue safely. Providing detailed information about transport can increase user confidence and thus the eventual likelihood of actual attendance at an event.

Further information about the use of `transportNote` can be found in the [RouteGuide 1.0 specification](https://openactive.io/route-guide/#describing-transport-to-and-from-the-route-oa-transportnote).

Note that the presence of disabled parking should normally be communicated as an [`amenityFeature`](amenityfeature.md).

### Implementation Example

The `@type` for transportNote is `oax:TransportNote`. Note that this is currently also defined within the top-level OpenActive namespace \(`oa:`\), but this definition is intended for removal once the Accessibility specification is formalised.

```text
"transportNote" : [
    { "@type" : "TransportNote",
      "transportMode": "Bus",
      "description": "The number 37 Southbound stops outside and across
      the street from the leisure centre. A pelican crossing with audio
      signal leads across the four-lane street from the stop directly 
      to the centre entrance" },
    { "@type" : "TransportNote",
      "transportMode": "Rail",
      "description": "The Maiden Valley tram stop is a ten-minute walk
      from the leisure centre. All crossings en route are wheelchair-
      accessible, though some gradients are steep." }
]
```

