---
description: Capturing complex accessibility provision
---

# Overview

In cases where accessibility provision is good, data-collection practices are strong, or both, it will generally be helpful to model accessibility information with more detail. In such cases, the `accessibilitySupport` datatype should be used.

An `accessibilitySupport` object may have any combination of the following attributes:

* [description](), a free-text description of the support offered
* [isAdvanceNoticeRequired](isadvancenoticerequired.md), indicating whether individuals requesting such support are required to alert staff in advance to their attendance
* [hoursAvailable](hoursavailable.md), capturing the hours in which such support is available
* [name](name.md), a short label indicating the nature of the support
* [participantConditionSupported](participantconditionsupported.md), a list of the medical condition or condition\(s\) for which an activity is suitable
* [url](url.md), providing a hyperlink to more information

Note that any number of `accessibilitySupport` objects may be associated with a given place or event.



