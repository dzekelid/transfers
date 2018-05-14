{
  "info": {
    "name": "Capital One DevExchange Delete a specific existing transfer",
    "_postman_id": "23ea6335-e620-4d6e-a58d-fdd522023c0f",
    "description": "Deletes the specific transfer",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "57e41fcd-9574-4c1c-9899-2762de0d1337",
          "name": "deletes-the-specific-transfer",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specific transfer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b725ae1-0d62-460e-a987-900043011ab9"
            }
          ]
        }
      ]
    }
  ]
}