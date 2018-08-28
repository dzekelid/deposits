---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Wallets Depositaddress Asset
  version: 1.0.0
  description: Add api wallets depositaddress asset.
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