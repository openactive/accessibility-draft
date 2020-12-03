---
description: Medical and/or chronic conditions for which an activity is suitable
---

# participantConditionSupported

In cases where an activity or opportunity is recommended as suitable or therapeutic for a particular accessibility need \(e.g., sensory impairment\) or medical condition \(e.g. pregnancy\), this condition should be indicated using the `participantConditionSupported` property.

The values for this property must be drawn from the Participant Condition Supported [controlled vocabulary](https://disab.herokuapp.com/en/hierarchical_concepts.html). Note, however, that this vocabulary is still evolving and is far from static. If you have terms you wish to see added or suggestions for its improvement, please see our [Getting Involved](../getting-involved.md) page to find out how you can contribute.

### Implementation Example

Note that the Participant Condition Supported vocabulary is defined as a SKOS vocabulary. It accordingly consists of `skos:Concepts`.

```text
"participantConditionSupported": [
    { "@type": "Concept",
      "@id": "https://openactive.io/accessibility/pcs/_ff9a09ed-fb5a-4a62-b4d7-0fa263aa631d"
      "prefLabel": "Cardiac Recuperation"
    },
    { "@type": "Concept",
      "@id": "https://openactive.io/accessibility/pcs/_e2f6e425-66b0-4c74-b843-d3dbc634b99"
      "prefLabel": "Post-surgical Recuperation"
    }
]
```

