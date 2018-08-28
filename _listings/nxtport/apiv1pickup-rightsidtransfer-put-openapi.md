---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort T-mining Secure Container Release API Transfer
  description: Transfer the PickupRight to another Organization (a subcontractor).
  contact:
    name: T-Mining API support
    url: http://support.t-mining.be/
    email: support@t-mining.be
  version: 1.0.0
host: api.nxtport.eu
basePath: /blockchain
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/pickup_rights/{id}/transfer:
    put:
      summary: Transfer
      description: Transfer the PickupRight to another Organization (a subcontractor).
      operationId: putApiV1PickupRightsTransfer
      x-api-path-slug: apiv1pickup-rightsidtransfer-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of the PickupRight (as reported by List PickupRights)
      responses:
        200:
          description: OK
      tags:
      - Transfer
  /api/v1/pickup_rights/{id}/revoke_transfer:
    put:
      summary: Revoke Transfer
      description: Revoke the current PickupRight transfer. This must be used in case
        you did a transfer of a PickupRight to another Organization and you want to
        cancel this. This action is only possible as long as the PickupRight is not
        assigned.
      operationId: putApiV1PickupRightsRevokeTransfer
      x-api-path-slug: apiv1pickup-rightsidrevoke-transfer-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the PickupRight as reported by List PickupRights
      responses:
        200:
          description: OK
      tags:
      - Revoke
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