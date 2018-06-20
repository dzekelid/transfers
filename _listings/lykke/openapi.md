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
  /api/Ethereum/transfers:
    get:
      summary: Get API Ethereum Transfers
      description: Get api ethereum transfers.
      operationId: ApiEthereumTransfersGet
      x-api-path-slug: apiethereumtransfers-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Transfers
    post:
      summary: Add API Ethereum Transfers
      description: Add api ethereum transfers.
      operationId: ApiEthereumTransfersPost
      x-api-path-slug: apiethereumtransfers-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: operations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Transfers
---