---
swagger: "2.0"
info:
  title: Capital One DevExchange
  description: Nessie is Capital One&rsquo;s Hackathon API that gives you access to
    a multitude of real public-facing data - such as ATM and bank branch locations
    - along with mock customer account data. Use HTTP requests to set up peer-to-peer
    transactions, simulate a weekly paycheck, or even schedule bills for customers!
    This is all structured in a way that resembles how we actually run things here
    at Capital One.
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
  /merchants/{id}/purchases:
    get:
      summary: Get all purchases by merchant
      description: Returns the purchases that a merchant is involved in
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      parameters:
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - banks
      - merchants
      - ""
      - purchases
definitions:
  account:
    properties:
      _id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      rewards:
        description: This is a default description.
        type: delete
      balance:
        description: This is a default description.
        type: delete
      account_number:
        description: This is a default description.
        type: delete
      customer_id:
        description: This is a default description.
        type: delete
  account-put:
    properties:
      nickname:
        description: This is a default description.
        type: delete
      account_number:
        description: This is a default description.
        type: delete
  account-post:
    properties:
      type:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      rewards:
        description: This is a default description.
        type: delete
      balance:
        description: This is a default description.
        type: delete
      account_number:
        description: This is a default description.
        type: delete
  address:
    properties:
      street_number:
        description: This is a default description.
        type: delete
      street_name:
        description: This is a default description.
        type: delete
      city:
        description: This is a default description.
        type: delete
      state:
        description: This is a default description.
        type: delete
      zip:
        description: This is a default description.
        type: delete
  atm:
    properties:
      _id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      language_list:
        description: This is a default description.
        type: delete
      hours:
        description: This is a default description.
        type: delete
      accessibility:
        description: This is a default description.
        type: delete
      amount_left:
        description: This is a default description.
        type: delete
  bill:
    properties:
      _id:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      payee:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      creation_date:
        description: This is a default description.
        type: delete
      payment_date:
        description: This is a default description.
        type: delete
      recurring_date:
        description: This is a default description.
        type: delete
      upcoming_payment_date:
        description: This is a default description.
        type: delete
      payment_amount:
        description: This is a default description.
        type: delete
      account_id:
        description: This is a default description.
        type: delete
  bill-put:
    properties:
      status:
        description: This is a default description.
        type: delete
      payee:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      payment_date:
        description: This is a default description.
        type: delete
      recurring_date:
        description: This is a default description.
        type: delete
      payment_amount:
        description: This is a default description.
        type: delete
  bill-post:
    properties:
      status:
        description: This is a default description.
        type: delete
      payee:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      payment_date:
        description: This is a default description.
        type: delete
      recurring_date:
        description: This is a default description.
        type: delete
      payment_amount:
        description: This is a default description.
        type: delete
  branch:
    properties:
      _id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      hours:
        description: This is a default description.
        type: delete
      phone_number:
        description: This is a default description.
        type: delete
  customer:
    properties:
      _id:
        description: This is a default description.
        type: delete
      first_name:
        description: This is a default description.
        type: delete
      last_name:
        description: This is a default description.
        type: delete
  customer-put:
    properties: []
  customer-post:
    properties:
      first_name:
        description: This is a default description.
        type: delete
      last_name:
        description: This is a default description.
        type: delete
  deposit:
    properties:
      _id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      transaction_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      payee_id:
        description: This is a default description.
        type: delete
      medium:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  deposit-put:
    properties:
      medium:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  deposit-post:
    properties:
      medium:
        description: This is a default description.
        type: delete
      transaction_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  error:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
      fields:
        description: This is a default description.
        type: delete
  geocode:
    properties:
      lat:
        description: This is a default description.
        type: delete
      lng:
        description: This is a default description.
        type: delete
  loan:
    properties:
      _id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      creation_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      credit_score:
        description: This is a default description.
        type: delete
      monthly_payment:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  loan-put:
    properties:
      type:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      credit_score:
        description: This is a default description.
        type: delete
      monthly_payment:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
  loan-post:
    properties:
      type:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      credit_score:
        description: This is a default description.
        type: delete
      monthly_payment:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  merchant:
    properties:
      _id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      category:
        description: This is a default description.
        type: delete
  merchant-put-post:
    properties:
      name:
        description: This is a default description.
        type: delete
      category:
        description: This is a default description.
        type: delete
  customer-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  account-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  bill-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  deposit-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  merchant-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  purchase-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  loan-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  transfer-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  withdrawal-post-success:
    properties:
      code:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
  purchase:
    properties:
      _id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      merchant_id:
        description: This is a default description.
        type: delete
      payer_id:
        description: This is a default description.
        type: delete
      purchase_date:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      medium:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  purchase-put:
    properties:
      payer_id:
        description: This is a default description.
        type: delete
      medium:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  purchase-post:
    properties:
      merchant_id:
        description: This is a default description.
        type: delete
      medium:
        description: This is a default description.
        type: delete
      purchase_date:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  transfer:
    properties:
      _id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      transaction_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      medium:
        description: This is a default description.
        type: delete
      payer_id:
        description: This is a default description.
        type: delete
      payee_id:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  transfer-put:
    properties:
      medium:
        description: This is a default description.
        type: delete
      payee_id:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  transfer-post:
    properties:
      medium:
        description: This is a default description.
        type: delete
      payee_id:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      transaction_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  withdrawal:
    properties:
      _id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      transaction_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      payer_id:
        description: This is a default description.
        type: delete
      medium:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  withdrawal-put:
    properties:
      medium:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  withdrawal-post:
    properties:
      medium:
        description: This is a default description.
        type: delete
      transaction_date:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      amount:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
x-collection-name: Capital One DevExchange
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