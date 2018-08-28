---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Transfer funds between bank accounts (also Deposit Cash/Cheques from
    Cash Held)
  version: 1.0.0
  description: Transfer funds between bank accounts (also deposit cash/cheques from
    cash held).
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/{id}/deposits:
    get:
      summary: Get Deposits processed for an Account
      description: Get deposits processed for an account.
      operationId: Account_GetDepositsByid
      x-api-path-slug: apiaccountiddeposits-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Deposits
      - Processedan
      - Account
  /api/deposit/allocate:
    post:
      summary: Receipt (optional) and allocate deposit funds to holding account
      description: Receipt (optional) and allocate deposit funds to holding account.
      operationId: Deposit_ReceiptAndAllocateDepositBymoveDataContract
      x-api-path-slug: apidepositallocate-post
      parameters:
      - in: body
        name: moveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Receipt
      - (optional)
      - Ocate
      - Deposit
      - Funds
      - To
      - Holding
      - Account
  /api/role/lettings/{id}/setdeposit:
    post:
      summary: Sets the deposit on a letting role
      description: Sets the deposit on a letting role.
      operationId: LettingRole_SetDepositByidBydatacontract
      x-api-path-slug: apirolelettingsidsetdeposit-post
      parameters:
      - in: body
        name: datacontract
        description: The deposit to set on the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Deposit
      - "On"
      - Letting
      - Role
  /api/progression/lettings/{id}/setdeposit:
    post:
      summary: Sets the deposit on a letting role
      description: Sets the deposit on a letting role.
      operationId: LettingsProgression_SetDepositByidBydatacontract
      x-api-path-slug: apiprogressionlettingsidsetdeposit-post
      parameters:
      - in: body
        name: datacontract
        description: The deposit to set on the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Deposit
      - "On"
      - Letting
      - Role
  /api/progression/lettings/{id}/setfurnishinglevel:
    post:
      summary: Sets the deposit on a letting role
      description: Sets the deposit on a letting role.
      operationId: LettingsProgression_SetFurnishingLevelByidBydatacontract
      x-api-path-slug: apiprogressionlettingsidsetfurnishinglevel-post
      parameters:
      - in: body
        name: datacontract
        description: The deposit to set on the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Deposit
      - "On"
      - Letting
      - Role
  /api/role/{id}/payholdingdeposit:
    post:
      summary: Pay funds against holding deposit
      description: Pay funds against holding deposit.
      operationId: Role_PayHoldingDepositByidBypayHoldingDepositDataContract
      x-api-path-slug: apiroleidpayholdingdeposit-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payHoldingDepositDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Funds
      - Against
      - Holding
      - Deposit
  /api/role/{id}/removeholdingdeposit:
    post:
      summary: Remove holding deposit from role
      description: Remove holding deposit from role.
      operationId: Role_RemoveHoldingDepositByidByrelatedRoleId
      x-api-path-slug: apiroleidremoveholdingdeposit-post
      parameters:
      - in: path
        name: id
      - in: query
        name: relatedRoleId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Holding
      - Deposit
      - From
      - Role
  /api/transfer/interaccount:
    post:
      summary: Transfer funds between bank accounts (also Deposit Cash/Cheques from
        Cash Held)
      description: Transfer funds between bank accounts (also deposit cash/cheques
        from cash held).
      operationId: Transfer_ProcessIatByiatDataContract
      x-api-path-slug: apitransferinteraccount-post
      parameters:
      - in: body
        name: iatDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Transfer
      - Funds
      - Between
      - Bank
      - Accounts
      - (also
      - Deposit
      - Cash
      - Cheques
      - From
      - Cash
      - Held)
  /api/role/{id}/releaseholdingdeposit:
    post:
      summary: Reset the holding deposit for a role
      description: Reset the holding deposit for a role.
      operationId: Role_ReleaseHoldingDepositByidByrelatedRoleId
      x-api-path-slug: apiroleidreleaseholdingdeposit-post
      parameters:
      - in: path
        name: id
      - in: query
        name: relatedRoleId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Holding
      - Deposita
      - Role
  /api/role/{id}/setholdingdeposit:
    post:
      summary: Set holding deposit for marketing role
      description: Set holding deposit for marketing role.
      operationId: Role_SetHoldingDepositByidBysetHoldingDepositDataContract
      x-api-path-slug: apiroleidsetholdingdeposit-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setHoldingDepositDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Holding
      - Depositmarketing
      - Role
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