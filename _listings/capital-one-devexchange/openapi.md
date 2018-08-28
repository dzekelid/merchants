swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 1
info:
  title: Capital One DevExchange
  description: nessie-is-capital-ones-hackathon-api-that-gives-you-access-to-a-multitude-of-real-publicfacing-data--such-as-atm-and-bank-branch-locations--along-with-mock-customer-account-data--use-http-requests-to-set-up-peertopeer-transactions-simulate-a-weekly-paycheck-or-even-schedule-bills-for-customers-this-is-all-structured-in-a-way-that-resembles-how-we-actually-run-things-here-at-capital-one-
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
    put:
      summary: Update a specific existing merchant
      description: Updates the specific merchant
      operationId: updates-the-specific-merchant
      x-api-path-slug: merchantsid-put
      parameters:
      - in: body
        name: body
        description: Updated merchant object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of merchant that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
  /merchants/{id}/purchases:
    get:
      summary: Get all purchases by merchant
      description: Returns the purchases that a merchant is involved in.
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      x-api-path-slug: merchantsidpurchases-get
      parameters:
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
      - ""
      - Purchases
  /merchants/{id}/accounts/{accountId}/purchases:
    get:
      summary: Get all purchases by account and merchant
      description: Returns the purchases that a merchant is involved in.
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      x-api-path-slug: merchantsidaccountsaccountidpurchases-get
      parameters:
      - in: path
        name: accountId
        description: ID of the account associated with all the purchases
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
      - ""
      - Accounts
      - Account
      - Purchases