{
  "info": {
    "name": "Spreaker API Get Owned Media",
    "_postman_id": "2b3168a8-f43e-4ab7-aeb8-999a4f50e8e1",
    "description": "Get a paginated list of media owned by <user_id> filtered by type:.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Episode",
      "item": [
        {
          "id": "79450ade-f6ae-434d-ba62-848fffdb90f8",
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
              "id": "a2dd3fcf-4949-4e43-9004-7f72d8935b9a"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "d7b58fe4-28cb-4e9f-b47f-51f198a7e211",
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
              "id": "8c87e659-1110-485e-9f05-7912b28e4f39"
            }
          ]
        }
      ]
    },
    {
      "name": "Owned",
      "item": [
        {
          "id": "f8f41280-8946-4b33-8c4a-2336c0c936e9",
          "name": "getLibraryUserEffectsOwned",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id/effects/owned"
              ],
              "query": [
                {
                  "key": "sort_col",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_dir",
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
            "description": "Get a paginated list of media owned by <user_id> filtered by type:."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adb02c54-9df1-46ea-b972-18d11efc8742"
            }
          ]
        }
      ]
    }
  ]
}