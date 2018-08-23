{
  "info": {
    "name": "Spreaker API Create Media",
    "_postman_id": "1bf9a80c-8c11-458e-bb2c-1e4d8266c48c",
    "description": "Upload a new Media in the specified user library",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Episode",
      "item": [
        {
          "id": "8d5eb2cd-20a2-4515-b1d4-5c5a5c3aed68",
          "name": "getEpisodeEpisodeMedia",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id/media"
              ],
              "variable": [
                {
                  "id": "episode_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Episode Media List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49545c98-e54b-43a2-94db-35580209cb8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "3e2aff03-09a1-4a87-89a8-f64e5eafe15e",
          "name": "postLibraryUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id"
              ],
              "query": [
                {
                  "key": "Filedata",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "length",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "style_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new Media in the specified user library"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56a7163f-dd8f-4776-89e7-58bc4c476683"
            }
          ]
        }
      ]
    }
  ]
}