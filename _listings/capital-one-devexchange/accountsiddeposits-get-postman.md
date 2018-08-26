{
  "info": {
    "name": "Capital One DevExchange Get all deposits",
    "_postman_id": "a7bc4059-1fea-4614-885b-02976f6817fa",
    "description": "Returns the deposits that you are involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "efa1c6a3-611e-4080-8685-b2fc9910a318",
          "name": "returns-the-deposits-that-you-are-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id/deposits"
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
            "description": "Returns the deposits that you are involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bde31c7-0f19-476f-8527-89636b4c1b88"
            }
          ]
        }
      ]
    }
  ]
}