{
  "info": {
    "name": "Capital One DevExchange Get all transfers",
    "_postman_id": "88f7d732-89f5-4404-8a87-2f0cfec5c709",
    "description": "Returns the transfers that you are involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "f389c440-9457-414c-b4d0-f61efc96cc4a",
          "name": "returns-the-transfers-that-you-are-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id/transfers"
              ],
              "query": [
                {
                  "key": "type",
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
            "description": "Returns the transfers that you are involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20eb6308-7340-49e6-a901-0e6b9931a954"
            }
          ]
        }
      ]
    }
  ]
}