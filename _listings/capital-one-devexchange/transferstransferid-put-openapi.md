---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Update a specific existing transfer
  description: Updates the specific transfer
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
  /accounts/{id}/transfers:
    get:
      summary: Get all transfers
      description: Returns the transfers that you are involved in.
      operationId: returns-the-transfers-that-you-are-involved-in
      x-api-path-slug: accountsidtransfers-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the transfer
      - in: query
        name: type
        description: When param is empty, will return transfers associated with account
          where account is payer AND payee
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Transfers
    post:
      summary: Create a transfer
      description: Creates a transfer where the account with the ID specified is the
        payer.
      operationId: creates-a-transfer-where-the-account-with-the-id-specified-is-the-payer
      x-api-path-slug: accountsidtransfers-post
      parameters:
      - in: body
        name: body
        description: Transfer to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account payer in transfer
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Transfers
  /transfers/{transferId}:
    get:
      summary: Get transfer by id
      description: Returns the transfer with the specific id
      operationId: returns-the-transfer-with-the-specific-id
      x-api-path-slug: transferstransferid-get
      parameters:
      - in: path
        name: transferId
        description: ID of the transfer that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Transfers
      - Transfer
    put:
      summary: Update a specific existing transfer
      description: Updates the specific transfer
      operationId: updates-the-specific-transfer
      x-api-path-slug: transferstransferid-put
      parameters:
      - in: body
        name: body
        description: Transfer to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: transferId
        description: ID of the transfer that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Transfers
      - Transfer
    delete:
      summary: Delete a specific existing transfer
      description: Deletes the specific transfer
      operationId: deletes-the-specific-transfer
      x-api-path-slug: transferstransferid-delete
      parameters:
      - in: path
        name: transferId
        description: ID of the transfer that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Transfers
      - Transfer
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