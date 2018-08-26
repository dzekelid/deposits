---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Get Deposit Crypro Address
  description: Get deposit crypro address.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/crypto/address/{currency}:
    get:
      summary: Get Deposit Crypro Address
      description: Get deposit crypro address.
      operationId: getAccountCryptoAddressCurrency
      x-api-path-slug: accountcryptoaddresscurrency-get
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - Deposit
      - Crypro
      - Address
    post:
      summary: Create New Deposit Crypro Address
      description: Create new deposit crypro address.
      operationId: postAccountCryptoAddressCurrency
      x-api-path-slug: accountcryptoaddresscurrency-post
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - New
      - Deposit
      - Crypro
      - Address
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