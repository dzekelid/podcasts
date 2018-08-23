{
  "info": {
    "name": "Spreaker API Search Users",
    "_postman_id": "e4dbed50-0df7-4721-9c9a-2b4a0bb2f981",
    "description": "This API allows to find users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "c6771287-bd84-49f3-b921-c445ad98f707",
          "name": "getSearchQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "search/:query"
              ],
              "variable": [
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search users, shows and episodes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da76f299-6be2-4fc0-9bed-0b35de1a061c"
            }
          ]
        },
        {
          "id": "54d88d8e-bb14-438f-b6f3-6d10e1bd93cc",
          "name": "getUsersSearchQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "users/search/:query"
              ],
              "variable": [
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows to find users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e10a6440-b8a1-4f36-9c51-6736c86fff88"
            }
          ]
        }
      ]
    }
  ]
}