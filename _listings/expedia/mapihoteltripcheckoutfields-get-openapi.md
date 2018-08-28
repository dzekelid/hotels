---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Get Required Checkout Fields
  description: Service that returns the fields that are required or optional for a
    given point of sale.
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
  /m/api/hotel/offers:
    get:
      summary: Get Offers
      description: Mobile API Hotels Offers
      operationId: hotels-offers
      x-api-path-slug: mapihoteloffers-get
      parameters:
      - in: query
        name: checkInDate
        description: Checkin Date
      - in: query
        name: checkOutDate
        description: Checkout Date
      - in: query
        name: hotelId
        description: a 32-bit integer, currently between 1 through 7 digit number
      - in: query
        name: priceType
        description: Price Type, can only be TOTAL_PRICE or BASE_PRICE_ONLY
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
        name: sourceType
        description: Source Type, for example mobilweb or mobileapp
      - in: query
        name: useCacheForAirAttach
        description: '[Optional] If this flag is set then the hotel offers (on a successful
          offers call) and the search fields will be cached'
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Hotels
  /m/api/hotel/offers/v3:
    get:
      summary: Get Offers
      description: Mobile API Hotels Offers
      operationId: hotels-offers
      x-api-path-slug: mapihoteloffersv3-get
      parameters:
      - in: query
        name: checkInDate
        description: Checkin Date
      - in: query
        name: checkOutDate
        description: Checkout Date
      - in: query
        name: hotelId
        description: a 32-bit integer, currently between 1 through 7 digit number
      - in: query
        name: priceType
        description: Price Type, can only be TOTAL_PRICE or BASE_PRICE_ONLY
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
        name: sourceType
        description: Source Type, for example mobilweb or mobileapp
      - in: query
        name: useCacheForAirAttach
        description: '[Optional] If this flag is set then the hotel offers (on a successful
          offers call) and the search fields will be cached'
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Hotels
  /m/api/hotel/trip/create:
    post:
      summary: Create A Trip
      description: Mobile API Hotels Create Trip
      operationId: hotels-create-trip
      x-api-path-slug: mapihoteltripcreate-post
      parameters:
      - in: formData
        name: productKey
        description: The product key, obtained by calling /m/api/hotel/offers,  we
          are going to create a trip for
      - in: formData
        name: qualifyAirAttach
        description: '[Optional] Whether to return a qualified air attach product
          for this trip'
      - in: formData
        name: roomInfoFields[0].room
        description: 'A Comma Separated Value of #OfAdults, followed by childrens
          ages for all children that are 18 and under'
      - in: formData
        name: tripTitle
        description: '[Optional] The name of this itinerary as it will appear to customer
          service and in the itinerary list'
      - in: formData
        name: withInsurance
        description: '[Optional] Whether to return the available insurance options
          for this trip'
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Hotels
  /m/api/hotel/trip/checkout:
    post:
      summary: Checkout
      description: Mobile API Hotels Checkout
      operationId: hotels-checkout
      x-api-path-slug: mapihoteltripcheckout-post
      parameters:
      - in: formData
        name: bedTypeId
        description: Parameter that indicates the selected bed Type
      - in: formData
        name: checkInDate
        description: Check in date in ISO format (yyyy-MM-dd)
      - in: formData
        name: checkOutDate
        description: Check out date in ISO format (yyyy-MM-DD)
      - in: formData
        name: city
        description: The city of the travelers billing address
      - in: formData
        name: country
        description: The 3 letter country code of the travelers billing address
      - in: formData
        name: creditCardNumber
        description: The credit card number used for this booking, if checking out
          with a new card
      - in: formData
        name: cvv
        description: The CVV of the travelers credit card used for this booking
      - in: formData
        name: doIThinkImSignedIn
        description: As a client I am checking-out with the assumption that I am signed
          in
      - in: formData
        name: email
        description: This passengers email address
      - in: formData
        name: expectedCardFee
        description: The expected credit card fee, as returned by the createTrip call
          in the validFormsOfPayment object for whatever credit card the user is paying
          with
      - in: formData
        name: expectedCardFeeCurrencyCode
        description: Three letter 4217 ISO currency code of the expected total price
      - in: formData
        name: expectedFareCurrencyCode
        description: Three letter 4217 ISO currency code of the expected credit card
          fee
      - in: formData
        name: expectedTotalFare
        description: The expected total price of the trip, matching exactly whatever
          the user last saw
      - in: formData
        name: expediaEmailOptIn
        description: Whether to opt-in the users email to travel deals
      - in: formData
        name: expirationDateMonth
        description: The expiration date month of the credit card used for this booking
      - in: formData
        name: expirationDateYear
        description: The 4 digit expiration date year of the credit card used for
          this booking
      - in: formData
        name: firstName
        description: The first name of the traveler
      - in: formData
        name: lastName
        description: The last name of the traveler
      - in: formData
        name: middleName
        description: The middle name of the traveler
      - in: formData
        name: nameOnCard
        description: The card holders name
      - in: formData
        name: omniturePartnerId
        description: Omniture partner identification string
      - in: formData
        name: password
        description: The password provided by the expedia user
      - in: formData
        name: phone
        description: The phone number of the traveler
      - in: formData
        name: phoneCountryCode
        description: The country code of the phone number of the traveler
      - in: formData
        name: postalCode
        description: The postal code of the travelers billing address
      - in: formData
        name: prettyPrint
        description: If true, return JSON with tabs, spaces and newlines to be human
          readable
      - in: formData
        name: rooms
        description: A list of room preferences to be applied to the rooms being booked
      - in: formData
        name: rooms[0].accessibilityOptionIds
        description: A Comma Separated Value of accessibility option Ids
      - in: formData
        name: rooms[0].specialRequests
        description: A text field for special requests
      - in: formData
        name: sendEmailConfirmation
        description: Used to check if confirmation email needs to be sent or not
      - in: formData
        name: state
        description: The state (or province) of the travelers billing address
      - in: formData
        name: storeCreditCardInUserProfile
        description: Indicates whether to save the credit card information as a stored
          credit card in the user profile
      - in: formData
        name: storedCreditCardId
        description: The GUID for the stored credit card information to be used for
          payment
      - in: formData
        name: streetAddress
        description: The street part of the credit card owners billing address
      - in: formData
        name: streetAddress2
        description: Apartment or suite number of the travelers billing address
      - in: formData
        name: suppressFinalBooking
        description: If true, do not actually charge for and book the trip, stop after
          creating the itinerary
      - in: formData
        name: tealeafTransactionId
        description: The unique transaction ID used in TeaLeaf PSR tracking
      - in: formData
        name: tripId
        description: The trip ID of an existing trip, from /m/api/hotel/trip/create
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Hotels
  /m/api/hotel/trip/V2/checkout:
    post:
      summary: Hotel Checkout With JSON Request Body
      description: Mobile API Hotel Checkout V2
      operationId: checkoutV2
      x-api-path-slug: mapihoteltripv2checkout-post
      parameters:
      - in: body
        name: body
        description: JSON body with all the fields required for a Hotel checkout
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Hotels
  /m/api/hotel/trip/checkoutfields:
    get:
      summary: Get Required Checkout Fields
      description: Service that returns the fields that are required or optional for
        a given point of sale.
      operationId: hotels-checkout-fields
      x-api-path-slug: mapihoteltripcheckoutfields-get
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