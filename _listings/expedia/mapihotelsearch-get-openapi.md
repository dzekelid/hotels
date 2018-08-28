---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Search
  description: |-
    Mobile API Hotels Search

    There are multiple successful responses for this operation.
    See the examples below for more information.
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /m/api/hotel/search:
    get:
      summary: Search
      description: |-
        Mobile API Hotels Search

        There are multiple successful responses for this operation.
        See the examples below for more information.
      operationId: hotels-search
      x-api-path-slug: mapihotelsearch-get
      parameters:
      - in: query
        name: airAttachQualificationCode
        description: Qualification code needed to get air attached hotel prices
      - in: query
        name: checkInDate
        description: Check in date in ISO format (yyyy-MM-dd)
      - in: query
        name: checkOutDate
        description: Check out date in ISO format (yyyy-MM-dd)
      - in: query
        name: city
        description: A string to identify the city to search
      - in: query
        name: correlationId
        description: Define a correlation between a hotel search and a flight search
      - in: query
        name: enableSponsoredListings
        description: Used to check for sponsoredListing
      - in: query
        name: filterAmenities
        description: Used to filter by amenities
      - in: query
        name: filterHotelName
        description: Hotel name used to filter the search results
      - in: query
        name: filterInventoryType
        description: A parameter to filter by inventory type
      - in: query
        name: filterPrice
        description: Used to filter by price, make sure it matches filterPriceBuckets
          if counts are desired
      - in: query
        name: filterPriceBuckets
        description: Used to define custom price filter buckets
      - in: query
        name: filterStarRatings
        description: Used to filter by star rating
      - in: query
        name: filterUnavailable
        description: Unavailable hotels will be removed from the response if set to
          true
      - in: query
        name: forceV2Search
        description: A flag to indicate whether the api should do a domain V2 search
          for the mobile app
      - in: query
        name: hgid
        description: If the hotel group ID parameter (hgid) is present it will take
          precedence over city, location or lat/long
      - in: query
        name: latitude
        description: Latitude to be used in combination with longitude for a coordinate
          search
      - in: query
        name: longitude
        description: Longitude to be used in combination with latitude for a coordinate
          search
      - in: query
        name: pageIndex
        description: The zero-based index of the page that you are requesting
      - in: query
        name: regionId
        description: An Expedia region ID to limit the search to a particular region
      - in: query
        name: resultsPerPage
        description: The number of hotels to return per page
      - in: query
        name: returnOpaqueHotels
        description: Return Opaque hotels if set to true
      - in: query
        name: room
        description: '[Optional if room1 field is specified] A Comma Separated Value
          of #OfAdults, followed by childrens ages for all children that are 18 and
          under'
      - in: query
        name: room1
        description: '[Optional if room field is specified] A Comma Separated Value
          of #OfAdults, followed by childrens ages for all children that are 18 and
          under'
      - in: query
        name: sortOrder
        description: Order to sort the list of hotels by Expedia picks, star rating,
          price and guest rating
      - in: query
        name: sortOrderFilter
        description: A post process sort order filter used to apply post sort order
          filtering to the sorted (sortOrder) search results
      - in: query
        name: sourceType
        description: Source type for the request
      - in: query
        name: tripId
        description: This field is optional and will default to the the POS default
          PriceType
      - in: query
        name: vipOnly
        description: Used to filter only VIP type hotels
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Hotels
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---