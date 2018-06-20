{
  "info": {
    "name": "Stripe Get Transfers Transfer Reversals",
    "_postman_id": "03861845-19ef-4086-a2e7-60b0822c49dc",
    "description": "By default, you can see the 10 most recent reversals stored directly on the transfer object, but you can also retrieve details about a specific reversal stored on the transfer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transfers",
      "item": [
        {
          "id": "0abe2866-10ab-4890-9bd3-49045a6529a7",
          "name": "getTransfersTransferReversals",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "transfers/:transfer/reversals/:id"
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
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "By default, you can see the 10 most recent reversals stored directly on the transfer object, but you can also retrieve details about a specific reversal stored on the transfer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b87cba09-29e8-4965-b42d-0c25279ef36b"
            }
          ]
        }
      ]
    }
  ]
}