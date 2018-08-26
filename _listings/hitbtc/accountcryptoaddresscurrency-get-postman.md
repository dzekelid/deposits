{
  "info": {
    "name": "HitBTC Get Deposit Crypro Address",
    "_postman_id": "48b211cb-61a3-45be-9367-b44035b7f0ed",
    "description": "Get deposit crypro address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deposit",
      "item": [
        {
          "id": "424a0bee-764a-480d-abb3-9a9bf31cb1cd",
          "name": "getAccountCryptoAddressCurrency",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/address/:currency"
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get deposit crypro address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "affeb90e-13f5-460d-bfd5-48e1726079d9"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "e24428aa-1402-4c7c-b5b5-ab24858d4cbf",
          "name": "postAccountCryptoAddressCurrency",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/address/:currency"
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create new deposit crypro address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "741a1f36-81cd-4164-83c3-7ca04a7b69de"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api/2"
    }
  ]
}