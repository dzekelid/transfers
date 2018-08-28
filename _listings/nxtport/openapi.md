swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
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