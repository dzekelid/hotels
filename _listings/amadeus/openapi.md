swagger: "2.0"
x-collection-name: Amadeus
x-complete: 1
info:
  title: Amadeus
  description: amadeus-api-is-a-toolkit-designed-for-travel-agencies-who-want-to-develop-their-own-travel-products-rather-than-using-offtheshelf-solutions--with-this-tool-you-can-build-your-very-own-customised-applications-that-link-in-a-stable-and-secure-dialogue-with-our-global-distribution-system-gds-
  contact:
    name: Amadeus Innovation and Research
    url: https://sandbox.amadeus.com
  version: 1.0.0
host: api.sandbox.amadeus.com
basePath: /v1.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hotels/search-airport:
    get:
      summary: Get Hotels Search Airport
      description: |-
        A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

        This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
      operationId: getHotelsSearchAirport
      x-api-path-slug: hotelssearchairport-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: location
        description: IATA airport code for hotel availability is required requested
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Airport
  /hotels/search-box:
    get:
      summary: Get Hotels Search Box
      description: "A fast Hotel shopping API to see which hotels are available in
        a given area, on a given day and displays their lowest prices. With this API
        you can find out the price of the cheapest daily rate for all hotels within
        a specified geographical region.\n\nThis API allows you to quickly see the
        hotel locations in a region, and what prices in that area look like,  as well
        as the check-in and check-out dates, and get a list of up to 140 properties
        (names, codes, image, amenities) with their locations and rates. Optional
        parameters such as currency and maximum rates, amenities or hotel chain codes
        are also available and can be used to narrow down the results. More optional
        parameters such as show_sold_out & rooms can be used to show sold out rooms
        and all available rooms.\n            \nThe API is based on our high-speed
        hotel pricing cache, which is also used to power the Amadeus Hotel Search
        Engine application. Results are returned very quickly, response times are
        generally under 2s. Our cache has great global coverage and is constantly
        refreshed with the latest prices."
      operationId: getHotelsSearchBox
      x-api-path-slug: hotelssearchbox-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: north_east_corner
        description: The coordinates of the north-east corner of the search box
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      - in: query
        name: south_west_corner
        description: The coordinates of the south-west corner of the search box
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Box
  /hotels/search-circle:
    get:
      summary: Get Hotels Search Circle
      description: "A fast Hotel shopping API to see which hotels are available in
        a given area, on a given day and displays their lowest prices. With this API
        you can find out the price of the cheapest daily rate for all hotels within
        a specified radius of a point.\n\nThis API allows you to quickly see the hotel
        locations in a region, and what prices in that area look like,  as well as
        the check-in and check-out dates, and get list of up to 140 properties (names,
        codes, image, amenities) with their locations and rates. Optional parameters
        such as currency and maximum rates, amenities or hotel chain codes are also
        available and can be used to narrow down the results. More optional parameters
        such as show_sold_out & rooms can be used to show sold out rooms and all available
        rooms. \n\nThe API is based on our high-speed hotel pricing cache, which is
        also used to power the Amadeus Hotel Search Engine application. Results are
        returned very quickly, response times are generally under 2s. Our cache has
        great global coverage and is constantly refreshed with the latest prices."
      operationId: getHotelsSearchCircle
      x-api-path-slug: hotelssearchcircle-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: latitude
        description: Latitude of the center of the search
      - in: query
        name: longitude
        description: Longitude of the center of the search
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Circle
  /hotels/{property_code}:
    get:
      summary: Get Hotels Property Code
      description: "This API allows you to quickly see the detailed information of
        a single hotel, including descriptions, address, GPS location, amenities,
        awards, lowest priced room and all room prices and booking information. \n\nThis
        API gives you more information on a specific property. Optional parameters
        such as show_sold_out & rooms can be used to show sold out rooms and all available
        rooms. \n\nThe API is based on our high-speed hotel pricing cache, which is
        also used to power the Amadeus Hotel Search Engine application. Results are
        returned very quickly, response times are generally under 2s. Our cache has
        great global coverage and is constantly refreshed with the latest prices."
      operationId: getHotelsPropertyCode
      x-api-path-slug: hotelsproperty-code-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: path
        name: property_code
        description: A Hotel property code based on 2 letter chain code + 3 letter
          IATA code of the city + 3 char property unique id
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Property
      - Code