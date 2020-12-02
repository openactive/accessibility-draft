---
description: Describing support offered to participants with accessibility needs
---

# accessibilitySupportLevel

One of the most important pieces of information disabled users have is knowing what degree of support they can expect when attending an event. This is captured in the `accessibilitySupportLevel` property, which can have one of three values:

* "No Additional Support", indicating that no additional provision is made for individuals with accessibility needs.
* 'Inclusion Support', indicating that some additional provision will be made for individuals with accessibility needs. If this value is used, it is advised that an [`accessibilitySupport`](../accessibility-support/overview.md) object also be supplied to indicate more fully what this support consists of.
* 'Accessibility Needs Only', which indicates that the event has been specifically designed for participants with accessibility needs. Again, this value should be accompanied by an [`accessibilitySupport`](../accessibility-support/overview.md) object indicating who the intended audience is and what support they can expect to receive.

Note that `accessibilitySupportLevel` is a property only of events; it cannot be applied to a place.

