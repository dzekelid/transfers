---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /BankTransfers:
    get:
      summary: Get Banks Transfers
      description: Get banktransfers.
      operationId: getBanktransfers
      x-api-path-slug: banktransfers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
    put:
      summary: Put Banks Transfers
      description: Put banktransfers.
      operationId: putBanktransfers
      x-api-path-slug: banktransfers-put
      parameters:
      - in: body
        name: BankTransfers
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
    x-related-model:
      summary: X-related-model Banks Transfers
      description: X-related-model banktransfers.
      operationId: x-related-modelBanktransfers
      x-api-path-slug: banktransfers-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
  /BankTransfers/{BankTransferID}:
    get:
      summary: Get Banks Transfers
      description: Get banktransfers banktransfer.
      operationId: getBanktransfersBanktransfer
      x-api-path-slug: banktransfersbanktransferid-get
      parameters:
      - in: path
        name: BankTransferID
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
    x-related-model:
      summary: X-related-model Banks Transfers
      description: X-related-model banktransfers banktransfer.
      operationId: x-related-modelBanktransfersBanktransfer
      x-api-path-slug: banktransfersbanktransferid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
  /BankTransfers/{BankTransferID}/Attachments/{FileName}:
    get:
      summary: Get Banks Transfers Attachments Filename
      description: Get banktransfers banktransfer attachments filename.
      operationId: getBanktransfersBanktransferAttachmentsFilename
      x-api-path-slug: banktransfersbanktransferidattachmentsfilename-get
      parameters:
      - in: path
        name: BankTransferID
        description: The Xero generated unique identifier for an BankTransfer
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
      - Attachments
      - FileName
    post:
      summary: Post Banks Transfers Attachments Filename
      description: Post banktransfers banktransfer attachments filename.
      operationId: postBanktransfersBanktransferAttachmentsFilename
      x-api-path-slug: banktransfersbanktransferidattachmentsfilename-post
      parameters:
      - in: path
        name: BankTransferID
        description: The Xero generated unique identifier for a BankTransfer
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
      - Attachments
      - FileName
---