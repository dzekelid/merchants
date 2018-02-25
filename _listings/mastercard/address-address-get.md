---
swagger: "2.0"
info:
  title: MasterCard
  description: As a technology company in the global payments business, we operate
    the world&rsquo;s fastest payments processing network, connecting consumers, financial
    institutions, merchants, governments and businesses in more than 210 countries
    and territories. Mastercard&rsquo;s products and solutions make everyday commerce
    activities &ndash; such as shopping, traveling, running a business and managing
    finances &ndash; easier, more secure and more efficient for everyone.
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /address/{address}:
    get:
      summary: Get Address Address
      description: Information about a particular address on the network
      operationId: getAddressAddress
      parameters:
      - in: path
        name: address
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - blockchain
      - address
      - address
definitions:
  AppConfig:
    properties:
      name:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
      definition:
        description: This is a default description.
        type: post
  AppInfo:
    properties:
      name:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
      owner:
        description: This is a default description.
        type: post
      definition:
        description: This is a default description.
        type: post
  AddressInfo:
    properties:
      address:
        description: This is a default description.
        type: post
      owner:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      authority:
        description: This is a default description.
        type: post
  Block:
    properties:
      network:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
      previous_block:
        description: This is a default description.
        type: post
      partitions:
        description: This is a default description.
        type: post
      nonce:
        description: This is a default description.
        type: post
      authority:
        description: This is a default description.
        type: post
      signature:
        description: This is a default description.
        type: post
  NodeInfo:
    properties:
      type:
        description: This is a default description.
        type: post
      services:
        description: This is a default description.
        type: post
      address:
        description: This is a default description.
        type: post
      ip:
        description: This is a default description.
        type: post
      port:
        description: This is a default description.
        type: post
      authority:
        description: This is a default description.
        type: post
      connections:
        description: This is a default description.
        type: post
      last_active:
        description: This is a default description.
        type: post
  DataPartition:
    properties:
      application:
        description: This is a default description.
        type: post
      entries:
        description: This is a default description.
        type: post
      merkle_root:
        description: This is a default description.
        type: post
  EntryRequest:
    properties:
      app:
        description: This is a default description.
        type: post
      encoding:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  EntryResponse:
    properties:
      key:
        description: This is a default description.
        type: post
      slot:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
  EntryInfo:
    properties:
      key:
        description: This is a default description.
        type: post
      slot:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ValidationError:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
      fields:
        description: This is a default description.
        type: post
  AuthorizationError:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  SystemError:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
x-collection-name: MasterCard
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