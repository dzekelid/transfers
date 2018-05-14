{
  "info": {
    "name": "Stripe Get Transfers Transfer",
    "_postman_id": "5be27eb6-e21e-40b0-8c53-f74f9be88c0c",
    "description": "Retrieves the details of an existing transfer. Supply the unique transfer ID from either a transfer creation request or the transfer list, and Stripe will return the corresponding transfer information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transfers",
      "item": [
        {
          "id": "49e3fba7-8e28-4739-ba36-f79d43e30880",
          "name": "getTransfersTransfer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "transfers/:transfer"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "transfer",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details of an existing transfer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d6840bf-d542-45a4-b470-e36a90feacd9"
            }
          ]
        }
      ]
    }
  ]
}