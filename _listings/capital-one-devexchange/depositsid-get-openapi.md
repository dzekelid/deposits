---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Get deposit by id
  description: Returns the deposit with the specific id
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
  /accounts/{id}/deposits:
    get:
      summary: Get all deposits
      description: Returns the deposits that you are involved in.
      operationId: returns-the-deposits-that-you-are-involved-in
      x-api-path-slug: accountsiddeposits-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the deposit
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Deposits
    post:
      summary: Create a deposit
      description: Creates a deposit where the account with the ID specified receives
        the amount.
      operationId: creates-a-deposit-where-the-account-with-the-id-specified-receives-the-amount
      x-api-path-slug: accountsiddeposits-post
      parameters:
      - in: body
        name: body
        description: Deposit to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account receiver of deposit
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Deposits
  /deposits/{id}:
    get:
      summary: Get deposit by id
      description: Returns the deposit with the specific id
      operationId: returns-the-deposit-with-the-specific-id
      x-api-path-slug: depositsid-get
      parameters:
      - in: path
        name: id
        description: ID of the deposit that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Deposits
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