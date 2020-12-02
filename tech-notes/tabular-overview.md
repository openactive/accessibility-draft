---
description: OpenActive Accessibility at a glance
---

# Tabular Overview

## Top-Level Attributes

Note that all top-level attributes are considered optional.

| Property | Format | Notes |
| :--- | :--- | :--- |
| `oax:accessibilitySupport` | Array of `oax:accessibilitySupport` | See further below |
| `oax:accessibilitySupportLevel` | Controlled vocabulary. See [page](../top-level-attributes/accessibilitysupportlevel.md) on `accessibilitySupportLevel` | Applies to opportunities only |
| `schema:amenityFeature` | Array of `schema:LocationFeatureSpecification` | Applies to places only |
| `oax:carerPolicy` | Text |  |
| `schema:contactPoint` | `schema:ContactPoint` |  |
| `schema:review` | Array of `schema:Review` |  |
| `oax:transportNote` | See [page](../top-level-attributes/transportnote.md) on `transportNote` | Applies to places only. |

## `accessibilitySupport` Attributes

Note that the 'Status' assigned to each property is on the assumption that an \(optional\) `accessibilitySupport` value has already been supplied. That is to say, there is no requirement that data publishers populate the `accessibilitySupport` field. However, if they do, they must supply a `name` for it.

| Property | Status | Format |
| :--- | :--- | :--- |
| `schema:contactPoint` | recommended | `schema:ContactPoint` |
| `schema:description` | recommended | Text |
| `oax:isAdvanceNoticeRequired` | recommended | Boolean |
| `schema:hoursAvailable` | recommended | `schema:OpeningHoursSpecification` |
| `schema:name` | required | Text |
| `oax:participantConditionSupported` | optional | Controlled vocabulary. See [page](../accessibility-support/participantconditionsupported.md) on `participantConditionSupported` |
| `schema:url` | recommended | `schema:URL` |

