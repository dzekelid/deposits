{
  "info": {
    "name": "Capital One DevExchange Delete a specific existing deposit",
    "_postman_id": "02e38c88-6077-4d05-b617-2fb3ea0d6d0e",
    "description": "Deletes the specific deposit",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "f7924774-5a7d-4453-aa2f-1bd9762ef644",
          "name": "deletes-the-specific-deposit",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specific deposit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fc81a7e-6cfe-424f-9cb5-810b6f2009ad"
            }
          ]
        }
      ]
    }
  ]
}