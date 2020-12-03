# Accessible Leisure Centre

The following example illustrates a Slot for swimming at a leisure centre equipped with:

* Step-free access to
  * the entrance
  * the reception area
  * all social areas
  * all activity areas
* accessible parking
* accessible toilets
* accessible changing facilities
* accessible emergency exits
* a pool hoist

```text
{
   "@context":[
      "https://openactive.io/",
      "https://openactiove.io/accessibility",
      "https://schema.org/"
   ],
   "type":"FacilityUse",
   "url":"http://www.example.org/facility-use/1",
   "name":"Open Swim",
   "description":"Open swimming without lanes",
   "activity":"Swimming",
   "provider":{
      "type":"Organization",
      "name":"Example Leisure Centre Ltd"
   },
   "location":{
      "type":"Place",
      "name":"Example Leisure Centre",
      "address":{
         "type":"PostalAddress",
         "streetAddress":"1 High Street",
         "addressLocality":"Bristol",
         "addressRegion":"Somerset",
         "postalCode":"BS1 4SD",
         "addressCountry":"GB"
      },
      "carerPolicy":"All persons attending as personal careres for individuals with accessibility needs are permitted into facilities free of charge. They are also entitled to a 50% discount on all items in centre cafés.",
      "contactPoint":{
         "@type":"ContactPoint",
         "contactType":"Accessibility Information",
         "email":"example@example.com",
         "telephone":"0555555555"
      },
      "review":[
         {
            "@type":"Review",
            "reviewAspect":"Accessibility",
            "reviewRating":3,
            "headline":"Friendly staff, but need more training",
            "reviewBody":"Overall, I was very pleased with my experience at ExampleGym: accessibility features were as described, and step-free access is available throughout the entire building. Unfortunately, not all staff are trained in the use of wheelchair lifts, however. They were friendly about it - but I ended up having to wait ten or fifteen minutes while they figured out how to use it safely. I did not feel reassured!"
         }
      ],
      "transportNote":[
         {
            "@type":"TransportNote",
            "transportMode":"Bus",
            "description":"The number 37 Southbound stops outside and across the street from the leisure centre. A pelican crossing with audio signal leads across the four-lane street from the stop directly to the centre entrance"
         },
         {
            "@type":"TransportNote",
            "transportMode":"Rail",
            "description":"The Maiden Valley tram stop is a ten-minute walk from the leisure centre. All crossings en route are wheelchair- accessible, though some gradients are steep."
         }
      ],
      "amenityFeature":[
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Parking",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Changing Facilities",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Toilets",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Emergency Exits",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Reception Area",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Social Areas",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Activity Areas",
            "value":true
         },
         {
            "@type":"LocationFeatureSpecification",
            "name":"Accessible Parking",
            "value":true
         }
      ],
      "accessibilitySupport":[
         {
            "@type":"AccessibilitySupport",
            "name":"Pool Hoist",
            "hoursAvailable":[
               {
                  "opens":"09:00:00",
                  "closes":"20:00:00"
               }
            ]
         }
      ]
   },
   "offers":[
      {
         "type":"Offer",
         "name":"Standard rate",
         "price":10,
         "priceCurrency":"GBP"
      }
   ],
   "event":[
      {
         "type":"Slot",
         "id":"http://www.example.org/facility-use/slots/1",
         "facilityUse":"http://www.example.org/facility-use/1",
         "startDate":"2021-03-01T10:00:00Z",
         "duration":"PT2H",
         "remainingUses":1,
         "maximumUses":20
      },
      {
         "type":"Slot",
         "id":"http://www.example.org/facility-use/slots/2",
         "facilityUse":"http://www.example.org/facility-use/1",
         "startDate":"2021-03-02T11:00:00Z",
         "duration":"PT2H",
         "remainingUses":3,
         "maximumUses":20
      }
   ]
}
```

