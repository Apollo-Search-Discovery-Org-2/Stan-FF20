# Onsite Search Performed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Performed",
    "onsiteSearch": {
        "keyword": {
            "searchType": "<searchType>"
        },
        "location": {
            "center": {
                "accuracy": "<accuracy>"
            },
            "map": {
                "zoomLevel": "<zoomLevel>"
            },
            "radius": {
                "unitOfMeasure": "<unitOfMeasure>",
                "value": <value>
            },
            "storeSearchParameters": "<storeSearchParameters>"
        }
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|accuracy|string|A representation of the accuracy of the method that provides the location center.|high, medium, low|||||||
|searchType|string|Describes the domain of the search. |products, properties, articles, authors, coupons, publications|||||||
|storeSearchParameters|string|Captures the city\|state\|zip combination that was used to search for a store||||||||
|unitOfMeasure|string|The unit of measurement|miles, kilometers, meters|||||||
|value|number|The location search radius from the center POI.|2.294694||||0|||
|zoomLevel|string|Indicator of the zoom level in a map presentation. Values are typically integers, but can vary depending on the map service used. |1, 2, 3, 4, 5, 6|||||||




