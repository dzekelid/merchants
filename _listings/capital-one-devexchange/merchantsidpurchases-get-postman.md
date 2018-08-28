{
  "info": {
    "name": "Capital One DevExchange Get all purchases by merchant",
    "_postman_id": "d549574d-8852-4ac8-a764-7cd96caa3e9c",
    "description": "Returns the purchases that a merchant is involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "6c811809-b497-4203-88e6-72ee3becc4dc",
          "name": "returns-the-purchases-that-a-merchant-is-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "merchants/:id/purchases"
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
            "description": "Returns the purchases that a merchant is involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cced6724-0669-4fee-a1d8-f7c8f910ed53"
            }
          ]
        }
      ]
    }
  ]
}