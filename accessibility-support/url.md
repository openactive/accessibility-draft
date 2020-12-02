---
description: A link to further accessibility information
---

# url

Many organisations will maintain a page or section of their website dedicated to accessibility needs. Linking back to this from OpenActive data can be helpful, particularly in cases where the information present in the data itself is sparse.

### Links in place of data

In the situation where no accessibility information is provided within the OpenActive datafeed itself, a link may well be the only source of information a disabled user has to determine whether a given event is right for them. 

In such cases, the link should be provided in the following form:

```text
"accessibilitySupport": [{
    "@type": "AccessibilitySupport",
    "name": "Further Accessibility Information",
    "url": "https://www.example.com/further-accessibility-information"
}]
```

