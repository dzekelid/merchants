{
  "info": {
    "name": "Capital One DevExchange Get merchant by id",
    "_postman_id": "b4a8591a-f1a5-45ce-85b4-364abcc083d4",
    "description": "Returns the merchant with the specific id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "066d00ea-cdaf-49cc-9265-cd57c5a3a5d1",
          "name": "returns-the-merchant-with-the-specific-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "merchants/:id"
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
            "description": "Returns the merchant with the specific id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c8346ae-64cb-4bb8-98c1-b7558f3d1522"
            }
          ]
        }
      ]
    }
  ]
}