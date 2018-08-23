{
  "info": {
    "name": "Spreaker API Get User Actions",
    "_postman_id": "4f15ce86-f1b7-46d1-8d57-08e3d130211f",
    "description": "Retrieves the user actions settings",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "1e27b386-3999-4e7c-8910-4186e0641a6b",
          "name": "getUserUserActions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/actions"
              ],
              "query": [
                {
                  "key": "EPISODE_BROADCAST",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "FACEBOOK",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_MESSAGE",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_MESSAGE",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "TWITTER",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "USER_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the user actions settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bc9e5e7-7081-426c-8036-92c8f96b57b0"
            }
          ]
        }
      ]
    }
  ]
}