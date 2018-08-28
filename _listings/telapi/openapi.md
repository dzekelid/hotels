swagger: "2.0"
x-collection-name: TelAPI
x-complete: 1
info:
  title: TelAPI
  description: telapi-is-a-rest-api--what-that-means-for-you-is-that-interacting-with-telapi-to-perform-all-of-your-telephony-needs-is-almost-as-simple-as-visiting-a-website--deeper-knowledge-regarding-rest-is-useful-when-developing-with-telapi-but-definitely-not-required--we-aim-to-provide-all-of-the-information-needed-for-working-with-our-rest-api-throughout-its-documentation-provided-here-so-even-if-you-are-new-to-rest-telapi-will-still-be-a-pleasure-to-use-
  termsOfService: http://www.telapi.com/legal/tos
  version: v2
host: api.telapi.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/hotel/v0/hotels:
    get:
      summary: Get a list of all the hotels of a chain your application has access
        to.
      description: Get a list of all the hotels of a chain your application has access
        to..
      operationId: Hotels_GetHotels
      x-api-path-slug: apihotelv0hotels-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      responses:
        200:
          description: OK
      tags:
      - ""
      - Hotels
      - Of
      - Chain
      - Your
      - Application
      - Has
      - Access
      - To
  /api/hotel/v0/hotels/{hotelId}:
    get:
      summary: Get the details of the hotel with the speccified hotel id.
      description: Get the details of the hotel with the speccified hotel id..
      operationId: Hotels_GetHotel
      x-api-path-slug: apihotelv0hotelshotelid-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Hotel
      - Speccified
      - Hotel
      - Id
  /api/hotel/v0/hotels/{hotelId}/codes:
    get:
      summary: Get a list of codes for the specified hotel either filtered by type
        or code.
      description: "With this call you can find codes for a hotel by type or code.
        By default and without any filter criteria\r\n            defined it will
        return you all available codes."
      operationId: Codes_GetCodes
      x-api-path-slug: apihotelv0hotelshotelidcodes-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: code
        description: Return all codes matching the code
      - in: path
        name: hotelId
        description: The hotel id you are trying to find codes for
      - in: query
        name: type
        description: Return all codes available for the specified type
      responses:
        200:
          description: OK
      tags:
      - Codesthe
      - Specified
      - Hotel
      - Either
      - Filtered
      - By
      - Type
      - Code
  /api/hotel/v0/hotels/{hotelId}/codes/{id}:
    get:
      summary: Get all the details for a specific code available for the hotel.
      description: Read the details about a specific code available for the defined
        hotel.
      operationId: Codes_GetCode
      x-api-path-slug: apihotelv0hotelshotelidcodesid-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the code available for
      - in: path
        name: id
        description: The code identifier you want to see details for
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Code
      - Availablethe
      - Hotel
  /api/hotel/v0/hotels/{hotelId}/rateplans:
    get:
      summary: Get a list of rateplans for the specified hotel id matching the filter
        criteria.
      description: "With this call you can find rateplans for a hotel by different
        filters. By default and without any filter criteria\r\n            defined
        it will return you all active rateplans."
      operationId: RatePlans_GetRateplans
      x-api-path-slug: apihotelv0hotelshotelidrateplans-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: baseRateplan
        description: Return all rateplans having the specified rateplan as base rateplan
      - in: query
        name: channelCode
        description: Return all rateplans sold through the specified channel
      - in: query
        name: channelGroup
        description: Return all rateplans that are sold through at least one channel
          out of the specified channel group
      - in: query
        name: commissionable
        description: Return all rateplans having commisionable status
      - in: query
        name: group
        description: Return all rateplans belonging to the specified rateplan group
      - in: path
        name: hotelId
        description: The hotel id you are trying to find rateplans for
      - in: query
        name: includedServices
        description: Return all rateplans having at least one of the specified services
          included
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: marketCodes
        description: Return all rateplans having one of the specified values as a
          market code
      - in: query
        name: roomTypes
        description: Return all rateplans by which at least one of the specified room
          types are sold
      - in: query
        name: sellingStatus
        description: Specify which rateplans to return
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: top
        description: Amount of items to select
      responses:
        200:
          description: OK
      tags:
      - Rateplansthe
      - Specified
      - Hotel
      - Id
      - Matching
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rateplans/$count:
    get:
      summary: Get the count of all rateplans in the hotel matching the given filter
        criteria.
      description: Get the count of all rateplans in the hotel matching the given
        filter criteria..
      operationId: RatePlans_GetRateplansCount
      x-api-path-slug: apihotelv0hotelshotelidrateplanscount-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: baseRateplan
        description: Return all rateplans having the specified rateplan as base rateplan
      - in: query
        name: channelCode
        description: Return all rateplans sold through the specified channel
      - in: query
        name: channelGroup
        description: Return all rateplans that are sold through at least one channel
          out of the specified channel group
      - in: query
        name: commissionable
        description: Return all rateplans having commisionable status
      - in: query
        name: group
        description: Return all rateplans belonging to the specified rateplan group
      - in: path
        name: hotelId
        description: The hotel you are counting the rateplans for
      - in: query
        name: includedServices
        description: Return all rateplans having at least one of the specified services
          included
      - in: query
        name: marketCodes
        description: Return all rateplans having one of the specified values as a
          market code
      - in: query
        name: roomTypes
        description: Return all rateplans by which at least one of the specified room
          types are sold
      - in: query
        name: sellingStatus
        description: Specify which rateplans to return
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Rateplans
      - In
      - Hotel
      - Matching
      - Given
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}:
    get:
      summary: Get all the details for a specific rateplan in the hotel.
      description: Read the details about a specific rateplan for the defined hotel.
      operationId: RatePlans_GetRateplan
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancode-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to see details for
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Rateplan
      - In
      - Hotel
  /api/hotel/v0/hotels/{hotelId}/room_types:
    get:
      summary: Get a list with the details of all room types for for the specified
        hotel id.
      description: With this call you can load the details about a all available room
        types for the specified hotel.
      operationId: RoomTypes_GetRoomTypes
      x-api-path-slug: apihotelv0hotelshotelidroom-types-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - ""
      - Room
      - Typesfor
      - Specified
      - Hotel
      - Id
  /api/hotel/v0/hotels/{hotelId}/room_types/{code}:
    get:
      summary: Get all the details for a specific room type in the hotel.
      description: With this call you can load the details about a specific room type
        in the hotel.
      operationId: RoomTypes_GetRoomType
      x-api-path-slug: apihotelv0hotelshotelidroom-typescode-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: code
        description: The code of the room type you want to see details for
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Room
      - Type
      - In
      - Hotel
  /api/hotel/v0/hotels/{hotelId}/rooms/$count:
    get:
      summary: Get the count of all rooms in the hotel matching the given filter criteria.
      description: Get the count of all rooms in the hotel matching the given filter
        criteria..
      operationId: Rooms_GetRoomsCount
      x-api-path-slug: apihotelv0hotelshotelidroomscount-get
      parameters:
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: conditions
        description: Return results only for rooms that have the given room condition
          status
      - in: path
        name: hotelId
        description: The hotel you are counting the rooms for
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: maintenances
        description: Return results only for rooms that have the given maintenance
          status
      - in: query
        name: occupancy
        description: Return results only for rooms that have the given frontdesk ocuppancy
          status
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Rooms
      - In
      - Hotel
      - Matching
      - Given
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rooms/{roomNumber}:
    get:
      summary: Get all the details for a specific room in the hotel.
      description: With this call you can load the details about a specific room in
        the hotel. It will show you the current status of the room.
      operationId: Rooms_GetRoom
      x-api-path-slug: apihotelv0hotelshotelidroomsroomnumber-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the room belongs to
      - in: path
        name: roomNumber
        description: The room number you want to see details for
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Room
      - In
      - Hotel