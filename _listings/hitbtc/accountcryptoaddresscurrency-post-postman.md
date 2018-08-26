{
  "info": {
    "name": "HitBTC Create New Deposit Crypro Address",
    "_postman_id": "09645cb1-bad2-4b64-82dd-52b9b4205f08",
    "description": "Create new deposit crypro address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deposit",
      "item": [
        {
          "id": "c4ece7ab-ac52-406e-817f-86e1e2c9d13f",
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
              "id": "4a917163-ddba-4a1d-b6c8-35822b09dc8a"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "9ae67fea-d5a5-4e46-bfe6-d5f95630dba5",
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
              "id": "58d6e130-78f1-49c1-b367-c12a2bc9f5eb"
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