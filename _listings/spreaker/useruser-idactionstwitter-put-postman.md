{
  "info": {
    "name": "Spreaker API Twitter Settings",
    "_postman_id": "bacdc7ed-9924-49f5-ac36-60657d59a4f8",
    "description": "Edit twitter share settings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Facebook",
      "item": [
        {
          "id": "7258403d-3ecb-4851-aa8e-6b362d037ee9",
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
              "id": "c2a73661-c8ee-459f-97bc-c5e7c2b38c14"
            }
          ]
        }
      ]
    },
    {
      "name": "Twitter",
      "item": [
        {
          "id": "94adbd62-410a-4fe9-afb4-01cfea48cfbc",
          "name": "putUserUserActionsTwitter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/actions/twitter"
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
                  "key": "SHOW_FOLLOW",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit twitter share settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34f8f768-e58e-4394-ad86-156efb53f70d"
            }
          ]
        }
      ]
    }
  ]
}