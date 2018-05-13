{
  "info": {
    "name": "Capital One DevExchange Get all merchants",
    "_postman_id": "da6f4b9d-30c0-4b9e-ba96-e2493d8b9462",
    "description": "Returns the merchants that have been assigned to you.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "1e6598ad-cef3-464f-91fd-92afda85684f",
          "name": "returns-the-merchants-that-have-been-assigned-to-you",
          "request": {
            "url": "http://api.reimaginebanking.com/merchants?lat=%7B%7D&lng=%7B%7D&rad=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the merchants that have been assigned to you"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a97301c-9f18-4e8f-87f4-92c6c68c543c"
            }
          ]
        }
      ]
    }
  ]
}