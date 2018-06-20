---
name: Amadeus
x-slug: amadeus
description: Amadeus travel technology helps businesses connect to the global travel
  ecosystem, manage operations more effectively and serve travellers better than ever
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
x-kinRank: "8"
x-alexaRank: "4309"
tags: Hotels
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/apis.md
specificationVersion: "0.14"
apis:
- name: Amadeus Get Hotels Search Airport
  x-api-slug: amadeus
  description: |-
    A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

    This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/search-airport
  tags: Hotels, Search, Airport
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelssearchairport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelssearchairport-get-openapi.md
- name: Amadeus Get Hotels Search Box
  x-api-slug: amadeus
  description: "A fast Hotel shopping API to see which hotels are available in a given
    area, on a given day and displays their lowest prices. With this API you can find
    out the price of the cheapest daily rate for all hotels within a specified geographical
    region.\n\nThis API allows you to quickly see the hotel locations in a region,
    and what prices in that area look like,  as well as the check-in and check-out
    dates, and get a list of up to 140 properties (names, codes, image, amenities)
    with their locations and rates. Optional parameters such as currency and maximum
    rates, amenities or hotel chain codes are also available and can be used to narrow
    down the results. More optional parameters such as show_sold_out & rooms can be
    used to show sold out rooms and all available rooms.\n            \nThe API is
    based on our high-speed hotel pricing cache, which is also used to power the Amadeus
    Hotel Search Engine application. Results are returned very quickly, response times
    are generally under 2s. Our cache has great global coverage and is constantly
    refreshed with the latest prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/search-box
  tags: Hotels, Search, Box
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelssearchbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelssearchbox-get-openapi.md
- name: Amadeus Get Hotels Search Circle
  x-api-slug: amadeus
  description: "A fast Hotel shopping API to see which hotels are available in a given
    area, on a given day and displays their lowest prices. With this API you can find
    out the price of the cheapest daily rate for all hotels within a specified radius
    of a point.\n\nThis API allows you to quickly see the hotel locations in a region,
    and what prices in that area look like,  as well as the check-in and check-out
    dates, and get list of up to 140 properties (names, codes, image, amenities) with
    their locations and rates. Optional parameters such as currency and maximum rates,
    amenities or hotel chain codes are also available and can be used to narrow down
    the results. More optional parameters such as show_sold_out & rooms can be used
    to show sold out rooms and all available rooms. \n\nThe API is based on our high-speed
    hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine
    application. Results are returned very quickly, response times are generally under
    2s. Our cache has great global coverage and is constantly refreshed with the latest
    prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/search-circle
  tags: Hotels, Search, Circle
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelssearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelssearchcircle-get-openapi.md
- name: Amadeus Get Hotels Property Code
  x-api-slug: amadeus
  description: "This API allows you to quickly see the detailed information of a single
    hotel, including descriptions, address, GPS location, amenities, awards, lowest
    priced room and all room prices and booking information. \n\nThis API gives you
    more information on a specific property. Optional parameters such as show_sold_out
    & rooms can be used to show sold out rooms and all available rooms. \n\nThe API
    is based on our high-speed hotel pricing cache, which is also used to power the
    Amadeus Hotel Search Engine application. Results are returned very quickly, response
    times are generally under 2s. Our cache has great global coverage and is constantly
    refreshed with the latest prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/{property_code}
  tags: Hotels, Property, Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelsproperty-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/hotelsproperty-code-get-openapi.md
- name: Amadeus
  x-api-slug: amadeus
  description: Amadeus travel technology helps businesses connect to the global travel
    ecosystem, manage operations more effectively and serve travellers better than
    ever
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Hotels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/amadeus/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/amadeus
- type: x-documentation
  url: https://sandbox.amadeus.com/api-catalog
- type: x-github
  url: https://github.com/AmadeusITGroup
- type: x-privacy-policy
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-sandbox
  url: https://sandbox.amadeus.com
- type: x-twitter
  url: https://twitter.com/amadeusinnov
- type: x-website
  url: https://amadeus.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---