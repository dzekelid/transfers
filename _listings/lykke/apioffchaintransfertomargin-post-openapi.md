---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Offchain Transfertomargin
  version: 1.0.0
  description: Add api offchain transfertomargin.
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
  /api/Ethereum/{operationId}/transfer:
    post:
      summary: Add API Ethereum Operation Transfer
      description: Add api ethereum operation transfer.
      operationId: ApiEthereumByOperationIdTransferPost
      x-api-path-slug: apiethereumoperationidtransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: operationId
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Operation
      - Transfer
  /api/TrustedWallets/{operationId}/transfer:
    post:
      summary: Add API Trustedwallets Operation Transfer
      description: Add api trustedwallets operation transfer.
      operationId: Transfer
      x-api-path-slug: apitrustedwalletsoperationidtransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: operationId
      responses:
        200:
          description: OK
      tags:
      - Trustedwallets
      - Operation
      - Transfer
  /api/TransferInfo:
    get:
      summary: Get API Transferinfo
      description: Get api transferinfo.
      operationId: ApiTransferInfoGet
      x-api-path-slug: apitransferinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: transferId
      responses:
        200:
          description: OK
      tags:
      - Transferinfo
  /api/BankTransferRequest:
    post:
      summary: Add API Banktransferrequest
      description: Add api banktransferrequest.
      operationId: ApiBankTransferRequestPost
      x-api-path-slug: apibanktransferrequest-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transferReq
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Banktransferrequest
  /api/BcnTransactionByTransfer/{id}:
    get:
      summary: Get API Bcntransactionbytransfer
      description: Get api bcntransactionbytransfer.
      operationId: ApiBcnTransactionByTransferByIdGet
      x-api-path-slug: apibcntransactionbytransferid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbytransfer
  /api/GenerateTransferTransaction:
    post:
      summary: Add API Generatetransfertransaction
      description: Add api generatetransfertransaction.
      operationId: ApiGenerateTransferTransactionPost
      x-api-path-slug: apigeneratetransfertransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Generatetransfertransaction
  /api/offchain/requestTransfer:
    post:
      summary: Add API Offchain Requesttransfer
      description: Add api offchain requesttransfer.
      operationId: ApiOffchainRequestTransferPost
      x-api-path-slug: apioffchainrequesttransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Requesttransfer
  /api/offchain/transferToMargin:
    post:
      summary: Add API Offchain Transfertomargin
      description: Add api offchain transfertomargin.
      operationId: ApiOffchainTransferToMarginPost
      x-api-path-slug: apioffchaintransfertomargin-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Transfertomargin
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