---
description: Indicating limitations on availability
---

# hoursAvailable

Some forms of support may be available only at certain times during the day. In this case, the times during which these can be accessed must be included.

### Implementation Example

The `@type` for `hoursAvailable` is a [`schema:OpeningHoursSpecification`](https://schema.org/OpeningHoursSpecification).

```text
"accessibilitySupport": [
    { "@type": "AccessibilitySupport",
      "name": "Pool Hoist",
      "hoursAvailable": [{
        "opens": "09:00:00",
        "closes": "20:00:00"
      }]
    }
]
```

