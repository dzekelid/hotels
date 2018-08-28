---
swagger: "2.0"
x-collection-name: TelAPI
x-complete: 0
info:
  title: hetras Hotel API Version 0 Get a list of all the hotels of a chain your application
    has access to.
  version: v0
  description: Get a list of all the hotels of a chain your application has access
    to..
host: api.hetras-certification.net
basePath: /
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