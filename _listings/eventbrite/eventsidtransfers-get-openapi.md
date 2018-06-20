---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Events Transfers
  description: Returns a list of transfers for the event.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/transfers/:
    get:
      summary: Get Events Transfers
      description: Returns a list of transfers for the event.
      operationId: getEventsTransfers
      x-api-path-slug: eventsidtransfers-get
      parameters:
      - in: query
        name: changed_since
        description: Only return transfers changed on or after the time given
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Transfers
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