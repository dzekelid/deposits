---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
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
---