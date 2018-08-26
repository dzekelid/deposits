---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/settlements:
    get:
      summary: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      description: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      operationId: ListSettlements
      x-api-path-slug: v1location-idsettlements-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list settlements for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      - in: query
        name: status
        description: Provide this parameter to retrieve only settlements with a particular
          status (SENT or FAILED)
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Deposits
      - Withdrawals
      - Initiated
      - By
      - Square
      - To
      - Merchants
      - Bank
      - Account
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
---