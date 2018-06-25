---
name: Expedia
x-slug: expedia
description: Expedia Affiliate Network is the B2B partnership brand of Expedia, Inc.
  Our technology powers the hotel offering of thousands of partners around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
x-kinRank: "9"
x-alexaRank: "197733"
tags: Hotels
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/apis.md
specificationVersion: "0.14"
apis:
- name: Expedia Search
  x-api-slug: expedia
  description: |-
    Mobile API Hotels Search

    There are multiple successful responses for this operation.
    See the examples below for more information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/search
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelsearch-get-openapi.md
- name: Expedia Get Offers
  x-api-slug: expedia
  description: Mobile API Hotels Offers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/offers
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteloffers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteloffers-get-openapi.md
- name: Expedia Get Offers
  x-api-slug: expedia
  description: Mobile API Hotels Offers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/offers/v3
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteloffersv3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteloffersv3-get-openapi.md
- name: Expedia Create A Trip
  x-api-slug: expedia
  description: Mobile API Hotels Create Trip
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/create
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcreate-post-openapi.md
- name: Expedia Checkout
  x-api-slug: expedia
  description: Mobile API Hotels Checkout
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/checkout
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcheckout-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcheckout-post-openapi.md
- name: Expedia Hotel Checkout With JSON Request Body
  x-api-slug: expedia
  description: Mobile API Hotel Checkout V2
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/V2/checkout
  tags: Travel,Hotels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripv2checkout-post-openapi.md
- name: Expedia Get Required Checkout Fields
  x-api-slug: expedia
  description: Service that returns the fields that are required or optional for a
    given point of sale.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/checkoutfields
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcheckoutfields-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcheckoutfields-get-openapi.md
- name: Expedia Cancel Enquiry
  x-api-slug: expedia
  description: Cancel Enquiry for hotel, pass in itinerary id, email address of trip
    owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/cancelEnquiry
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcancelenquiry-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcancelenquiry-get-openapi.md
- name: Expedia Cancel Enquiry
  x-api-slug: expedia
  description: Cancel Enquiry for hotel, pass in itinerary id, email address of trip
    owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/V2/cancelEnquiry
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripv2cancelenquiry-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripv2cancelenquiry-get-openapi.md
- name: Expedia Product
  x-api-slug: expedia
  description: Hotel Product
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/product
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelproduct-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelproduct-get-openapi.md
- name: Expedia Info
  x-api-slug: expedia
  description: Hotel Information
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/info
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelinfo-get-openapi.md
- name: Expedia Cancel Trip
  x-api-slug: expedia
  description: Hotel Trip Cancellation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/trip/cancel
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihoteltripcancel-post-openapi.md
- name: Expedia Cancel Room
  x-api-slug: expedia
  description: Hotel Room Cancellation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/rooms/cancel
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelroomscancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelroomscancel-post-openapi.md
- name: Expedia Get Package Offers
  x-api-slug: expedia
  description: Mobile API Packages
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/packages/hotelOffers
  tags: Travel,Packages,Offers,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/apipackageshoteloffers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/apipackageshoteloffers-get-openapi.md
- name: Expedia Checkout
  x-api-slug: expedia
  description: Mobile API Lx Checkout
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/lx/trip/checkout
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapilxtripcheckout-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapilxtripcheckout-post-openapi.md
- name: Expedia LPAS Search
  x-api-slug: expedia
  description: Mobile API Hotel Search using LPAS
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///m/api/hotel/search/v3
  tags: Travel,Hotels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelsearchv3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/mapihotelsearchv3-get-openapi.md
- name: Expedia
  x-api-slug: expedia
  description: Expedia is the leader in travel and technology and is the worlds largest
    travel company. The EAN Developer Hub gives developers FREE access to our highly
    flexible APIs that power cutting-edge websites, mobile apps, and much more. Some
    of the best travel applications on the market are powered by the EAN API. Learn
    more reasons to partner with EAN by taking a look at our brochure and watching
    our video. The world of travel awaits you!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x/
  tags: Hotels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hotels/master/_listings/expedia/openapi.md
x-common:
- type: x-base
  url: http://api.ean.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/expedia
- type: x-crunchbase
  url: https://crunchbase.com/organization/ean-upc-codes-com
- type: x-documentation
  url: https://www.expedia.com/static/mobile/swaggerui/
- type: x-email
  url: support@ean.com
- type: x-github
  url: https://github.com/Expedia
- type: x-swagger--original
  url: https://www.expedia.com/static/mobile/swaggerui/swagger.json
- type: x-twitter
  url: https://twitter.com/ExpediaEAN
- type: x-website
  url: http://developer.ean.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---