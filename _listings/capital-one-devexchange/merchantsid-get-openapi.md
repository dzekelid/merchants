---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Get merchant by id
  description: Returns the merchant with the specific id
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /merchants:
    get:
      summary: Get all merchants
      description: Returns the merchants that have been assigned to you.
      operationId: returns-the-merchants-that-have-been-assigned-to-you
      x-api-path-slug: merchants-get
      parameters:
      - in: query
        name: lat
        description: Latitude of where youre looking for a merchant
      - in: query
        name: lng
        description: Longitude of where youre looking for a merchant
      - in: query
        name: rad
        description: Search radius in miles
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
    post:
      summary: Create a merchant
      description: Creates a merchant
      operationId: creates-a-merchant
      x-api-path-slug: merchants-post
      parameters:
      - in: body
        name: body
        description: Merchant to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
  /merchants/{id}:
    get:
      summary: Get merchant by id
      description: Returns the merchant with the specific id
      operationId: returns-the-merchant-with-the-specific-id
      x-api-path-slug: merchantsid-get
      parameters:
      - in: path
        name: id
        description: ID of merchant that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
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