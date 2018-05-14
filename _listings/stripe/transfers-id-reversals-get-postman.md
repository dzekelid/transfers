{
  "info": {
    "name": "Stripe Get Transfers  Reversals",
    "_postman_id": "da98edb6-dd36-4e0b-9713-e0162aa24132",
    "description": "You can see a list of the reversals belonging to a specific transfer. Note that the 10 most recent reversals are always available by default on the transfer object. If you need more than those 10, you can use this API method and the limit and starting_after parameters to page through additional reversals.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transfers",
      "item": [
        {
          "id": "7eedf41f-a5a9-4d53-8efe-30dff95d96f3",
          "name": "getTransfersReversals",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "transfers/:id/reversals"
              ],
              "query": [
                {
                  "key": "ending_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starting_after",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can see a list of the reversals belonging to a specific transfer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca7365c5-a033-4d8e-8cb0-89aba67aa46c"
            }
          ]
        }
      ]
    }
  ]
}