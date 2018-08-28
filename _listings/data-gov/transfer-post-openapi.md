---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Transfer
  description: Initiate transfer request
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