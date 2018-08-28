swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transfer/:
    get:
      summary: Get Transfer
      description: List all transfer requests
      operationId: getTransfer
      x-api-path-slug: transfer-get
      responses:
        200:
          description: OK
      tags:
      - Transfer
    post:
      summary: Add Transfer
      description: Initiate transfer request
      operationId: postTransfer
      x-api-path-slug: transfer-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Transfer
  /transfer/{id}/:
    get:
      summary: Get Transfer
      description: Fetch a transfer request given its identifier
      operationId: getTransfer
      x-api-path-slug: transferid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Transfer
    post:
      summary: Add Transfer
      description: Respond to a transfer request
      operationId: postTransfer
      x-api-path-slug: transferid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Transfer