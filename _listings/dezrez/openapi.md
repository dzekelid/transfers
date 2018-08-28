swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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