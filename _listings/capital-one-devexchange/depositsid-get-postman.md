{
  "info": {
    "name": "Capital One DevExchange Get deposit by id",
    "_postman_id": "48953d1b-cd49-49ab-b10c-76600c9f4edc",
    "description": "Returns the deposit with the specific id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "05050d99-f249-45b8-9f87-9ef2852aebaf",
          "name": "returns-the-deposit-with-the-specific-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "deposits/:id"
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
            "description": "Returns the deposit with the specific id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28c5187b-95cf-48ae-8709-2e6850b616c4"
            }
          ]
        }
      ]
    }
  ]
}