{
  "info": {
    "name": "Capital One DevExchange Get all purchases by account and merchant",
    "_postman_id": "fb2a1945-0307-4c95-bda6-ebe7289a7d68",
    "description": "Returns the purchases that a merchant is involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "776a5036-29cc-44c0-a61e-81747a0cfdd4",
          "name": "returns-the-purchases-that-a-merchant-is-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "merchants/:id/accounts/:accountId/purchases"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Returns the purchases that a merchant is involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f4e84ae-dd2a-4dcf-8839-ecd01dd7e571"
            }
          ]
        }
      ]
    }
  ]
}