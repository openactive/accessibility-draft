---
description: Getting in touch about accessibility needs
---

# contactPoint

Accessibility needs are complex and individual: very often, disabled individuals will want to get in touch with someone who can provide them with fine-grained information about the kind of support offered and how suitable it is for their needs. As such, `contactPoint` information is highly valued by those with accessibility needs, particularly in regard to activities they have never tried before.

### Implementation Example

Note that the `@type` for `contactPoint` is `schema:ContactPoint`. The value of `contactType` should normally be "Accessibility Information", unless a more specific and dedicated description is applicable.

```text
"contactPoint": {
    "@type": "ContactPoint",
    "contactType": "Accessibility Information",
    "email": "example@example.com",
    "telephone": "0555555555"
}
```

