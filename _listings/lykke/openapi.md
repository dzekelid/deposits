---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Wallets/depositaddress/{assetId}:
    post:
      summary: Add API Wallets Depositaddress Asset
      description: Add api wallets depositaddress asset.
      operationId: ApiWalletsDepositaddressByAssetIdPost
      x-api-path-slug: apiwalletsdepositaddressassetid-post
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Wallets
      - Depositaddress
      - Asset
---