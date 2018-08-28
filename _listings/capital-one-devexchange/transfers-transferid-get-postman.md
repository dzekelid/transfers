{
  "info": {
    "name": "Capital One DevExchange Get transfer by id",
    "_postman_id": "b8012904-e136-4e9b-98cf-3522b655a10b",
    "description": "Returns the transfer with the specific id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "4c1c4ad5-5670-490e-a129-d844b0e3bbc4",
          "name": "returns-the-transfer-with-the-specific-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "transfers/:transferId"
              ],
              "variable": [
                {
                  "id": "transferId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the transfer with the specific id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3179f259-dfd9-4191-a6cc-b65b7a93665e"
            }
          ]
        }
      ]
    }
  ]
}