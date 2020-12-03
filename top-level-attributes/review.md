---
description: User feedback related to accessibility
---

# review

Data and assessment assurance can be difficult in relation to accessibility needs, and trust in claims of being 'accessible' or 'disability friendly' is often low. Publishing user reviews are one way of gathering feedback and gaining the trust of disabled users.

Note that `reviews` may be collected either regarding a venue as a whole, or of a particular event within that venue. 

It is advised that systems implementing `review` have some mechanism for moderation of these, rather than automatically publishing these as received. 

### Implementation Example

```text
"review": [
    { "@type": "Review",
      "reviewAspect": "Accessibility",
      "reviewRating": 3,
      "headline": "Friendly staff, but need more training',
      "reviewBody": "Overall, I was very pleased with my experience 
       at ExampleGym: accessibility features were as described, and 
       step-free access is available throughout the entire building. 
       Unfortunately, not all staff are trained in the use of 
       wheelchair lifts, however. They were friendly about it - but
       I ended up having to wait ten or fifteen minutes while they 
       figured out how to use it safely. I did not feel reassured!"
    }
]
```

