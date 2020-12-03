# Chair Yoga

The following JSON object models a yoga session conducted seated in a chair and intended both for wheelchair users and for those whose chronic health conditions limit their mobility and degree of exertion.

```text
{
   "@context":[
      "https://openactive.io/",
      "https://openactiove.io/accessibility",
      "https://schema.org/"
   ],
   "type":"SessionSeries",
   "url":"http://www.example.org/events/1",
   "name":"Chair Yoga",
   "description":"Chair Yoga is yoga adapted to a seated position, for individuals who want a full yoga workout but with mobility restrictions that prevent them from supporting themselves for long periods",
   "accessibilitySupportLevel":"Accessibility Needs Only",
   "contactPoint":{
      "@type":"ContactPoint",
      "contactType":"Accessibility Information",
      "email":"example@example.com",
      "telephone":"0555555555"
   },
   "carerPolicy":"Individuals attending in the capacity of carer are admitted and may participate free of charge.",
   "location":{
      "type":"Place",
      "name":"Example Community Hall",
      "address":{
         "type":"PostalAddress",
         "streetAddress":"1 High Street",
         "addressLocality":"Bristol",
         "addressRegion":"Somerset",
         "postalCode":"BS1 4SD",
         "addressCountry":"GB"
      }
   },
   "transportNote":[
      {
         "@type":"TransportNote",
         "transportMode":"Bus",
         "description":"The number 37 Southbound stops outside and across the street from the leisure centre. A pelican crossing with audio signal leads across the four-lane street from the stop directly to the centre entrance"
      }
   ],
   "accessibilitySupport":{
      "@type":"AccessibilitySupport",
      "name":"Inclusion Support",
      "description":"The instructors of Chair Yoga are aware that mobility problems are often associated with other physical conditions, such as breathing difficult, chronic pain, etc. If you feel you need additional support to participate in Chair Yoga, our instructors will be on hand to instruct and guide you. All poses are designed to be adaptable as required.",
      "participantConditionSupported":[
         {
            "@type":"Concept",
            "@id":"https://openactive.io/accessibility/pcs/_ff9a09ed-fb5a-4a62-b4d7-0fa263aa631d",
            "prefLabel":"Physical Impairment"
         },
         {
            "@type":"Concept",
            "@id":"https://openactive.io/accessibility/pcs/_e2f6e425-66b0-4c74-b843-d3dbc634b99",
            "prefLabel":"Pregnancy Support"
         }
      ]
   },
   "eventSchedule":[
      {
         "type":"Schedule",
         "startDate":"2021-01-01",
         "endDate":"2021-12-31",
         "repeatFrequency":"P1W",
         "byDay":[
            "https://schema.org/Wednesday"
         ],
         "startTime":"19:00",
         "endTime":"20:00",
         "duration":"PT1H",
         "scheduledEventType":"ScheduledSession"
      }
   ]
}
```

