{
  "info": {
    "name": "Spreaker API Facebook Settings",
    "_postman_id": "55d9f917-08ab-434f-b300-a05ac005f81d",
    "description": "Edit facebook share settings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Facebook",
      "item": [
        {
          "id": "13c0a551-2cee-4985-b585-482195dfc9a3",
          "name": "getUserUserActionsFacebook",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/actions/facebook"
              ],
              "query": [
                {
                  "key": "EPISODE_BROADCAST",
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
            "description": "Edit facebook share settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51fdcb3b-201d-4b29-a7a5-04d51dc04452"
            }
          ]
        }
      ]
    }
  ]
}