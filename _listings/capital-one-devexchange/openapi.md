---
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
    put:
      summary: Update a specific existing deposit
      description: Updates the specific deposit
      operationId: updates-the-specific-deposit
      x-api-path-slug: depositsid-put
      parameters:
      - in: body
        name: body
        description: deposit to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the deposit that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Deposits
    delete:
      summary: Delete a specific existing deposit
      description: Deletes the specific deposit
      operationId: deletes-the-specific-deposit
      x-api-path-slug: depositsid-delete
      parameters:
      - in: path
        name: id
        description: ID of the deposit that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Deposits
---